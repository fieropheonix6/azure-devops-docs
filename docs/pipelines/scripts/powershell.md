---
title: Use PowerShell scripts to customize pipelines
description: Learn how you can use a script to customize your pipeline.
ms.topic: conceptual
ms.assetid: 7D184F55-18BC-40E5-8BE7-283A0DB8E823
ms.date: 05/24/2024
monikerRange: '<= azure-devops'
---

# Use a PowerShell script to customize your pipeline

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]



When you're ready to move beyond the basics of compiling and testing your code, use a PowerShell script to add your team's business logic to your build pipeline. You can run Windows PowerShell on a [Windows build agent](../agents/windows-agent.md) or PowerShell Core on any platform. 

When you use the PowerShell task [PowerShell task](/azure/devops/pipelines/tasks/reference/powershell-v2), your PowerShell script runs in your pipeline. You can use PowerShell to access the Azure DevOps REST API, work with the Azure DevOps work items and test management, and call other services as needed.

## Add a PowerShell script
### [YAML](#tab/yaml)

The syntax for including PowerShell Core is slightly different from the syntax for Windows PowerShell. 

1. Push your PowerShell script to your repo.

1. Add a `pwsh` or `powershell` step to your pipeline
    The `pwsh` keyword is a shortcut for the [PowerShell task](/azure/devops/pipelines/tasks/reference/powershell-v2) for PowerShell Core. The `powershell` keyword is another shortcut for the [PowerShell task](/azure/devops/pipelines/tasks/reference/powershell-v2).

Examples:

```yaml
# for PowerShell Core
steps:
- pwsh: ./my-script.ps1

# for Windows PowerShell
steps:
- powershell: .\my-script.ps1
```

### [Classic](#tab/classic)

1. Add the PowerShell Script task to your pipeline. The same [PowerShell task](/azure/devops/pipelines/tasks/reference/powershell-v2) works for PowerShell Core and Windows PowerShell. 

    :::image type="content" source="media/powershell-script.png" alt-text="Screenshot of PowerShell task selection.":::

1. Add your file to the **Script Path**. 
    
    :::image type="content" source="media/powershell-update-script-path.png" alt-text="Screenshot of PowerShell task script path setting.":::

---

## Example PowerShell script: version assemblies

Here's an example script to version your assemblies. For the script to run successfully, you need to update your build number to use a format with four periods (example: `$(BuildDefinitionName)_$(Year:yyyy).$(Month).$(DayOfMonth)$(Rev:.r)`). Build number can also be referred to as run number.

### [YAML](#tab/yaml)

You can [customize your build number](../process/run-number.md) within a YAML pipeline with the `name` property. 

```yaml
name: $(BuildDefinitionName)_$(Year:yyyy).$(Month).$(DayOfMonth)$(Rev:.r)

pool:
  vmImage: windows-latest

steps:
- pwsh: echo $(Build.BuildNumber) //output updated build number
```
#### [Classic](#tab/classic)

:::moniker range=">= azure-devops-2022"

1. To customize your build number in a classic pipeline, first add the build task to your pipeline. 

    :::image type="content" source="media\powershell-script-task.png" alt-text="Screenshot of PowerShell script task.":::

1. Next, specify your build number.

    :::image type="content" source="media\build-number-format.png" alt-text="Screenshot of build number format setting.":::

1. Save your changes.
   
:::moniker-end

:::moniker range="< azure-devops-2022"

1. To customize your build number in a classic pipeline, first add the build task to your pipeline. 

    :::image type="content" source="media\powershell-script-task-2020.png" alt-text="Screenshot of PowerShell build task.":::

1. Next, specify your build number.

    :::image type="content" source="media\build-number-format-2019.png" alt-text="Screenshot of build number format setting.":::

1. Save your changes.

:::moniker-end

---

Example PowerShell script:

