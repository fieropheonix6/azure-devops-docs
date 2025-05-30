---
title: Get Started as a Project Administrator
titleSuffix:  Azure DevOps
description: Learn how to structure a project, manage users, and more to support your software development teams in Azure DevOps.
ms.subservice: azure-devops-new-user
ms.author: chcomley
author: chcomley
ms.topic: concept-article
monikerRange: '<= azure-devops'
ms.date: 05/05/2025
#customer intent: As a project administrator, I want to structure my projects and manage users in Azure DevOps, so I can support my development teams.
---

# Get started managing your project 

[!INCLUDE [version-lt-eq-azure-devops.md](../includes/version-lt-eq-azure-devops.md)]  

With most Azure DevOps Services, you can start using the service and configure resources as you go. No up-front work is required. Most settings define defaults. 

If you created a project or you're added to the **Project Administrators** group, get familiar with the administrative tasks you're charged with. There are a few tasks you might want to do to ensure a smooth operational experience. 

## Prerequisites

[!INCLUDE [prerequisites-project-administrator-only](../includes/prerequisites-project-administrator-only.md)]

> [!NOTE]   
> This article provides an overview of tasks a member of the **Project Administrators** group should review and attend to. For information on tasks to be performed by members of the **Project Collection Administrators** group, see [Manage your organization or project collection](manage-organization-collection.md).

[!INCLUDE [add-users-project](../includes/get-started/add-users-project.md)]  
 
[!INCLUDE [share-project-vision](../includes/get-started/share-project-vision.md)]  

[!INCLUDE [enable-remove-services](../includes/get-started/enable-remove-services.md)]  

## Manage security and permissions

Permissions and security groups control access to specific tasks. To quickly understand the defaults configured for your project, see [Default permissions and access](../organizations/security/permissions-access.md).  

[!INCLUDE [project-level-permissions](../organizations/security/includes/project-level-permissions.md)]

For more information about security and setting permissions at the project-level, review the following articles:

- [Get started with permissions, access, and security groups](../organizations/security/about-permissions.md)   
- [Change permissions at the project-level](../organizations/security/change-project-level-permissions.md) 
 
### Add members to the Project Administrators group 

[!INCLUDE [add-project-administrators](../includes/get-started/add-project-administrators.md)]  

### Grant or restrict permissions  

Permissions are managed at the following three levels and through role-based assignments:

- object
- project
- organization or collection

As a member of the **Project Administrators** group, you can grant or restrict permissions for all objects at the project-level. To delegate specific tasks to others, a good approach is to add the users to a built-in or custom security group, or add them to a specific role. For more information, see the following articles:

- [Use role-based permissions](../organizations/security/about-permissions.md#role-based-permissions)
- [Add/remove users or groups, manage security groups](../organizations/security/add-remove-manage-user-group-security-group.md)
- [Manage access to specific features and functions](../organizations/security/restrict-access.md)   
- [Set object-level permissions](../organizations/security/set-object-level-permissions.md) 

[!INCLUDE [review-notifications](../includes/get-started/review-notifications.md)] 

[!INCLUDE [determine-traceability-requirements](../includes/get-started/determine-traceability-requirements.md)]  

## Set DevOps policies 

Set policies to support collaboration across your teams and automatically remove obsolete files. To set policies that govern Azure Repos, Azure Pipelines, and Azure Test Plans, review the following articles: 

- [Manage branch policies](../repos/git/branch-policies.md)  
- [Add Team Foundation Version Control (TFVC) check-in policies](../repos/tfvc/add-check-policies.md)  
- [Set build and release pipeline retention policies](../pipelines/policies/retention.md) 
- [Set test retention policies](../test/how-long-to-keep-test-results.md) 
 
## Configure and customize Azure Boards 

You can configure and customize Azure Boards to support many business requirements for planning and tracking work. At a minimum, you should configure the following elements:

- **Area paths** to group work items by team, product, or feature area
- **Iteration paths** to group work into sprints, milestones, or other event-specific or time-related periods 

If you're new to Azure Boards and want an in-depth overview of what you can configure and customize, see [Configure and customize Azure Boards](../boards/configure-customize.md).

[!INCLUDE [define-area-iteration-paths](../includes/get-started/define-area-iteration-paths.md)] 
 
[!INCLUDE [customize-work-tracking](../includes/get-started/customize-work-tracking.md)] 

## Integrate with other services 

Azure DevOps supports integration with Azure, GitHub, and many other services. As a member of the **Project Administrators** group, you can configure integration with many of these services. For more information, see the following articles. 

|Service integration |Resources |
|--------------------|----------|
| **Azure DevOps and GitHub** | [Azure DevOps and GitHub integration overview](../cross-service/github-integration.md) |
| **Azure Boards and GitHub** | [Azure Boards and GitHub integration](../boards/github/index.md) |
| **Microsoft Teams** | - [Azure Boards with Microsoft Teams](../boards/integrations/boards-teams.md) <br> - [Azure Repos with Microsoft Teams](../repos/integrations/repos-teams.md) <br> - [Azure Pipelines with Microsoft Teams](../pipelines/integrations/microsoft-teams.md) |
| **Slack** | - [Azure Boards with Slack](../boards/integrations/boards-slack.md) <br> - [Azure Repos with Slack](../repos/integrations/repos-slack.md) <br> - [Azure Pipelines with Slack](../pipelines/integrations/slack.md) |
| **Azure DevOps service hooks** | [Integrate with service hooks](../service-hooks/overview.md) |

[!INCLUDE [add-teams-to-scale](../includes/get-started/add-teams-to-scale.md)] 
 
## Related content

- [View and update project summary page](../organizations/projects/project-vision-status.md)
- [Get started managing your organization or project collection](manage-organization-collection.md)
- [About user, team, project, and organization-level settings](../organizations/settings/about-settings.md)


<!--- 
What to tell their users?
- advantage of setting up teams for repos and pipelines 
::: moniker range="azure-devops"  

> [!NOTE]  
> If the **Limit user visibility and collaboration to specific projects** preview feature is enabled for the organization, users added to the **Project-Scoped Users** group won't be able to access projects that they haven't been added to. For more information, see [Manage your organization, Limit  user visibility for projects and more](manage-organization-collection.md#project-scoped-user-group).

::: moniker-end  
-->
