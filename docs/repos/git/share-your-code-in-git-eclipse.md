---
title: Share your Eclipse project with Git
titleSuffix: Azure Repos
description: Share code in Git using Eclipse
ms.assetid: a00b91da-9f74-44f2-8c48-04bfd50a74c3
ms.service: azure-devops-repos
ms.topic: quickstart
monikerRange: '<= azure-devops'
ms.subservice: azure-devops-repos-git
ms.date: 05/13/2019
ms.custom:
  - archive-candidate
  - sfi-image-nochange
---


# Share your code in Git using Eclipse

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]

Share your Eclipse project with your team in an Azure DevOps Services/TFS Git repo.

## Prerequisites

[!INCLUDE [azure-repos-prerequisites](includes/azure-repos-prerequisites.md)]

<a name="git"></a>

## Use Team Explorer Everywhere

[Team Explorer Everywhere](https://github.com/Microsoft/team-explorer-everywhere) is an open-source Eclipse plug-in to connect Eclipse to Azure DevOps Services or Team Foundation Server. If you're working with Azure DevOps Services/TFS and Eclipse, use this plugin to connect to your repos, builds, and work items. 

> [!NOTE]
> The Team Explorer Everywhere plug-in works with Eclipse versions 4.2 (Juno) - 4.6 (Neon).

1. [Install the Team Explorer Everywhere plug-in](/previous-versions/azure/devops/all/java/download-eclipse-plug-in#to-install-team-explorer-everywhere-from-within-eclipse).

2. Add the Team Explorer Everywhere view in Eclipse. Go to **Window, Show View** and select **Other...** Search for **Team Explorer**, select the **Team Explorer** view, and select **OK**.   

   ![Add the Team Explorer view to Eclipse](media/share-your-code-in-git-eclipse/add_team_explorer_to_eclipse.png)

## Connect to Azure DevOps Services

1. In the Team Explorer Everywhere view, select **Connect to VSTS or a Team Foundation Server** . 

   ![Select Connect to Team Foundation Server to connect your TFS or Azure DevOps organization](media/share-your-code-in-git-eclipse/connect_to_vsts_from_tee.png)
   

2. If you know your Azure DevOps Services or Team Foundation Server account URL, select the **Servers...** button under **Connect to a Team Foundation Server or Azure DevOps organization** to add your TFS server or account to the drop-down list. 
   If you don't know your account information for Azure DevOps Services, select **Browse Visual Studio Services** and select **Next**.

   ![Add Existing Project Dialog](media/share-your-code-in-git-eclipse/tee_existing_team_project.png)

   Either choice will prompt for your credentials before continuing further. 

3. Select the project where you will share your code from the **Project Selection** dialog and select **Finish**.

## Create a local Git repo for your Eclipse project

Before you can push your project to Azure Repos, you need to add it to a local Git repo.

> [!NOTE]
> If your code is already in a local Git repo, you can skip this step.

1. With your project open in Eclipse, right-click the project name in Project Explorer and select **Team, Share Project...** Select **Git** and select **Next**. 

2. Select **Create...** from the **Configure Git Repository** window and choose a folder for your local Git repo. Select **Finish**.

    ![Create a local Git repo in Eclipse](media/share-your-code-in-git-eclipse/eclipse_create_repo.png)

3. Right-click your project in Project Explorer and select **Team, Commit...**. Stage your changes by dragging your files to the **Staged Changes** field, enter a commit message, then select **Commit**.

   ![Commit your code with Git in Eclipse](media/share-your-code-in-git-eclipse/commit_files_in_eclipse.png)

## Push your project to your Azure DevOps Services/TFS repo

1. In Team Explorer Everywhere, select **Git Repositories**, then right-click the empty repo you want to push your Eclipse project to and select **Copy Clone URL**. If you don't have an empty Git repo created in Azure DevOps Services/TFS yet, you can create one using [these instructions](create-new-repo.md).

    ![Copy the Git repo clone URL in Team Explorer Everywhere with a right-click](media/share-your-code-in-git-eclipse/tee_copy_clone_url.png)
    
2. In Package Explorer, right-click your project and Select **Team, Push Branch ...** . Paste the clone URL from the clipboard into the **URI** field and select **Next**. Make sure **Configure upstream for push and pull** is selected in the next window and select **Next**.

    ![Push your code to Azure Repos using the Clone URL from the web](media/share-your-code-in-git-eclipse/push_commits_to_team_services.png)
    
3. Review the changes and select **Finish** in the **Push Branch** window.

Your project code is now in your Git repo.

## Troubleshooting

### What if the Git views for commit and push don't show up?

You can [download EGit](https://www.eclipse.org/egit/) to use Git with Eclipse.

## Next steps

> [!div class="nextstepaction"]
> [Learn more about using Git in the Git tutorial](gitworkflow.md)