```ps
# If found use it to version the assemblies.
#
# For example, if the 'Build number format' build pipeline parameter 
# $(BuildDefinitionName)_$(Year:yyyy).$(Month).$(DayOfMonth)$(Rev:.r)
# then your build numbers come out like this:
# "Build HelloWorld_2013.07.19.1"
# This script would then apply version 2013.07.19.1 to your assemblies.
	
# Enable -Verbose option
[CmdletBinding()]
	
# Regular expression pattern to find the version in the build number 
# and then apply it to the assemblies
$VersionRegex = "\d+\.\d+\.\d+\.\d+"
	
# If this script is not running on a build server, remind user to 
# set environment variables so that this script can be debugged
if(-not ($Env:BUILD_SOURCESDIRECTORY -and $Env:BUILD_BUILDNUMBER))
{
	Write-Error "You must set the following environment variables"
	Write-Error "to test this script interactively."
	Write-Host '$Env:BUILD_SOURCESDIRECTORY - For example, enter something like:'
	Write-Host '$Env:BUILD_SOURCESDIRECTORY = "C:\code\FabrikamTFVC\HelloWorld"'
	Write-Host '$Env:BUILD_BUILDNUMBER - For example, enter something like:'
	Write-Host '$Env:BUILD_BUILDNUMBER = "Build HelloWorld_0000.00.00.0"'
	exit 1
}
	
# Make sure path to source code directory is available
if (-not $Env:BUILD_SOURCESDIRECTORY)
{
	Write-Error ("BUILD_SOURCESDIRECTORY environment variable is missing.")
	exit 1
}
elseif (-not (Test-Path $Env:BUILD_SOURCESDIRECTORY))
{
	Write-Error "BUILD_SOURCESDIRECTORY does not exist: $Env:BUILD_SOURCESDIRECTORY"
	exit 1
}
Write-Verbose "BUILD_SOURCESDIRECTORY: $Env:BUILD_SOURCESDIRECTORY"
	
# Make sure there is a build number
if (-not $Env:BUILD_BUILDNUMBER)
{
	Write-Error ("BUILD_BUILDNUMBER environment variable is missing.")
	exit 1
}
Write-Verbose "BUILD_BUILDNUMBER: $Env:BUILD_BUILDNUMBER"
	
# Get and validate the version data
$VersionData = [regex]::matches($Env:BUILD_BUILDNUMBER,$VersionRegex)
switch($VersionData.Count)
{
   0		
      { 
         Write-Error "Could not find version number data in BUILD_BUILDNUMBER."
         exit 1
      }
   1 {}
   default 
      { 
         Write-Warning "Found more than instance of version data in BUILD_BUILDNUMBER." 
         Write-Warning "Will assume first instance is version."
      }
}
$NewVersion = $VersionData[0]
Write-Verbose "Version: $NewVersion"
	
# Apply the version to the assembly property files
$files = gci $Env:BUILD_SOURCESDIRECTORY -recurse -include "*Properties*","My Project" | 
	?{ $_.PSIsContainer } | 
	foreach { gci -Path $_.FullName -Recurse -include AssemblyInfo.* }
if($files)
{
	Write-Verbose "Will apply $NewVersion to $($files.count) files."
	
	foreach ($file in $files) {
		$filecontent = Get-Content($file)
		attrib $file -r
		$filecontent -replace $VersionRegex, $NewVersion | Out-File $file
		Write-Verbose "$file.FullName - version applied"
	}
}
else
{
	Write-Warning "Found no files."
}
```

<a name="oauth"></a>

## Example PowerShell script: access REST API

In this example, you use the `SYSTEM_ACCESSTOKEN` variable to access the [Azure Pipelines REST API](../../integrate/index.md). 

#### [YAML](#tab/yaml)

You can use `$env:SYSTEM_ACCESSTOKEN` in your script in a YAML pipeline to access the OAuth token. 

The following example inline PowerShell script uses the OAuth token to access the Azure Pipelines REST API that retrieves the pipeline definition.

```yaml
- task: PowerShell@2
  inputs:
    targetType: 'inline'
    script: |
      $url = "$($env:SYSTEM_TEAMFOUNDATIONCOLLECTIONURI)$env:SYSTEM_TEAMPROJECTID/_apis/build/definitions/$($env:SYSTEM_DEFINITIONID)?api-version=5.0"
              Write-Host "URL: $url"
              $pipeline = Invoke-RestMethod -Uri $url -Headers @{
                  Authorization = "Bearer $env:SYSTEM_ACCESSTOKEN"
              }
              Write-Host "Pipeline = $($pipeline | ConvertTo-Json -Depth 100)"
  env:
     SYSTEM_ACCESSTOKEN: $(System.AccessToken)
```


#### [Classic](#tab/classic)

To enable your script to use the build process OAuth token, go to the **Tasks** tab of the build definition and select an **Agent job** and  select **Allow Scripts to Access OAuth Token** located in the **Additional options** section.

To enable your script to use the build process OAuth token, navigate to the **Tasks** tab of the build definition, select an **Agent job**, and in the **Additional options** section, select **Allow Scripts to Access OAuth Token**.

:::image type="content" source="media\Allow-scripts-to-access-oauth-token.png" alt-text="Screenshot enabling OAuth token access for scripts.":::

After you do that, your script can use to SYSTEM_ACCESSTOKEN environment variable to access the [Azure Pipelines REST API](../../integrate/index.md).

The following example PowerShell script uses the OAuth token to access the Azure Pipelines REST API that retrieves the pipeline definition.

```ps
$url = "$($env:SYSTEM_TEAMFOUNDATIONCOLLECTIONURI)$env:SYSTEM_TEAMPROJECTID/_apis/build/definitions/$($env:SYSTEM_DEFINITIONID)?api-version=5.0"
Write-Host "URL: $url"
$pipeline = Invoke-RestMethod -Uri $url -Headers @{
    Authorization = "Bearer $env:SYSTEM_ACCESSTOKEN"
}
Write-Host "Pipeline = $($pipeline | ConvertTo-Json -Depth 100)"
```

--- 


## FAQ
<!-- BEGINSECTION class="md-qanda" -->


### What variables are available for me to use in my scripts?

You can use [predefined variables](../build/variables.md) in your scripts. For more information on available variables and how to use them, see [Use predefined variables](../build/variables.md).

[!INCLUDE [include](../includes/variable-set-in-script-qa.md)]

### Which branch of the script does the build run?

The build uses the active branch of your code. If your pipeline run uses the `main` branch, your script also uses the `main` branch. 
### What kinds of parameters can I use?

You can use named parameters. Other kinds of parameters, such as switch parameters, aren't supported. You see errors if you try to use switch parameters. 

::: moniker range="< azure-devops"
[!INCLUDE [temp](../includes/qa-versions.md)]
::: moniker-end

<!-- ENDSECTION -->
