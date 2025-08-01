---
title: Export a list of users and their access levels
titleSuffix: Azure DevOps
description: Determine the access level-stakeholder, basic, advanced, or Visual Studio Enterprise-granted to user accounts.  
ms.subservice: azure-devops-security
ms.assetid: 
ms.topic: how-to
ms.reviewer:  
ms.author: chcomley
author: chcomley
monikerRange: 'azure-devops'
ms.date: 04/08/2025
---

# Export a list of users and their access levels

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-eq-azure-devops.md)]

<a id="export-audit-log" >  </a>

You can get a list of users and groups that have access to your organization in Azure DevOps by exporting users. The downloaded list also indicates access levels.

## Prerequisites

[!INCLUDE [prerequisites-pca-only](../../includes/prerequisites-pca-only.md)]

## Export a list of users

From your web portal or the Azure DevOps CLI command, get a list of the users in your organization and view their access level information.

#### [Browser](#tab/browser)

1. Select the :::image type="icon" source="../../media/icons/project-icon.png" border="false"::: Azure DevOps logo to open **Projects**. Then choose **Organization settings**. 

	> [!div class="mx-imgBorder"]  
	> ![Screenshot of highlighted Organization settings button.](../../media/settings/open-admin-settings-vert.png)  

2. Select **Users** > **Export users**.

	> [!div class="mx-imgBorder"]  
	> ![Screenshot of Export users button.](media/export-users-audit/export-new-nav.png) 

#### [Azure DevOps CLI](#tab/azure-devops-cli)

[Add a user](../accounts/add-organization-users.md#add-user) | [List users](#list-users) | [Remove a user](../accounts/delete-organization-users.md#remove-user) | [Update a user](../accounts/add-organization-users.md#update-user) | [Show users](../accounts/add-organization-users.md#show-users)

<a id="list-users"></a> 

### List users

You can list the users in an organization with the [az devops user list](/cli/azure/devops/user#az-devops-user-list) command. This action doesn't apply to users added via Microsoft Entra groups, as certain commands or features might not directly apply to users added via Microsoft Entra. When you export the list, you might notice that group users get indicated with an "assignmentSource" of "groupRule." This assignment signifies that their access gets determined by the group membership rules, rather than individual settings. To get started, see [Azure DevOps CLI](../../cli/index.md).

```azurecli
az devops user list [--org] [--skip] [--top]
```

#### Parameters

- **org**: Azure DevOps organization URL. Configure the default organization using `az devops configure -d organization=ORG_URL`. Required if not configured as default or picked up using `git config`. For example, `--org https://dev.azure.com/MyOrganizationName/`.
- **skip**: Optional. Number of users to skip.
- **top**: Optional. Maximum number of users to return. The maximum value is 10000; the default value is 100.

#### Example

The following command returns five users in your organization without skipping any and shows the result in table format.

```azurecli
az devops user list --skip 0 --top 5  --output table

ID                                    Display Name            Email                          License Type    Access Level    Status
------------------------------------  ----------------------  -----------------------------  --------------  --------------  --------
3b5f0c34-4aec-4bf4-8708-1d36f0dbc468  Christie Church         fabrikamfiber1@contoso.com     stakeholder     Stakeholder     active
8c8c7d32-6b1b-47f4-b2e9-30b477b5ab3d  Chuck Reinhart          fabrikamfiber3@contoso.com     stakeholder     Stakeholder     active
3b5f0c34-4aec-4bf4-8708-1d36f0dbc468  contoso@contoso.com     contoso@contoso.com            stakeholder     Stakeholder     active
f14a4f19-9910-6116-9836-cccd6dd1b7b7  contoso2@contoso.com    contoso2@contoso.com           express         Basic           active
74be024c-ebf5-4993-81eb-81ae1551e45f  Helena Petersen         fabrikamfiber8@contoso.com     stakeholder     Stakeholder     active
```


* * *
 
## Related content

- [About access levels](access-levels.md)
- [Manage users and access in Azure DevOps](../accounts/add-organization-users.md) 
- [Default permissions and access](permissions-access.md)

