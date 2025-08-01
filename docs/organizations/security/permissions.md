---
title: Permissions, security groups, and service accounts reference
titleSuffix: Azure DevOps
description: Reference guide of security groups, service accounts, and permissions for Azure DevOps
ms.subservice: azure-devops-security
ms.assetid: 169E817F-B297-4461-B359-27C78D4A8A7D
toc: show
ms.topic: reference
ms.author: chcomley
author: chcomley
monikerRange: '<= azure-devops'
ms.date: 11/12/2024
--- 

# Security groups, service accounts, and permissions reference

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]

This article provides a comprehensive reference for each built-in user, group, and permission.

For a quick reference to default assignments, see [Default permissions and access](permissions-access.md). For an overview of how permissions and security are managed, see [About permissions, access, and security groups](about-permissions.md), [About security roles](about-security-roles.md), and [About access levels](access-levels.md). 

For more information about adding users to a group or setting a specific permission that you can manage through the web portal, see the following resources:  

:::row:::
   :::column span="1":::
  **Users and groups**  
  ::: moniker range="azure-devops"
     - [Add users to the Project Administrators group](change-project-level-permissions.md)
     - [Add users to the Project Collection Administrators group](change-organization-collection-level-permissions.md)
     - [Add users to an organization](../accounts/add-organization-users.md)  
     - [Add users to a project or a team](add-users-team-project.md)  
     - [Add a team administrator](../settings/add-team-administrator.md)  
  ::: moniker-end
  ::: moniker range="< azure-devops"
     - [Add users to the Project Administrators group](change-project-level-permissions.md)
     - [Add users to the Project Collection Administrators group](change-organization-collection-level-permissions.md)
     - [Add a server-level administrator](/azure/devops/server/admin/add-administrator)  
     - [Add users to a project or team](add-users-team-project.md)  
     - [Add a team administrator](../settings/add-team-administrator.md)  
  ::: moniker-end
  **Wiki**
     - [README & Wiki](../../project/wiki/manage-readme-wiki-permissions.md)  
   :::column-end:::
   :::column span="1":::
  **DevOps**   
     - [Git branch](../../repos/git/branch-permissions.md)  
     - [Git repositories](../../repos/git/set-git-repository-permissions.md)  
     - [TFVC](../../repos/tfvc/set-tfvc-repository-permissions.md)  
     - [Build and release pipelines](../../pipelines/policies/permissions.md#pipeline-permissions)  
     - [Approvals and approvers](../../pipelines/release/approvals/index.md)  
     - [Task groups](../../pipelines/policies/permissions.md#task-group-permissions)   
     - [Variable groups](../../pipelines/policies/permissions.md#library-permissions)  
     - [Role-based resources](../../pipelines/policies/permissions.md)  
   :::column-end:::
   :::column span="1":::
  **Work tracking**  
     - [Area and iteration paths](set-permissions-access-work-tracking.md)  
     - [Queries and folders](../../boards/queries/set-query-permissions.md)  
     - [Plan permissions](set-permissions-access-work-tracking.md)  
     - [Customize process](set-permissions-access-work-tracking.md#process-permissions)  
  **Reporting**
  ::: moniker range="azure-devops"
     - [Dashboard permissions](../../report/dashboards/dashboard-permissions.md#set-permissions)  
     - [Analytics](../../report/powerbi/analytics-security.md)  
     - [Analytics views](../../report/powerbi/analytics-security.md)  
  ::: moniker-end
  ::: moniker range=" < azure-devops"
     - [Dashboard permissions](../../report/dashboards/dashboard-permissions.md#set-permissions)  
     - [Analytics](../../report/powerbi/analytics-security.md)  
     - [Analytics views](../../report/powerbi/analytics-security.md) 
     - [SQL Server Reports](/previous-versions/azure/devops/report/admin/grant-permissions-to-reports) 
  ::: moniker-end
   :::column-end:::
:::row-end:::
---

> [!NOTE]  
> The images shown in your web portal might differ from the images in this article due to system updates, but the basic functionality remains the same unless explicitly mentioned. 

## Service accounts

The system generates a few service accounts to support specific operations. The following table describes these user accounts, which get added at the organization or collection level. 

| User name | Description |  
| ----------| ----------- |  
| Agent Pool Service | Has permission to listen to the message queue for the specific pool to receive work. In most cases, you don't need to manage group members directly - the agent registration process handles it for you. When you register the agent, the service account you specify (typically Network Service) automatically gets added. Responsible for performing Azure Boards read/write operations and updating work items when GitHub objects change.   |  
| Azure Boards | Added when Azure Boards is [connected to GitHub](../../boards/github/connect-to-github.md). You shouldn't have to manage members of this group. Responsible for managing the link creation between GitHub and Azure Boards. |  
| PipelinesSDK | Added as needed to support the Pipelines policy service scope tokens. This user account is similar to the build service identities but supports locking down permissions separately. In practice, the tokens that involve this identity are granted read-only permissions to pipeline resources and the one-time ability to approve policy requests. This account should be treated in the same way that the build service identities are treated.   |  
| *ProjectName* Build Service | Has permissions to run build services for the project and is a legacy user used for XAML builds. It's automatically a member of the Security Service Group, which is used to store users who are granted permissions, but no other security group.  |  
| Project Collection Build Service | Has permissions to run build services for the collection. It's automatically a member of the Security Service Group, which is used to store users who are granted permissions, but no other security group. |  

<a name="groups"></a>

## Groups

You can grant permissions directly to an individual, or to a group.
Using groups makes things simpler and the system provides several built-in groups for that purpose.
These groups and the default permissions they're assigned get defined at different levels: server (on-premises deployment only), project collection, project, and specific objects. You can also create your own groups and grant them the specific set of permissions that are appropriate for certain roles in your organization.

::: moniker range="azure-devops"

[!INCLUDE [version-all](./includes/hidden-security-groups.md)]

::: moniker-end
<!---Team Foundation Administrators, Team Foundation Proxy Service Accounts, Team Foundation Service Accounts, Team Foundation Valid Users, Project Server Integration Service Accounts, SharePoint Web Application Services-->
::: moniker range="< azure-devops"

## Server-level groups 

When you install Azure DevOps Server, the system creates default groups that have [deployment-wide, server-level permissions](#server-permissions). You can't remove or delete the built-in server-level groups.

> [!div class="mx-imgBorder"]  
> ![Screenshot of Azure DevOps Security group dialog.](media/permissions/server-level-groups-azdo-2019-update1.png) 

You can't remove or delete the default server level groups. 

The full name of each of these groups is **[Team Foundation]\\{group name}**. So the full name of the server level administrators group is **[Team Foundation]\\Team Foundation Administrators**.
 
:::row:::
   :::column span="1":::
   **Group name**
   :::column-end:::
   :::column span="1":::
   **Permissions**
   :::column-end:::
   :::column span="2":::
   **Membership**
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Azure DevOps Service Accounts
   :::column-end:::
   :::column span="1":::
   Has service-level permissions for the server instance.
   :::column-end:::
   :::column span="2":::
   Contains the service account that was supplied during installation  

   This group should contain only service accounts
   and not user accounts or groups that contain user accounts.
   By default, this group is a member of **Team Foundation Administrators**.  

   To add an account to this group after you install Azure DevOps Server, use the TFSSecurity.exe utility in the **Tools** subfolder of your on-premises installation directory. Use the following command: `TFSSecurity /g+ "[TEAM FOUNDATION]\Team Foundation Service Accounts" n:domain\username /server:http(s)://azuredevopsservername`.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Azure DevOps Proxy Service Accounts
   :::column-end:::
   :::column span="1":::   
   Has service level permissions for Azure DevOps Server Proxy,
   and some service-level permissions.
   > [!NOTE]   
   > This account gets created when you [install the Azure DevOps proxy service](/azure/devops/server/install/install-proxy-setup-remote). 
   :::column-end:::
   :::column span="2":::   
   This group should contain only service accounts and not user accounts or groups
   that contain user accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Azure DevOps Valid Users
   :::column-end:::
   :::column span="1":::   
   Has permission to view server instance-level information.
   :::column-end:::
   :::column span="2":::   
   Contains all users known to exist in the server instance.
   You can't modify the membership of this group.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Team Foundation Administrators
   :::column-end:::
   :::column span="1":::   
   Has permissions to perform all server-level operations.
   :::column-end:::
   :::column span="2":::
   **Local Administrators** group (BUILTIN\Administrators)
   for any server that hosts Azure DevOPs/Team Foundation application services.  

   *Server* **\Team Foundation Service Accounts** group
   and the members of the **\Project Server Integration Service Accounts** group.  

   Limit this group to the fewest users who require full administrative control over server-level operations.

   > [!NOTE]   
   > If your deployment uses Reporting, consider [adding the members of this group](/azure/devops/server/admin/add-administrator) to the Content Managers groups in Reporting Services.
   :::column-end:::
:::row-end:::

::: moniker-end

## Collection-level groups

When you create an organization or project collection in Azure DevOps, the system creates collection-level groups that have [permissions in that collection](#collection-level). You can't remove or delete the built-in collection-level groups.

<!---Project Collection Administrators, Project Collection Build Administrators, Project Collection Build Service Accounts, Project Collection Proxy Service Accounts, Project Collection Service Accounts, Project Collection Test Service Accounts, Project Collection Valid Users, Security Service Group-->

::: moniker range="azure-devops"
> [!NOTE]   
> To enable the **Organizations Permissions Settings Page v2** preview page,see [Enable preview features](../../project/navigation/preview-features.md). The preview page provides a group settings page that the current page doesn't.
::: moniker-end  

#### [Preview page](#tab/preview-page)

::: moniker range="< azure-devops"

Preview page is not available for on-premises versions.

::: moniker-end

::: moniker range="azure-devops"

> [!div class="mx-imgBorder"]  
> ![Screenshot of Project collection groups, new user interface.](media/permissions/collection-admin-permissions-vsts-new.png)

::: moniker-end

#### [Current page](#tab/current-page)

> [!div class="mx-imgBorder"]  
> ![Screenshot of Project collection groups, on-premises versions.](media/permissions/collection-admin-permissions-vsts.png)

---

The full name of each of these groups is **[{collection name}]\\{group name}**. 
So the full name of the administrator group for the default collection is 
**[Default Collection]\\Project Collection Administrators**.

:::row:::
   :::column span="1":::
  **Group name**
   :::column-end:::
   :::column span="1":::
  **Permissions**
   :::column-end:::
   :::column span="2":::
  **Membership**
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
  Project Collection Administrators
   :::column-end:::
   :::column span="1":::
  Has permissions to perform all operations for the collection.
   :::column-end:::
   :::column span="2":::
   Contains the **Local Administrators** group (BUILTIN\Administrators)
   for the server where the application-tier services are installed.
   Contains the members of the *CollectionName*/**Service Accounts** group.
   Limit this group to the fewest users who require full administrative control over the collection.  
   ::: moniker range="< azure-devops-2022"
   > [!NOTE]
   > If your deployment uses Reporting Services, consider adding the members of this group to the [Team Foundation Content Managers groups in Reporting Services](/previous-versions/azure/devops/report/admin/grant-permissions-to-reports).
   ::: moniker-end
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Collection Build Administrators
   :::column-end:::
   :::column span="1":::
   Has permissions to administer build resources and permissions for the collection.
   :::column-end:::
   :::column span="2":::
   Limit this group to the fewest users who require full administrative control over build servers and services for this collection.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Collection Build Service Accounts
   :::column-end:::
   :::column span="1":::
   Has permissions to run build services for the collection.
   :::column-end:::
   :::column span="2":::
   Limit this group to service accounts and groups that contain only service accounts. This is a legacy group used for XAML builds. Use the Project Collection Build Service ({your organization}) user for managing permissions for current builds. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Collection Proxy Service Accounts
   :::column-end:::
   :::column span="1":::
   Has permissions to run the proxy service for the collection.
   :::column-end:::
   :::column span="2":::
   Limit this group to service accounts and groups that contain only service accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Collection Service Accounts
   :::column-end:::
   :::column span="1":::
   Has service level permissions for the collection and for Azure DevOps Server.
   :::column-end:::
   :::column span="2":::
   Contains the service account that was supplied during installation. This group should contain only service accounts and groups that contain only service accounts. By default, this group is a member of the Administrators group.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Collection Test Service Accounts
   :::column-end:::
   :::column span="1":::
   Has test service permissions for the collection.
   :::column-end:::
   :::column span="2":::
   Limit this group to service accounts and groups that contain only service accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Collection Valid Users
   :::column-end:::
   :::column span="1":::
   Has permissions to access team projects and view information in the collection.
   :::column-end:::
   :::column span="2":::
   Contains all users and groups added anywhere within the collection. You can't modify the membership of this group.
   :::column-end:::
:::row-end:::
::: moniker range="azure-devops"
:::row:::
   :::column span="1":::
   Project-Scoped Users <a id="project-scoped-user-group"></a>
   :::column-end:::
   :::column span="1":::
   Has limited access to view organization settings and projects other than those projects they are specifically added to. Also, people picker options are limited to those users and groups explicitly added to the project the user is connected to.
   :::column-end:::
   :::column span="2":::
   Add users to this group when you want to limit their visibility and access to those projects that you explicitly add them to. don't add users to this group if they are also added to the Project Collection Administrators group.  
   > [!NOTE]   
   > The **Project-Scoped Users** group becomes available with limited access when the organization-level preview feature, **Limit user visibility and collaboration to specific projects** is enabled. For more information including important security-related call-outs, see [Manage your organization, Limit  user visibility for projects and more](../../user-guide/manage-organization-collection.md#project-scoped-user-group).
   :::column-end:::
:::row-end:::
::: moniker-end
:::row:::
   :::column span="1":::
   Security Service Group
   :::column-end:::
   :::column span="1":::
   Used to store users with permissions, but not added to any other security group. 
   :::column-end:::
   :::column span="2":::
   Don't assign users to this group. If you're removing users from all security groups, check whether you need to remove them from this group.   
   :::column-end:::
:::row-end:::

   <!---
   Build Administrators
   Contributors
   Endpoint Administrators - cloud
   Project Administrators
   Project Valid Users
   Readers
   Release Administrators  
[team name]
-->
<a id="project-level-groups"></a>

## Project-level groups

For each project that you create, the system creates the followings project-level groups. These groups are assigned [project-level permissions](#team-project-level-permissions).

> [!NOTE]   
> To enable the preview page for the **Project Permissions Settings Page**, see [Enable preview features](../../project/navigation/preview-features.md).

#### [Preview page](#tab/preview-page)

::: moniker range="< azure-devops"

Preview page is not available for on-premises versions.

::: moniker-end

::: moniker range="azure-devops"

:::image type="content" source="media/permissions/project-level-groups-new.png" alt-text="Screenshot of Project-level groups and permissions, Azure DevOps preview version.":::

::: moniker-end

#### [Current page](#tab/current-page) 

:::image type="content" source="media/permissions/project-level-groups-current.png" alt-text="Screenshot of Project-level groups and permissions, Azure DevOps current.":::

---

> [!TIP]  
> The full name of each of these groups is **[{project name}]\\{group name}**. 
> For example, the contributors group for a project called "My Project" is 
> **[My Project]\\Contributors**.

:::row:::
   :::column span="1":::
  **Group name**
   :::column-end:::
   :::column span="1":::
  **Permissions**
   :::column-end:::
   :::column span="2":::
  **Membership**
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
  Build Administrators
   :::column-end:::
   :::column span="1":::
  Has permissions to administer build resources and build permissions for the project. Members can manage test environments, create test runs, and manage builds.
   :::column-end:::
   :::column span="2":::
   Assign to users who define and manage build pipelines.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Contributors
   :::column-end:::
   :::column span="1":::
   Has permissions to contribute fully to the project code base and work item tracking. The main permissions they don't have are permissions that manage or administer resources.
   :::column-end:::
   :::column span="2":::
   By default, the team group created when you create a project is added to this group, and any user you add to the team or project is a member of this group. In addition, any team you create for a project is added to this group.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Readers
   :::column-end:::
   :::column span="1":::
   Has permissions to view project information, the code base, work items, and other artifacts but not modify them.
   :::column-end:::
   :::column span="2":::
   Assign to members of your organization or collection who you want to provide view-only permissions to a project. These users can view backlogs, boards, dashboards, and more, but not add or edit anything.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Administrators<a id="project-administrator-group"></a>
   :::column-end:::
   :::column span="1":::
   Has permissions to administer all aspects of teams and project, although they can't create team projects.
   :::column-end:::
   :::column span="2":::
  Assign to users who require the following functions: Manage user permissions, create or edit teams, modify team settings, define area or iteration paths, or customize work item tracking. Members of the Project Administrators group have permissions to perform the following tasks: 
  - Add and remove users from project membership 
  - Add and remove custom security groups from a project 
  - Add and administer all project teams and team-related features  
  - Edit project level permission ACLs  
  - Edit [event subscriptions (email or SOAP)](#alerts) for teams or project-level events.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Project Valid Users
   :::column-end:::
   :::column span="1":::
   Has permissions to access and view project information.
   :::column-end:::
   :::column span="2":::
   Contains all users and groups added anywhere to the project. You can't modify the membership of this group.
   > [!NOTE]  
   > We recommend that you don't change the default permissions for this group. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   Release Administrators
   :::column-end:::
   :::column span="1":::
   Has permissions to manage all release operations.
   :::column-end:::
   :::column span="2":::
   Assign to users who define and manage release pipelines.
   > [!NOTE]   
   > The Release Administrator group gets created at the same time the first release pipeline is defined. It isn't created by default when the project is created. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   *TeamName* <a id="team-group"></a> 
   :::column-end:::
   :::column span="1":::
   Has permissions to contribute fully to the project code base and work item tracking.  
   :::column-end:::
   :::column span="2":::
   The default Team group is created when you create a project, and by default is added to the Contributors group for the project. Any new teams you create also have a group created for them and added to the Contributors group.

   Add members of the team to this group. To grant access to configure team settings, [add a team member to the team administrator role](../settings/add-team-administrator.md).
   :::column-end:::
:::row-end:::
   <!---
   Create and manage team alerts
   Create and manage team rooms
   Configure team backlogs
   Customize the board (Add columns, Swimlanes, Customize Cards, Definition of Done ...
   Manage team dashboards
   Select team area paths
   Select team sprints
   Set working days off
   Show bugs on backlogs and boards
-->

## Team administrator role

For each team that you add, you can assign one or more team members as administrators. The team admin role isn't a group with a set of defined permissions. Instead, the team admin role is tasked with managing  team assets. For more information, see [Manage teams and configure team tools](../settings/manage-teams.md). To add a user as a team administrator, see [Add a team administrator](../settings/add-team-administrator.md).

> [!NOTE]   
> Project Administrators can manage all team administrative areas for all teams. 

## Permissions

::: moniker range="azure-devops"
The system manages permissions at different levels&mdash;organization, project, object, and role-based permissions&mdash;and by default assigns them to one or more built-in groups. You can manage most permissions through the web portal. Manage more permissions with the [command line tool (CLI)](manage-tokens-namespaces.md).
::: moniker-end

::: moniker range="< azure-devops"
The system manages permissions at different levels&mdash;server, collection, project, object, and role-based permissions&mdash;and by default assigns them to one or more built-in groups. You can manage most permissions through the web portal. Manage more permissions with the [command line tool (CLI)](manage-tokens-namespaces.md).
::: moniker-end

In the following sections, the namespace permission is provided following the permission label that displays in the user interface. For example:   
   **Create tag definition**  
   `Tagging, Create`

For more information, see [Security namespace and permission reference](namespace-reference.md).
   <a id="server">  </a>
   <a id="server-permissions">  </a>
::: moniker range="< azure-devops"

## Server-level permissions 

Manage server-level permissions through the [Team Foundation Administration Console](/azure/devops/server/admin/add-administrator) or [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#permissions). Team Foundation Administrators are granted all server-level permissions. Other server-level groups have select permission assignments.

> [!div class="mx-imgBorder"]  
> ![Screenshot of Server-level permissions.](media/permissions/global-security-azdo-server-2019-update-1.png) 

:::row:::
   :::column span="2":::
   **Permission (UI)**  
   `Namespace permission`
   :::column-end:::
   :::column span="2":::
   **Description**
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
   <a id="administer-warehouse-permission"></a> Administer warehouse  

   `Warehouse, Administer`
   :::column-end:::
   :::column span="2":::
   Only valid for Azure DevOps Server 2020 and earlier versions that are configured to support SQL Server reports. Can process or change the settings for the data warehouse or SQL Server Analysis cube
   by using the [Warehouse Control Web Service](/previous-versions/azure/devops/report/admin/manage-reports-data-warehouse-cube).  

   More permissions might be required to fully process
   or [rebuild the data warehouse and Analysis cube](/previous-versions/azure/devops/report/admin/rebuild-data-warehouse-and-cube).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-team-project-collection-permission"></a> Create project collection  

   `CollectionManagement, CreateCollection`
   :::column-end:::
   :::column span="2":::
   Can create and administer collections.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-team-project-collection-permission"></a> Delete project collection  

   `CollectionManagement, DeleteCollection`
   :::column-end:::
   :::column span="2":::   
   Can delete a collection from the deployment.
   > [!NOTE]  
   > Deleting a collection doesn't delete the collection database from SQL Server.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-instance-level-information-permission"></a> 
   Edit instance-level information  

   `Server, GenericWrite`
   :::column-end:::
   :::column span="2":::
   
   Can edit server-level permissions for users and groups,
   and add or remove server level groups from the collection.

   > [!NOTE]   
   > **Edit instance-level information** includes the ability to perform these tasks defined in all collections defined for the instance:  
   > - Modify **Extensions** and **Analytics** settings
   > - Implicitly allows the user to modify version control permissions and repository settings
   > - Edit [event subscriptions](#alerts) or alerts for global notifications, project-level, and team-level events 
   > - Edit all project and team-level settings for projects defined in the collections  
   > - Create and modify global lists 
   >
   > To grant all these permissions at a command prompt, you must use the `tf.exe Permission` command to grant the `AdminConfiguration` and `AdminConnections` permissions in addition to `GENERIC_WRITE`.

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="make-requests-on-behalf-of-others-permission"></a> Make requests on behalf of others    

   `Server, Impersonate`
   :::column-end:::
   :::column span="2":::
   Can perform operations on behalf of other users or services. Only assign to service accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="trigger-events-permission"></a> Trigger events  

   `Server, TriggerEvent`
   :::column-end:::
   :::column span="2":::
   Can trigger server-level alert events.
   Only assign to service accounts and members of the Azure DevOps or Team Foundation Administrators group.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="use-full-web-access-features-permission"></a> Use full Web Access features
   :::column-end:::
   :::column span="2":::
   
   Can use all on-premises Web portal features. This permission is deprecated with Azure DevOps Server 2019 and later versions.

   > [!NOTE]   
   > If the **Use full Web Access** features permission is set to **Deny**, the user only sees those features permitted for the **Stakeholder** group (see [Change access levels](change-access-levels.md)). A Deny overrides any implicit Allow, even for accounts that are members of administrative groups such as Team Foundation Administrators.

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-instance-level-information-permission"></a> View instance-level information  

   `Server, GenericRead`
   :::column-end:::
   :::column span="2":::
   Can view server level group membership and the permissions of those users.
   > [!NOTE]   
   > The **View instance-level information** permission is also assigned to the Azure DevOps Valid Users group.
   :::column-end:::
:::row-end:::

::: moniker-end
   <a id="collection">  </a>
   <a id="collection-level"> </a>

::: moniker range="azure-devops"

## Organization-level permissions

Manage organization-level permissions through the [web portal admin context](../../project/navigation/go-to-service-page.md#collection-admin-context) or with the [az devops security group](add-manage-security-groups.md) commands. Project Collection Administrators are granted all organization-level permissions. Other organization-level groups have select permission assignments.

> [!NOTE]   
> To enable the preview page for the **Project Permissions Settings Page**, see [Enable preview features](../../project/navigation/preview-features.md).

#### [Preview page](#tab/preview-page)

> [!div class="mx-imgBorder"]  
> ![Screenshot of Organization-level permissions and groups, Azure DevOps Services.](media/permissions/collection-level-permissions-new.png)   

[!INCLUDE [note-collection-level-permissions](includes/note-collection-level-permissions.md)]

:::row:::
   :::column span="2":::
   #### Permission (UI)<br/>
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  #### Description 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   #### General
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="alter-trace-settings"></a> Alter trace settings  
  `Collection, DIAGNOSTIC_TRACE`
   :::column-end:::
   :::column span="2":::
   
   Can [change the trace settings](/previous-versions/ms400797%28v%3dvs.80%29) for gathering more detailed diagnostic information about Azure DevOps Web services.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-new-team-projects"></a> Create new projects  
   (formerly Create new team projects)  
  `Collection, CREATE_PROJECTS`
   :::column-end:::
   :::column span="2":::
   
   Can [add a project](../projects/create-project.md) to an organization or project collection. More permissions may be required depending on your on-premises deployment. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-team-project"></a> Delete team project  
  `Project, DELETE`
   :::column-end:::
   :::column span="2":::
   
   Can [delete a project](../projects/delete-project.md). Deleting a project deletes all data that is associated with the project. You can't undo the deletion of a project except by restoring the collection to a point before the project was deleted.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-collection-level-information"></a> Edit instance-level information  
  `Collection, GENERIC_WRITE`
   :::column-end:::
   :::column span="2":::
   Can set organization and project-level settings.

   > [!NOTE]   
   > **Edit instance-level information** includes the ability to perform these tasks for all projects defined in an organization or collection:  
   > - Modify organization **Overview** settings and **Extensions**
   > - Modify version control permissions and repository settings
   > - Edit [event subscriptions](#alerts) or alerts for global notifications, project-level, and team-level events 
   > - Edit all project and team-level settings for projects defined in the collections
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-collection-level-information"></a> View instance-level information  
  `Collection, GENERIC_READ` 
   :::column-end:::
   :::column span="2":::
   Can view organization-level permissions for a user or group. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Service Account
   :::column-end:::
:::row-end:::
:::row:::  
   :::column span="2":::
   <a id="make-requests-on-behalf-of-others"></a> Make requests on behalf of others  
  `Server, Impersonate`    
   :::column-end:::
   :::column span="2":::
   Can perform operations on behalf of other users or services.
   Assign this permission only to service accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="trigger-events"></a> Trigger events  
  `Collection, TRIGGER_EVENT`
  `Server, TRIGGER_EVENT`
   :::column-end:::
   :::column span="2":::
   Can trigger project alert events within the collection. Assign only to service accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-system-synchronization-information"></a> View system synchronization information 
  `Collection, SYNCHRONIZE_READ`      
   :::column-end:::
   :::column span="2":::
   Can call the synchronization application programming interfaces. Assign only to service accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Boards  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="administer-process-permissions"></a> Administer process permissions  
  `Process, AdministerProcessPermissions`
   :::column-end:::
   :::column span="2":::
   Can modify permissions for customizing work tracking by creating and customizing [inherited processes](../settings/work/inheritance-process-model.md). 
   - [Customize a project](../settings/work/customize-process.md)
   - [Add and manage processes](../settings/work/manage-process.md)
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-process"></a> Create process  
  `Process, Create`
   :::column-end:::
   :::column span="2":::
   Can [create an inherited process](../settings/work/manage-process.md) used to customize work tracking and Azure Boards. Users  granted Basic and Stakeholder access are granted this permission by default. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-field"></a> Delete field from organization  
  `Collection, DELETE_FIELD`
   :::column-end:::
   :::column span="2":::
   Can [delete a custom field that was added to a process](../settings/work/customize-process-field.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-process"></a> Delete process  
  `Process, Delete`
   :::column-end:::
   :::column span="2":::
   Can [delete an inherited process](../settings/work/manage-process.md) used to customize work tracking and Azure Boards. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-process"></a> Edit process  
  `Process, Edit`
   :::column-end:::
   :::column span="2":::
   Can edit a [custom inherited process](../settings/work/customize-process.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Repos  
   Applies only to Team Foundation version control (TFVC)
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="administer-shelved-changes"></a>Administer shelved changes  
  `VersionControlPrivileges, AdminWorkspaces`
   :::column-end:::
   :::column span="2":::
   Can delete [shelvesets created by other users](../../repos/tfvc/suspend-your-work-manage-your-shelvesets.md).  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="administer-workspaces"></a> Administer workspaces  
  `Workspaces, Administer`
   :::column-end:::
   :::column span="2":::
   Can [create and delete workspaces for other users](../../repos/tfvc/create-work-workspaces.md).  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-a-workspace"></a> Create a workspace  
  `VersionControlPrivileges, CreateWorkspace`
   :::column-end:::
   :::column span="2":::
   Can create a version control workspace. The **Create a workspace** permission is granted to all users as part of their membership within the Project Collection Valid Users group.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Pipelines  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="administer-build-resource-permissions"></a> Administer build resource permissions  
  `BuildAdministration, AdministerBuildResourcePermissions`
   :::column-end:::
   :::column span="2":::
   Can modify permissions for build resources at the organization or project collection-level, which includes: 
   - [Set retention policies](../../pipelines/policies/retention.md)
   - [Set resource limits for pipelines](../../pipelines/licensing/concurrent-jobs.md)
   - [Add and manage agent pools](../../pipelines/agents/pools-queues.md)
   - [Add and manage deployment pools](../../pipelines/release/deployment-groups/index.md)
   
   > [!NOTE]   
   > In addition to this permission, Azure DevOps provides role-based permissions governing the [security of agent pools](../../pipelines/policies/permissions.md). Other, [object-level settings](#build-object-level) will override those set at the organization or project-level. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-build-resources"></a> Manage build resources  
  `BuildAdministration, ManageBuildResources`
   :::column-end:::
   :::column span="2":::
   Can manage build computers, build agents, and build controllers.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-build-resources"></a> Manage pipeline policies  
  `BuildAdministration, ManagePipelinePolicies`
   :::column-end:::
   :::column span="2":::
   Can manage pipeline settings set through **Organization settings, Pipelines, Settings**.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="use-build-resources"></a> Use build resources  
  `BuildAdministration, UseBuildResources`
   :::column-end:::
   :::column span="2":::
   Can reserve and allocate build agents. Assign only to service accounts for build services.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-build-resources"></a> View build resources  
  `BuildAdministration, ViewBuildResources`
   :::column-end:::
   :::column span="2":::
   Can view, but not use, build controllers and build agents that are configured for an organization or project collection.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Test Plans
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-test-controllers"></a> Manage test controllers  
  `Collection, MANAGE_TEST_CONTROLLERS`
   :::column-end:::
   :::column span="2":::
   Can register and deregister test controllers.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   <a id="audit-streams-permissions"></a> 
   
   #### Auditing
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2"::: 
   <a id="delete-audit-streams-permission"></a> Delete audit streams  
  `AuditLog, Delete_Streams`
   :::column-end:::
   :::column span="2":::
   Can delete an audit stream. Audit streams are in preview. For more information, see [Create audit streaming](../audit/auditing-streaming.md). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-audit-streams-permission"></a> Manage audit streams  
  `AuditLog, Manage_Streams`
   :::column-end:::
   :::column span="2":::
   Can add an audit stream. Audit streams are in preview. For more information, see [Create audit streaming](../audit/auditing-streaming.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-audit-log-permission"></a> View audit log  
  `AuditLog, Read`
   :::column-end:::
   :::column span="2":::
   Can view and export audit logs. Audit logs are in preview. For more information, see [Access, export, and filter audit logs](../audit/azure-devops-auditing.md). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Policies  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-enterprise-policies-permission"></a> Manage enterprise policies  
  `Collection, MANAGE_ENTERPRISE_POLICIES`
   :::column-end:::
   :::column span="2":::
   Can enable and disable application connection policies as described in [Change application connection policies](../accounts/change-application-access-policies.md).
   :::column-end:::
:::row-end:::

#### [Current page](#tab/current-page) 

> [!div class="mx-imgBorder"]
> ![Screenshot of Collection-level permissions dialog, Azure DevOps Services current page and on-premises.](media/permissions/collection-level-permissions.png)

[!INCLUDE [note-collection-level-permissions](includes/note-collection-level-permissions.md)]

[!INCLUDE [collection-level-permissions-reference-table](includes/collection-level-permissions-reference-table-cloud.md)]

---

::: moniker-end

::: moniker range="< azure-devops"

## Collection-level permissions

Manage collection-level permissions through the [web portal admin context](../../project/navigation/go-to-service-page.md#collection-admin-context) or the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#collection-level-permissions). Project Collection Administrators are granted all collection-level permissions. Other collection-level groups have select permission assignments.

The permissions available for Azure DevOps Server 2019 and later versions vary depending on the process model configured for the collection. For an overview of process models, see [Customize work tracking](../../reference/customize-work.md). 

:::row:::
   :::column span="2":::
  **Inherited process model**
   :::column-end:::
   :::column span="2":::
  **On-premises XML process model**
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
  > [!div class="mx-imgBorder"]  
  > ![Screenshot of Collection level permissions, on-premises, Inherited process model.](media/permissions/collection-level-permissions.png)
   :::column-end:::
   :::column span="2":::
  > [!div class="mx-imgBorder"]  
  > ![Screenshot of Collection level permissions, on-premises, On-premises XML process model.](media/permissions/collection-level-permissions-2020-xml-on-premises-1.png)
   :::column-end:::
:::row-end:::

[!INCLUDE [note-collection-level-permissions](includes/note-collection-level-permissions.md)]

[!INCLUDE [collection-level-permissions-reference-table](includes/collection-level-permissions-reference-table.md)]

::: moniker-end

   <a name="project-level"> </a>
   <a name="project_test">  </a>
   <a name="team-project-level-permissions">  </a>
   <a name="project-level-permissions"> </a>

## Project-level permissions

> [!IMPORTANT]
> To access project-level resources, the **View project-level information** permission must be set to **Allow**.  This permission gates all other project-level permissions.

::: moniker range="azure-devops" 

Manage project-level permissions through the [web portal admin context](change-project-level-permissions.md) or with the [az devops security group](add-manage-security-groups.md) commands. Project Administrators are granted all project-level permissions. Other project-level groups have select permission assignments.
 
> [!NOTE]   
> To enable the **Project Permissions Settings Page** preview page, see [Enable preview features](../../project/navigation/preview-features.md).

::: moniker-end

::: moniker range="< azure-devops"

Manage project-level permissions through the [web portal admin context](change-project-level-permissions.md). Project Administrators are granted all project-level permissions. Other project-level groups have select permission assignments.

::: moniker-end

#### [Preview page](#tab/preview-page)

::: moniker range="< azure-devops"

Preview page is not available for on-premises versions.

::: moniker-end

::: moniker range="azure-devops"

> [!div class="mx-imgBorder"]
> ![Screenshot of Project-level permissions dialog, Azure DevOps Services preview page.](media/permissions/project-permissions-contributors.png)

[!INCLUDE [note-project-level-permissions](includes/note-project-level-permissions.md)]

:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end::: 
:::row:::
   :::column span="4":::
   #### General  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-team-project-permission"></a> Delete team project  

   `Project, DELETE`
   :::column-end:::
   :::column span="2":::
   Can [delete a project](../projects/delete-project.md) from an organization or project collection.
   > [!NOTE]   
   > Even if you set this permission to **Deny**, users granted permission at the project level can likely delete the project for which they have permission. To ensure that a user can't delete a project, make sure you set the **Delete team project** at the project-level to **Deny** as well. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-team-project-level-information-permission"></a> Edit project-level information  

   `Project, MANAGE_PROPERTIES`
   :::column-end:::
   :::column span="2":::
   Can perform the following tasks for the selected project defined in an organization or collection. 
   - [Edit the project description](../projects/project-vision-status.md)
   - [Modify project services visibility](../settings/set-services.md).
   > [!NOTE]
   > The permission to add or remove project-level security groups and add and manage project-level group membership is assigned to all members of the **Project Administrators** group. It isn't controlled by a permissions surfaced within the user interface.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-team-project-property-permission"></a>  
   Manage project properties  

   `Project, MANAGE_SYSTEM_PROPERTIES`
   :::column-end:::
   :::column span="2":::
   Can provide or edit metadata for a project. For example, a user can provide high-level information about the contents of a project. Changing metadata is supported through the [Set project properties REST API](/rest/api/azure/devops/core/projects/set%20project%20properties). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="rename-team-project-permission"></a> Rename project  

   `Project, RENAME`
   :::column-end:::
   :::column span="2":::
   Can [change the name of the project](../projects/rename-project.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="suppress-notifications-for-work-item-updates-permission"></a> Suppress notifications for work item updates  

   `Project, SUPPRESS_NOTIFICATIONS`
   :::column-end:::
   :::column span="2":::
   Users with this permission can update work items without generating notifications. This feature is useful when performing migrations of bulk updates by tools and want to skip generating notifications.  

   Consider granting this permission to service accounts or users with the **Bypass rules on work item updates** permission. You can set the `suppressNotifications` parameter to `true` when updating working via [Work Items - update REST API](/rest/api/azure/devops/wit/work-items/update).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="update-project-visibility"></a> Update project visibility  

   `Project, UPDATE_VISIBILITY`
   :::column-end:::
   :::column span="2":::
   Can [change the project visibility](../projects/make-project-public.md) from private to public or public to private. Applies to Azure DevOps Services only.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-team-project-level-information-permission"></a> View project-level information 

   `Project, GENERIC_READ`
   :::column-end:::
   :::column span="2":::
   Can view project-level information, including security information group membership and permissions. If you set this permission to **Deny** for a user, they can't view the project or sign in to the project.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   #### Boards  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="bypass-rules-permission"></a> Bypass rules on work item updates  <br />
   `Project, BYPASS_RULES`
   :::column-end:::
   :::column span="2":::
   
   Users with this permission can save a work item that ignores rules, such as [copy, constraint, or conditional rules](../settings/work/rule-reference.md), defined for the work item type. Useful scenarios are migrations where you don't want to update the by/date fields on import or when you want to skip the validation of a work item.  <br />
   Rules can be bypassed in one of two ways. The first is through the [Work Items - update REST API](/rest/api/azure/devops/wit/work-items/update) and setting the `bypassRules` parameter to `true`. The second is through the client object model, by initializing in bypass rules mode (initialize `WorkItemStore` with `WorkItemStoreFlags.BypassRules`).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="change-process-team-project-permission"></a> Change process of project  <br />
   `Project, CHANGE_PROCESS`
   :::column-end:::
   :::column span="2":::
   
   When combined with the 'Edit project-level information' permission, allows users to change the Inheritance process for a project. For more information, see [Create and manage inherited processes](../settings/work/manage-process.md).  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-tag-definition-permission"></a> Create tag definition  <br />
   `Tagging, Create`
   :::column-end:::
   :::column span="2":::
   
   [Can add tags to a work item](../../boards/queries/add-tags-to-work-items.md). By default, all members of the Contributors group have this permission. Also, you can set more tagging permissions through security management tools. For more information, see [Security namespace and permission reference, Tagging](namespace-reference.md). 

   > [!NOTE] 
   > All users granted Stakeholder access for a private project can only add existing tags. Even if the **Create tag definition** permission is set to **Allow**, stakeholders can't add tags. This is part of the Stakeholder access settings. Azure DevOps Services users granted Stakeholder access for a public project are granted this permission by default. For more information, see [Stakeholder access quick reference](stakeholder-access.md).  
  > Although the **Create tag definition**  permission appears
  > in the security settings at the project-level,
  > tagging permissions are actually collection level permissions that are scoped
  > at the project level when they appear in the user interface.
  > To scope tagging permissions to a single project when using the **TFSSecurity** command,
  > you must provide the GUID for the project as part of the command syntax.
  > Otherwise, your change applies to the entire collection.
  > Keep this in mind when changing or setting these permissions.
  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-work-items-in-this-project-permission"></a> 
   Delete and restore work items or Delete work items in this project. <br />
   `Project, WORK_ITEM_DELETE`
   :::column-end:::
   :::column span="2":::
   
   Can [mark work items in the project as deleted](../../boards/backlogs/remove-delete-work-items.md). Azure DevOps Services users granted Stakeholder access for a public project are granted this permission by default.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="move-work-items-out-of-this-project-permission"></a> Move work items out of this project  <br />
   `Project, WORK_ITEM_MOVE`
   :::column-end:::
   :::column span="2":::
   
   Can [move a work item from one project to another project](../../boards/backlogs/remove-delete-work-items.md) within the collection.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="permanently-delete-work-items-in-this-project-permission"></a> Permanently delete work items in this project  <br />
   `Project, WORK_ITEM_PERMANENTLY_DELETE`
   :::column-end:::
   :::column span="2":::
   
   Can [permanently delete work items](../../boards/backlogs/remove-delete-work-items.md) from this project. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Analytics
   In addition to the `AnalyticsView` namespace permissions listed in this section, you can set [object-level permissions on each view](#analytics). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-shared-analytic-views-permission"></a> Delete shared Analytics view  <br />
   `AnalyticsViews, Delete`  
   :::column-end:::
   :::column span="2":::
   
   Can delete [Analytics views](../../report/powerbi/analytics-views-manage.md)
   under the Shared area. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-shared-analytic-views-permission"></a> Edit shared Analytics view  <br />
   `AnalyticsViews, Edit`
   :::column-end:::
   :::column span="2":::
   
   Can create and modify [shared Analytics views](../../report/powerbi/analytics-views-manage.md).   
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-analytics-permission"></a> View analytics  <br />
   `AnalyticsViews, Read`
   :::column-end:::
   :::column span="2":::
   Can access data available from the [Analytics service](../../report/powerbi/what-is-analytics.md). For more information, see [Permissions required to access the Analytics service](../../report/powerbi/analytics-security.md).   
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   
   #### Test Plans 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-test-runs-permission"></a> Create test runs  <br />
   `Project, PUBLISH_TEST_RESULTS`
   :::column-end:::
   :::column span="2":::
   
   Can add and remove test results and add or modify test runs. For more information, see [Control how long to keep test results](../../test/how-long-to-keep-test-results.md) and [Run manual tests](../../test/run-manual-tests.md). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-test-runs-permission"></a> Delete test runs  <br />
   `Project, DELETE_TEST_RESULTS`
   :::column-end:::
   :::column span="2":::
   Can [delete a test run](../../boards/backlogs/delete-test-artifacts.md). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-test-configurations-permission"></a> Manage test configurations  <br />
   `Project, MANAGE_TEST_CONFIGURATIONS`
   :::column-end:::
   :::column span="2":::
   Can create and delete [test configurations](../../test/test-different-configurations.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-test-environments-permission"></a> Manage test environments  <br />
   `Project, MANAGE_TEST_ENVIRONMENTS`
   :::column-end:::
   :::column span="2":::
   Can create and delete [test environments](../../test/test-different-configurations.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-test-runs-permission"></a> View test runs  <br />
   `Project, VIEW_TEST_RESULTS`
   :::column-end:::
   :::column span="2":::
   Can view test plans under the project area path.
   :::column-end:::
:::row-end:::

::: moniker-end

#### [Current page](#tab/current-page)

> [!div class="mx-imgBorder"]
> ![Screenshot of Project-level permissions dialog, Azure DevOps Services current page.](media/permissions/project-level-permissions.png)

[!INCLUDE [project-level-permissions-reference-table](includes/project-level-permissions-reference-table-cloud.md)]

Manage project-level permissions through the [web portal admin context](change-project-level-permissions.md) or the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#collection-level-permissions). Project Administrators are granted all project-level permissions. Other project-level groups have select permission assignments.

> [!NOTE]
> Several permissions granted to members of the [Project Administrators group](#project-administrator-group) don't surface within the user interface.  

> [!div class="mx-imgBorder"]  
> ![Screenshot of Project-level permissions, on-premises, Inherited process model.](media/permissions/project-level-permissions.png)

:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="bypass-rules-permission"></a>  
   Bypass rules on work item updates  <br />
   `Project, BYPASS_RULES`
   :::column-end:::
   :::column span="2":::
   Users with this permission can save a work item that ignores rules, such as [copy, constraint, or conditional rules](../settings/work/rule-reference.md), defined for the work item type. Useful for migrations where you don't want to update the `by` or `date` fields on import, or when you want to skip the validation of a work item.  
   Rules can be bypassed in one of two ways. The first is through the [Work Items - update REST API](/rest/api/azure/devops/wit/work-items/update) and setting the `bypassRules` parameter to `true`. The second is through the client object model, by initializing in bypass rules mode (initialize `WorkItemStore` with `WorkItemStoreFlags.BypassRules`).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="change-process-team-project-permission"></a>  
   Change process of project  <br />
   `Project, CHANGE_PROCESS`
   :::column-end:::
   :::column span="2":::
   When combined with the 'Edit project-level information' permission, allows users to change the Inheritance process for a project. For more information, see [Create and manage inherited processes](../settings/work/manage-process.md).  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-tag-definition-permission"></a>  
   Create tag definition <br />
   `Tagging, Create`
   :::column-end:::
   :::column span="2":::
   [Can add tags to a work item](../../boards/queries/add-tags-to-work-items.md). By default, all members of the Contributors group have this permission. Also, you can set more tagging permissions through security management tools. For more information, see [Security namespace and permission reference, Tagging](namespace-reference.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   > [!NOTE]   
   > All users granted Stakeholder access can only add existing tags. Even if the **Create tag definition** permission is set to **Allow**, stakeholders can't add tags. This is part of the Stakeholder access settings. For more information, see [Stakeholder access quick reference](stakeholder-access.md).
   > Although the **Create tag definition**  permission appears
   > in the security settings at the project-level,
   > tagging permissions are actually collection level permissions that are scoped
   > at the project level when they appear in the user interface.
   > To scope tagging permissions to a single project when using the **TFSSecurity** command,
   > you must provide the GUID for the project as part of the command syntax.
   > Otherwise, your change will apply to the entire collection.
   > Keep this in mind when changing or setting these permissions.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="create-test-runs-permission"></a>  
   Create test runs  <br />
   `Project, PUBLISH_TEST_RESULTS`
   :::column-end:::
   :::column span="2":::
   Can add and remove test results and add or modify test runs. For more information, see [Control how long to keep test results](../../test/how-long-to-keep-test-results.md) and [Run manual tests](../../test/run-manual-tests.md). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-work-items-in-this-project-permission"></a> 
   Delete and restore work items or Delete work items in this project  <br />
   `Project, WORK_ITEM_DELETE`
   :::column-end:::
   :::column span="2":::
   Can [mark work items in the project as deleted](../../boards/backlogs/remove-delete-work-items.md). The Contributors group has **Delete and restore work items** at the project-level set to **Allow** by default.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-shared-analytic-views-permission"></a>  
   Delete shared Analytics view  <br />
   `AnalyticsViews, Delete`
   :::column-end:::
   :::column span="2":::
   Can delete [Analytics views](../../report/powerbi/analytics-views-manage.md) under the Shared area.   
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-team-project-permission"></a>  
   Delete project  <br />
   `Project, DELETE`
   :::column-end:::
   :::column span="2":::
   Can [delete a project](../projects/delete-project.md) from an organization or project collection.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-test-runs-permission"></a>  
   Delete test runs  <br />
   `Project, DELETE_TEST_RESULTS`
   :::column-end:::
   :::column span="2":::
   Can delete a test run.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-team-project-level-information-permission"></a>  
   Edit project-level information <br />
   `Project, MANAGE_PROPERTIES`
   :::column-end:::
   :::column span="2":::
   Can perform the following tasks for the selected project defined in an organization or collection. 
   - [Edit the project description](../projects/project-vision-status.md)
   - [Modify project services visibility](../settings/set-services.md).
   > [!NOTE]
   > The permission to add or remove project-level security groups and add and manage project-level group membership is assigned to all members of the **Project Administrators** group. It isn't controlled by a permissions surfaced within the user interface.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-shared-analytic-views-permission"></a>  
   Edit shared Analytics view  <br />
   `AnalyticsViews, Edit` 
   :::column-end:::
   :::column span="2":::
   Can create and modify [shared Analytics views](../../report/powerbi/analytics-views-manage.md).  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-team-project-property-permission"></a>  
   Manage project properties  <br />
   `Project, MANAGE_SYSTEM_PROPERTIES`
   :::column-end:::
   :::column span="2":::
   Can provide or edit metadata for a project. For example, a user can provide high-level information about the contents of a project. Changing metadata is supported through the [Set project properties REST API](/rest/api/azure/devops/core/projects/set%20project%20properties). 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-test-configurations-permission"></a>  
   Manage test configurations  <br />
   `Project, MANAGE_TEST_CONFIGURATIONS`
   :::column-end:::
   :::column span="2":::
   Can create and delete [test configurations](../../test/test-different-configurations.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-test-environments-permission"></a>  
   Manage test environments  <br />
   `Project, MANAGE_TEST_ENVIRONMENTS`
   :::column-end:::
   :::column span="2":::
   Can create and delete [test environments](../../test/test-different-configurations.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="move-work-items-out-of-this-project-permission"></a>  
   Move work items out of this project  <br />
   `Project, WORK_ITEM_MOVE`
   :::column-end:::
   :::column span="2":::
   Can [move a work item from one project to another project](../../boards/backlogs/remove-delete-work-items.md) within the collection. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="permanently-delete-work-items-in-this-project-permission"></a>  
   Permanently delete work items in this project <br />
   `Project, WORK_ITEM_PERMANENTLY_DELETE`
   :::column-end:::
   :::column span="2":::
   Can [permanently delete work items](../../boards/backlogs/remove-delete-work-items.md) from this project. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="rename-team-project-permission"></a>  
   Rename project <br />
   `Project, RENAME`
   :::column-end:::
   :::column span="2":::
   Can [change the name of the project](../projects/rename-project.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="suppress-notifications-for-work-item-updates-permission"></a>  
   Suppress notifications for work item updates <br />
   `Project, SUPPRESS_NOTIFICATIONS`
   :::column-end:::
   :::column span="2":::
   Users with this permission can update work items without generating notifications. Useful for performing migrations of bulk updates by tools and skipping generating notifications.  <br />
   Consider granting this permission to service accounts or users with the **Bypass rules on work item updates** permission. You can set the `suppressNotifications` parameter to `true` when updating working via [Work Items - update REST API](/rest/api/azure/devops/wit/work-items/update).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="update-project-visibility"></a>  
   Update project visibility  <br />
   `Project, UPDATE_VISIBILITY`
   :::column-end:::
   :::column span="2":::
   Can [change the project visibility](../projects/make-project-public.md) from private to public or public to private. Applies to Azure DevOps Services only.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-analytics-permission"></a>  
   View analytics <br />
   `AnalyticsViews, Read` 
   :::column-end:::
   :::column span="2":::
   Can access data available from the [Analytics service](../../report/powerbi/what-is-analytics.md). For more information, see [Permissions required to access the Analytics service](../../report/powerbi/analytics-security.md).  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-team-project-level-information-permission"></a>  
   View project-level information  <br />
   `Project, GENERIC_READ`
   :::column-end:::
   :::column span="2":::
   Can view project level group membership and permissions.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-test-runs-permission"></a>  
   View test runs   <br />
   `Project, VIEW_TEST_RESULTS`
   :::column-end:::
   :::column span="2":::
   Can view test plans under the project area path. 
   :::column-end:::
:::row-end:::

---

## Analytics views (object-level)  

With shared Analytics views, you can grant specific permissions to view, edit, or delete a view that you create. Manage the security of Analytics views from the [web portal](../../report/powerbi/analytics-security.md).  

::: moniker range="azure-devops"
:::image type="content" source="media/permissions/set-analytics-view-shared-permissions.png" alt-text="Screenshot of Shared Analytics view security dialog, change permissions for a user.":::
::: Moniker-end
::: moniker range=" < azure-devops"
:::image type="content" source="media/permissions/analytics-view-permissions.png" alt-text="Screenshot of Manage Shared Analytics view security dialog, change permissions for a user, Azure DevOps Server.":::
::: Moniker-end

The following permissions are defined for each shared Analytics view. All valid users are automatically granted all permissions to manage Analytics views. Consider granting select permissions to specific shared views to other team members or security group that you create. For more information, see [What are Analytics views?](../../report/powerbi/what-are-analytics-views.md) and [Security namespace and permission reference](namespace-reference.md#analytic-views-namespace).   
:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
   <a id="av-delete-permission"></a> Delete shared Analytics views

   `AnalyticsViews, Delete`  
   :::column-end:::
   :::column span="2":::
   Can delete the shared Analytics view.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="av-edit-permission"></a> Edit shared Analytics views

   `AnalyticsViews, Edit`  
   :::column-end:::
   :::column span="2":::  
   Can change the parameters of the shared Analytics view.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="av-view-permission"></a> View shared Analytics views 

   `AnalyticsViews, Read`  
   :::column-end:::
   :::column span="2":::
   Can view and use the shared Analytics view from Power BI desktop. 
   :::column-end:::
:::row-end:::

## Dashboards (object-level)  

::: moniker range="azure-devops"
Permissions for team and project dashboards can be set individually. The default permissions for a team can be set for a project. Manage the security of dashboards from the web portal. More namespace permissions are supported as defined in [Security namespace and permission reference](namespace-reference.md#dashboard-previleges-namespace).   

### Project dashboard permissions

> [!div class="mx-imgBorder"]  
> ![Screenshot of Project dashboard permissions dialog.](../../report/dashboards/media/set-permissions/add-user-project-permissions.png)  

By default, the creator of the project dashboard is the dashboard owner and granted all permissions for that dashboard. 

|**Permission**<br />`Namespace permission`  | **Description** |
|-----------| ----------- |
|Delete dashboard<br />`DashboardsPrivileges, Delete`   | Can delete the project dashboard. |
|Edit dashboard<br />`DashboardsPrivileges, Edit`  |  Can add widgets to and change the layout of the project dashboard. |
|Manage Permissions<br />`DashboardsPrivileges, ManagePermissions`  | Can manage permissions for the project dashboard. |

::: moniker-end

::: moniker range="< azure-devops"
   Permissions for team dashboards can be set individually. The default permissions for a team can be set for a project. Manage the security of dashboards from the web portal.
::: moniker-end

### Team dashboard default permissions

> [!div class="mx-imgBorder"]  
> ![Screenshot of Team dashboard permissions dialog.](../../report/dashboards/media/set-permissions/project-setting-permissions.png) 

By default, team administrators are granted all permissions for their team dashboards, including managing default and individual dashboard permissions. 

|**Permission**<br />`Namespace permission`  | **Description** |
|-----------| ----------- |
|Create dashboards<br />`DashboardsPrivileges, Create`  | Can create a team dashboard. |
|Delete dashboards<br />`DashboardsPrivileges, Delete` | Can delete a team dashboard. |
|Edit dashboards<br />`DashboardsPrivileges, Edit` |  Can add widgets to and change the layout of a team dashboard. |

### Individual team dashboard permissions

> [!div class="mx-imgBorder"]  
> ![Screenshot of individual team dashboard permissions dialog.](../../report/dashboards/media/set-permissions/team-analytics-dashboard-permissions.png) 

   Team administrators can change the permissions for individual team dashboards by changing the following two permissions.  

|**Permission**<br />`Namespace permission`  | **Description** |
|-----------| ----------- |
|Delete dashboard<br />`DashboardsPrivileges, Delete`  | Can delete the specific team dashboard. |
|Edit dashboard<br />`DashboardsPrivileges, Edit`  |  Can add widgets to and change the layout of the specific team dashboard. |

   <a name="build"></a>
   <a name="build-object-level"></a>

## Pipeline or Build (object-level)

Manage pipeline permissions [for each pipeline defined in the web portal](../../pipelines/policies/permissions.md#pipeline-permissions) or using the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#build-permissions). Project Administrators are granted all pipeline permissions and Build Administrators are assigned most of these permissions. You can set pipeline permissions for all pipelines defined for a project or for each pipeline definition.

::: moniker range="azure-devops"
:::image type="content" source="media/permissions/pipeline-object-level-permissions-cloud.png" alt-text="Screenshot of pipeline object-level security dialog, cloud."::: 
::: Moniker-end

::: moniker range=" < azure-devops"

> [!div class="mx-imgBorder"]  
> ![Screenshot of Pipeline object-level permissions dialog.](media/permissions/edit-build-pipeline-object-level-permissions-s163.png)

::: moniker-end

Permissions in Build follow a hierarchical model. Defaults for all the permissions can be set at the project level and can be overridden on an individual build definition.

To set the permissions at project level for all build definitions in a project, choose **Security** from the action bar on the main page of Builds hub.

To set or override the permissions for a specific build definition, choose **Security** from the context menu of the build definition.

You can define the following permissions in Build at both levels.

:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
   <a id="administer-build-permissions-permission"></a> 
   Administer build permissions  
   `Build, AdministerBuildPermissions`
   :::column-end:::
   :::column span="2":::
   Can administer the build permissions for other users.
   :::column-end:::
:::row-end:::
::: moniker range="azure-devops"
:::row:::
   :::column span="2":::
   <a id="create-build-pipeline"></a> 
   Create build pipeline
   `Build,  CreateBuildPipeline`
   :::column-end:::
   :::column span="2":::
   Can create pipeline lines and edit those pipelines.
   :::column-end:::
:::row-end:::
::: moniker-end
:::row:::
   :::column span="2":::
   <a id="create-build-pipeline-permission"></a>Create build pipeline
   `Build, CreateBuildDefinition`
   :::column-end:::
   :::column span="2":::
   Can create pipelines.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-build-definition-permission"></a> Delete build definition  
   `Build, DeleteBuildDefinition`
   :::column-end:::
   :::column span="2":::
   Can delete build definitions for this project.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-builds-permission"></a> Delete builds  
   `Build, DeleteBuilds`
   :::column-end:::
   :::column span="2":::
   Can delete a completed build. Builds that are deleted are [retained](../../pipelines/policies/retention.md) in the **Deleted** tab for some time before they're destroyed.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="destroy-builds-permission"></a> Destroy builds  
   `Build, DestroyBuilds`
   :::column-end:::
   :::column span="2":::
   Can permanently delete a completed build.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-build-pipeline-permission"></a>
   <a id="edit-build-definition-permission"></a> Edit build pipeline<br />Edit build definition   
   `Build, EditBuildDefinition`
   :::column-end:::
   :::column span="2":::
 
   **Edit build pipeline**: Can save any changes to a build pipeline, including configuration variables, triggers, repositories, and retention policy. Available with Azure DevOps Services, Azure DevOps Server 2019 1.1, and later versions. Replaces Edit build definition. Cannot create new pipelines.
   **Edit build definition*:* Can create and modify build definitions for this project.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="4":::
   > [!NOTE]   
   > To control permissions for specific build definitions, turn off **inheritance**.
   >
   > When inheritance is turned _on_, the build definition respects the build permissions defined at the project level or a group or user. For example, a custom Build Managers group has permissions set to manually queue a build for project Fabrikam. Any build definition with inheritance for project Fabrikam allows a member of the Build Managers group to manually queue a build.
   >
   > When inheritance is turned _off_, you can set permissions so only Project Administrators can manually queue a build for a specific build definition.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-build-quality-permission"></a> Edit build quality  
   `Build, EditBuildQuality`
   :::column-end:::
   :::column span="2":::
   Can add information about the quality of the build through Team Explorer or the web portal.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-build-qualities-permission"></a> Manage build qualities  
   `Build, ManageBuildQualities`
   :::column-end:::
   :::column span="2":::
   Can add or remove build qualities. *Only applies to XAML builds*.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="manage-build-queue-permission"></a> Manage build queue  
   `Build, ManageBuildQueue`
   :::column-end:::
   :::column span="2":::
   Can cancel, re-prioritize, or postpone queued builds. *Only applies to XAML builds*.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="override-check-in-validation-by-build-permission"></a> Override check-in validation by build  
   `Build, OverrideBuildCheckInValidation`
   :::column-end:::
   :::column span="2":::
   Can commit a TFVC changeset that affects a gated build definition
   without triggering the system to shelve and build their changes first.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="queue-builds-permission"></a> Queue builds  
   `Build, QueueBuilds`
   :::column-end:::
   :::column span="2":::
   Can put a build in the queue through the interface for Team Foundation Build or at a command prompt.
   They can also stop the builds that they have queued.
   :::column-end:::
:::row-end:::
::: moniker range="azure-devops"
:::row:::
   :::column span="2":::
   <a id="edit-pipeline-queue-configuration-permission"></a> Edit queue build configuration
   `Build, EditPipelineQueueConfigurationPermission`
   :::column-end:::
   :::column span="2":::
   Can specify values for free-text parameters (e.g., of type `object` or `array`) and pipeline variables when queueing new builds.
   :::column-end:::
:::row-end:::
::: moniker-end
:::row:::
   :::column span="2":::
   <a id="retain-indefinitely-permission"></a> Retain indefinitely  
   `Build, RetainIndefinitely`  
   :::column-end:::
   :::column span="2":::
   Can toggle the retain flag on a build to indefinitely. This feature marks a build so that the system doesn't automatically delete it based on any applicable retention policy.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="stop-builds-permission"></a> Stop builds  
   `Build, StopBuilds`  
   :::column-end:::
   :::column span="2":::
   Can stop any build that is in progress, including builds queued and started by another user.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="update-build-information-permission"></a> Update build information  
   `Build, UpdateBuildInformation`  
   :::column-end:::
   :::column span="2":::
   Can add build information nodes to the system, and can also add information about the quality of a build.
   Assign only to service accounts.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-build-definition-permission"></a> View build definition  
   `Build, ViewBuildDefinition`  
   :::column-end:::
   :::column span="2":::
   Can view the build definitions created for the project.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="view-builds-permission"></a> View builds  
   `Build, ViewBuilds`  
   :::column-end:::
   :::column span="2":::
   Can view the queued and completed builds for this project.
   :::column-end:::
:::row-end:::

> [!NOTE]
> - Turn **Inheritance Off** for a build definition when you want to control permissions for specific build definitions.
>     - When **inheritance is On**, the build definition respects the build permissions defined at the project level or a group or user. For example, a custom Build Managers group has permissions set to manually queue a build for project Fabrikam. Any build definition with inheritance On for project Fabrikam would allow a member of the Build Managers group the ability to manually queue a build.
>     - However, by turning **Inheritance Off** for project Fabrikam, you can set permissions that only allow Project Administrators to manually queue a build for a specific build definition. This would then allow me to set permissions for that build definition specifically.
> - Assign the **Override check-in validation by build** permission only to service accounts for build services and to build administrators who are responsible for the quality of the code. Applies to [TFVC gated check-in builds](../../pipelines/build/triggers.md). This doesn't apply to PR builds. For more information, see [Check in to a folder that is controlled by a gated check-in build process](../../repos/tfvc/check-folder-controlled-by-gated-check-build-process.md).

## Git repository (object-level)

   <!---
   Contribute 
   Create Branch 
   Create Repository 
   Create Tag 
   Delete Repository 
   Edit Policies 
   Exempt From Policy Enforcement 
   Force Push (Rewrite History and Delete Branches) 
   Manage Notes 
   Manage Permissions 
   Read 
   Remove Others' Locks 
   Rename Repository 
-->

Manage the security of each [Git repository](../../repos/git/set-git-repository-permissions.md) or [branch](../../repos/git/branch-permissions.md) from the web portal, the [TF command line tool](../../repos/tfvc/git-permission-command.md), or using the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#git-repo-permissions). Project Administrators are granted most of these permissions (which appear only for a project that configured with a Git repository). You can manage these permissions for all Git repositories, or for a specific Git repo.

::: moniker range="azure-devops" 

> [!div class="mx-imgBorder"]  
> ![Screenshot of Git repository permissions dialog.](media/permissions/git-repo-permissions-vsts.png)

::: moniker-end 

> [!NOTE]  
> Set permissions across all Git repositories by making changes to the top-level **Git repositories** entry. Individual repositories inherit permissions from  the top-level **Git repositories** entry. Branches inherit permissions from assignments made at the repository level. By default, the project level Readers groups only have Read permissions.

To manage Git repo and branch permissions, see [Set branch permissions](../../repos/git/branch-permissions.md).

:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
   <a id="git-bypass-policies-when-completing-pull-requests"></a> Bypass policies when completing pull requests  
   `GitRepositories, PullRequestBypassPolicy`  
   :::column-end:::
   :::column span="2":::
   Can opt in to override branch policies by checking **Override branch policies and enable merge** when completing a PR.
   > [!NOTE]   
   > Bypass policies when completing pull requests and **Bypass policies when pushing** replace **Exempt From Policy Enforcement**.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-bypass-policies-when-pushing"></a> Bypass policies when pushing
   :::column-end:::
   :::column span="2":::
   Can push to a branch that has branch policies enabled. When a user with this permission makes a push that would override branch policy, the push automatically bypasses branch policy with no opt-in step or warning.
   > [!NOTE]   
   > Bypass policies when completing pull requests and **Bypass policies when pushing** replace **Exempt From Policy Enforcement**.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-contribute-permission"></a> Contribute  
   `GitRepositories, GenericContribute`  
   :::column-end:::
   :::column span="2":::
   
   At the repository level, can push their changes to existing branches in the repository and can complete pull requests. Users who lack this permission but who have the **Create branch** permission might push changes to new branches. Doesn't override restrictions in place from [branch policies](../../repos/git/branch-policies.md).  
   
   At the branch level, can push their changes to the branch and lock the branch. Locking a branch blocks any new commits from others and prevents other users from changing the existing commit history.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-contribute-to-pull-requests-permission"></a> Contribute to pull requests  
   `GitRepositories, PullRequestContribute`  
   :::column-end:::
   :::column span="2":::
   Can create, comment on, and vote on pull requests.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-create-branch-permission"></a> Create branch  
   `GitRepositories, CreateBranch`  
   :::column-end:::
   :::column span="2":::
   Can create and publish branches in the repository. 
   Lack of this permission doesn't limit users from creating branches in their local repository; it merely prevents them from publishing local branches to the server.  
   
   > [!NOTE]  
   > When you create a new branch on the server, you have Contribute, Edit Policies, Force Push, Manage Permissions, and Remove Others' Locks permissions for that branch by default. This means that you can add new commits to the repo via your branch.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-create-repository-permission"></a> Create repository  
   `GitRepositories, CreateRepository`  
   :::column-end:::
   :::column span="2":::
   Can create new repositories. This permission is only available from the Security dialog for the top-level **Git repositories** object. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-create-tag-permission"></a> Create tag  
   `GitRepositories, CreateTag`  
   :::column-end:::
   :::column span="2":::
   Can push tags to the repository.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-delete-repository-permission"></a> Delete repository 
   `GitRepositories, DeleteRepository`  
   :::column-end:::
   :::column span="2":::
   Can delete the repository. At the top-level **Git repositories** level, can delete any repository.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-edit-policies-permission"></a> Edit policies  
   `GitRepositories, EditPolicies`  
   :::column-end:::
   :::column span="2":::
   Can edit policies for the repository and its branches.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-exempt-from-policy-permission"></a> Exempt From policy enforcement  
   `GitRepositories, PolicyExempt`  
   :::column-end:::
   :::column span="2":::
   Applies to TFS 2018 Update 2. Can bypass branch policies and perform the following two actions:  
  - Override branch policies and complete PRs that don't satisfy branch policy
  - Push directly to branches that have branch policies set
   > [!NOTE]   
   > In Azure DevOps it is replaced with the following two permissions: **Bypass policies when completing pull requests** and **Bypass policies when pushing**.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-force-push-permission"></a> Force push (rewrite history, delete branches and tags)  
   `GitRepositories, ForcePush`  
   :::column-end:::
   :::column span="2":::
   Can force an update to a branch, delete a branch, and modify the commit history of a branch. Can delete tags and notes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-note-management-permission"></a> Manage notes  
   `GitRepositories, ManageNote`  
   :::column-end:::
   :::column span="2":::
   Can push and edit Git notes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-create-repository-permission"></a> Manage permissions  
   `GitRepositories, ManagePermissions`  
   :::column-end:::
   :::column span="2":::
   Can set permissions for the repository.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-read-permission"></a> Read 
   `GitRepositories, GenericRead`  
   :::column-end:::
   :::column span="2":::
   Can clone, fetch, pull, and explore the contents of the repository.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-remove-others-locks-permission"></a> Remove others' locks  
   `GitRepositories, RemoveOthersLocks`  
   :::column-end:::
   :::column span="2":::
   Can remove [branch locks](../../repos/git/lock-branches.md) set by other users. Locking a branch blocks any new commits from being added to the branch by others and prevents other users from changing the existing commit history. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="git-rename-repository-permission"></a> Rename repository  
   `GitRepositories, RenameRepository`  
   :::column-end:::
   :::column span="2":::
   Can change the name of the repository. When set at the top-level **Git repositories** entry, can change the name of any repository.
   :::column-end:::
:::row-end:::

   <a id="tfvc">  </a>

## TFVC (object-level)

Manage the security of each TFVC branch from the [web portal](../../repos/tfvc/set-tfvc-repository-permissions.md) or using the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#tfvc-permissions). Project Administrators are granted most of these permissions, which appear only for a project that was configured to use Team Foundation Version Control as a source control system. In version control permissions, explicit deny takes precedence over administrator group permissions.

These permissions appear only for a project setup to use Team Foundation Version Control as the source control system.

> [!div class="mx-imgBorder"]  
> ![Screenshot of TFVC permissions dialog.](media/permissions/tfvc-repo-permissions-vsts.png)

In version control permissions, explicit **Deny** takes precedence over administrator group permissions.

:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
   Administer labels  
   `VersionControlItems, LabelOther`  
   :::column-end:::
   :::column span="2":::
   Can edit or delete labels created by another user.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Check in  
   `VersionControlItems, Checkin`  
   :::column-end:::
   :::column span="2":::
   Can check in items and revise any committed changeset comments.
   Pending changes are committed at check-in.*

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::   
   Check in other users' changes  
   `VersionControlItems, CheckinOther`  
   :::column-end:::
   :::column span="2":::
   Can check in changes that were made by other users.
   Pending changes are committed at check-in. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Pend a change in a server workspace  
   `VersionControlItems, PendChange`  
   :::column-end:::
   :::column span="2":::
   Can check out and make a pending change to items in a folder. 
   Examples of pending changes include adding, editing, renaming, deleting,
   undeleting, branching, and merging a file.
   Pending changes must be checked in,
   so users also must have the Check-in permission
   to share their changes with the team.*
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::   
   Label   
   `VersionControlItems, Label`  
   :::column-end:::
   :::column span="2":::
   Can label items. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::   
   <a id="lock-permission"></a>Lock  
   `VersionControlItems, Lock`  
   :::column-end:::
   :::column span="2":::
   Can lock and unlock folders or files. A folder or file tracked can be locked or unlocked to deny or restore a user's privileges. Privileges include checking out an item for edit into a different workspace or checking in Pending Changes to an item from a different workspace. For more information, see [Lock command](../../repos/tfvc/lock-command.md).
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Manage branch   
   `VersionControlItems, ManageBranch`  
   :::column-end:::
   :::column span="2":::
   Can convert any folder under that path into a branch,
   and also take the following actions on a branch:
   edit its properties, reparent it, and convert it to a folder.
   Users who have this permission can branch this branch
   only if they also have the Merge permission for the target path.
   Users can't create branches from a branch
   for which they don't have the Manage Branch permission.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Manage permissions  
   `VersionControlItems, AdminProjectRights`  
   :::column-end:::
   :::column span="2":::
   Can manage other users' permissions for folders and files in version control.*
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="merge-permission"></a> 
   Merge  
   `VersionControlItems, AdminProjectRights`  
   :::column-end:::
   :::column span="2":::
   Can merge changes into this path.*
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Read  
   `VersionControlItems, Read`   
   :::column-end:::
   :::column span="2":::
   Can read the contents of a file or folder.
   If a user has Read permissions for a folder,
   the user can see the contents of the folder and the properties of the files in it,
   even if the user doesn't have permission to open the files. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Revise other users' changes  
   `VersionControlItems, ReviseOther`  
   :::column-end:::
   :::column span="2":::
   Can edit the comments on checked-in files, even if another user checked in the file.*
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Undo other users' changes  
   `VersionControlItems, UndoOther`  
   :::column-end:::
   :::column span="2":::
   Can undo a pending change made by another user.*
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   Unlock other users' changes  
   `VersionControlItems, UnlockOther`  
   :::column-end:::
   :::column span="2":::
   Can unlock files locked by other users.*
   :::column-end:::
:::row-end:::

`*` Consider adding this permission to any manually added users or groups that are responsible for supervising or monitoring the project and that might or must change the comments on checked-in files, even if another user checked in the file.

## Area path (object-level) 

Area path permissions manage access to branches of the area hierarchy and to the work items in those areas. Manage the security of each area path from the [web portal](../../organizations/security/set-permissions-access-work-tracking.md) or using the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#area). Area permissions manage access to create and manage area paths as well as create and modify work items defined under area paths.

Members of the Project Administrators group are automatically granted permissions to manage area paths for a project. Consider granting team administrators or team leads permissions to create, edit, or delete area nodes.

> [!NOTE]  
> Multiple teams can contribute to a project.
> When that's the case, you can set up teams that are associated with an area.
> Permissions for the team's work items are assigned by assigning permissions to the area.
> There are other [team settings](../settings/manage-teams.md)
> that configure the team's agile planning tools.

> [!div class="mx-imgBorder"]  
> ![Screenshot of area path permissions dialog.](media/permissions/area-path-permissions-vsts.png)  

:::row:::
   :::column span="1":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="1":::
   <a id="area-create-child-nodes-permission"></a> Create child nodes  
   `CSS, CREATE_CHILDREN`  
   :::column-end:::
   :::column span="2":::
   Can create area nodes.
   Users who have both this permission and the **Edit this node** permission
   can move or reorder any child area nodes. 
   
   Consider adding this permission to any manually added users or groups that might need to delete, add, or rename area nodes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="area-delete-this-node-permission"></a> Delete this node  
   `CSS, CREATE_CHILDREN`  
   :::column-end:::
   :::column span="2":::
   
   Users who have both this permission and the **Edit this node** permission for another node
   can delete area nodes and reclassify existing work items from the deleted node. 
   If the deleted node has child nodes, those nodes are also deleted.
   
   Consider adding this permission to any manually added users or groups that might need to delete, add, or rename area nodes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="area-edit-this-node-permission"></a> Edit this node  
   `CSS, CREATE_CHILDREN`  
   :::column-end:::
   :::column span="2":::
   Can set permissions for this node and rename area nodes. 
   
   Consider adding this permission to any manually added users or groups that might need to delete, add, or rename area nodes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="area-edit-work-items-in-this-node-permission"></a> Edit work items in this node  
   `CSS, WORK_ITEM_WRITE`  
   :::column-end:::
   :::column span="2":::
   Can edit work items in this area node.
   
   Consider adding this permission to any manually added users or groups that might need to edit work items under the area node.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="area-manage-test-plans-permission"></a> Manage test plans  
   `CSS, MANAGE_TEST_PLANS`  
   :::column-end:::
   :::column span="2":::
   Can modify test plan properties such as build and test settings.
   
   Consider adding this permission to any manually added users or groups that might need to manage test plans or test suites under this area node.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="area-manage-test-suites-permission"></a> Manage test suites  
   `CSS, MANAGE_TEST_SUITES`  
   :::column-end:::
   :::column span="2":::
   Can create and delete test suites,
   add, and remove test cases from test suites,
   change test configurations associated with test suites,
   and modify suite hierarchy (move a test suite).
   
   Consider adding this permission to any manually added users or groups that might need to manage test plans or test suites under this area node.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="area-view-permissions-for-this-node-permission"></a> View permissions for this node 
   :::column-end:::
   :::column span="2":::
   Can view the security settings for an area path node.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="area-view-work-items-in-this-node-permission"></a> View work items in this node 
   
   `CSS, GENERIC_READ`  
   :::column-end:::
   :::column span="2":::
   Can view, but not change, work items in this area node.
   > [!NOTE]   
   > If you set the **View work items in this node** to **Deny**, the user can't see any work items in this area node. A **Deny** overrides any implicit allow, even for users that are members of an administrative groups.
   :::column-end:::
:::row-end:::

<a name="iteration-path-permissions"></a>

## Iteration path (object-level) 

Iteration path permissions manage access to create and manage iteration paths, also referred to as sprints.

Manage the security of each iteration path from the [web portal](../../organizations/security/set-permissions-access-work-tracking.md) or using the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#iteration-permissions). 

Members of the Project Administrators group are automatically granted these permissions for each iteration defined for a project. Consider granting team administrators, scrum masters, or team leads permissions to create, edit, or delete iteration nodes.  

> [!div class="mx-imgBorder"]  
> ![Screenshot of Iteration Path permissions dialog.](media/permissions/iteration-path-permissions-vsts.png)

:::row:::
   :::column span="1":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="1":::
   <a id="iteration-create-child-nodes-permission"></a> Create child nodes  
   `Iteration, CREATE_CHILDREN`  
   :::column-end:::
   :::column span="2":::
   Can create iteration nodes.
   Users who have both this permission and the **Edit this node** permission
   can move or reorder any child iteration nodes.

   Consider adding this permission to any manually added users or groups that might need to delete, add, or rename iteration nodes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="iteration-delete-this-node-permission"></a> Delete this node  
   `Iteration, DELETE`  
   :::column-end:::
   :::column span="2":::
   Users who have both this permission and the **Edit this node** permission for another node
   can delete iteration nodes and reclassify existing work items from the deleted node.
   If the deleted node has child nodes, those nodes are also deleted.
   
   Consider adding this permission to any manually added users or groups that might need to delete, add, or rename iteration nodes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="iteration-edit-this-node-permission"></a> Edit this node  
   `Iteration, GENERIC_WRITE`  
   :::column-end:::
   :::column span="2":::
   Can set permissions for this node and rename iteration nodes.
   
   Consider adding this permission to any manually added users or groups that might need to delete, add, or rename iteration nodes.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="iteration-view-permissions-for-this-node-permission"></a> View permissions for this node  
   `Iteration, GENERIC_READ`  
   :::column-end:::
   :::column span="2":::
   Can view the security settings for this node.
   > [!NOTE]   
   > Members of the Project Collection Valid Users, Project Valid Users, or any user or group that has **View collection-level information** or **View project-level information** can view permissions of any iteration node.
   :::column-end:::
:::row-end:::

<a id="query">  </a>

## Work item query and query folder (object-level)

Manage query and query folder permissions through the [web portal](../../boards/queries/set-query-permissions.md). Project Administrators are granted all of these permissions. Contributors are granted Read permissions only.

> [!div class="mx-imgBorder"]  
> ![Screenshot of Query folder permissions dialog.](media/permissions/query-folder-permissions-vsts.png)

Consider granting the **Contribute** permissions to users or groups that require the ability to create and share work item queries for the project. For more information, see [Set permissions on queries](../../boards/queries/set-query-permissions.md).

> [!NOTE]   
> To create query charts [you need Basic access](change-access-levels.md).

:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
   <a id="workitemqueryfolders-contribute-permission"></a> Contribute  
   `WorkItemQueryFolders, Contribute`  
   :::column-end:::
   :::column span="2":::
   Can view and modify the query folder or save queries within the folder. 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="workitemqueryfolders-delete-permission"></a> Delete  
   `WorkItemQueryFolders, Delete`  
   :::column-end:::
   :::column span="2":::
   Can delete a query or query folder and its contents.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="workitemqueryfolders-manage-permissions-permission"></a> Manage permissions  
   `WorkItemQueryFolders, ManagePermissions`  
   :::column-end:::
   :::column span="2":::
   Can manage the permissions for this query or query folder.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="workitemqueryfolders-read-permission"></a> Read  
   `WorkItemQueryFolders, Read`  
   :::column-end:::
   :::column span="2"::: 
   Can view and use the query or the queries in a folder,
   but can't modify the query or query folder contents.
   :::column-end:::
:::row-end:::

<a id="plan-permissions">  </a>

## Delivery Plans (object-level)   

Manage plan permissions through the [web portal](set-permissions-access-work-tracking.md#plan-permissions). Manage permissions for each plan through its Security dialog. Project Administrators are granted all permissions to create, edit, and manage plans. Valid users are granted View (read-only) permissions. 

:::row:::
   :::column span="1":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="1":::
   <a id="delete-plan-permission"></a> Delete  
   `Plan, Delete`  
   :::column-end:::
   :::column span="2":::
   Can delete the selected plan.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="edit-plan-permission"></a> Edit  
   `Plan, Edit`  
   :::column-end:::
   :::column span="2":::
   Can edit the configuration and settings defined for the selected plan.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="manage-plan-permission"></a> Manage  
   `Plan, Manage`  
   :::column-end:::
   :::column span="2":::
   Can manage the permissions for the selected plan.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="view-plan-permission"></a> View  
   `Plan, View`  
   :::column-end:::
   :::column span="2":::
   Can view the lists of plans, open, and interact with a plan, but can't modify the plan configuration or settings.
   :::column-end:::
:::row-end:::

## Process (object-level)   

You can manage the permissions for each inherited process that you create through the [web portal](set-permissions-access-work-tracking.md#process-permissions). Manage permissions for each process through its Security dialog. Project Collection Administrators are granted all permissions to create, edit, and manage processes. Valid users are granted View (read-only) permissions. 

:::row:::
   :::column span="2":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
  ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="2":::
   <a id="admin-process-permission"></a> Administer process permissions  
   `Process, AdministerProcessPermissions`  
   :::column-end:::
   :::column span="2":::
   Can set or change the permissions for an inherited process.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="delete-process-permission"></a> Delete process  
   `Process, Delete`  
   :::column-end:::
   :::column span="2":::
   Can delete the inherited process.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="2":::
   <a id="edit-process-permission"></a> Edit process  
   `Process, Edit`  
   :::column-end:::
   :::column span="2":::
   Can create an inherited process from a system process, or copy or modify an inherited process.  
   :::column-end:::
:::row-end:::

## Work item tags

::: moniker range="azure-devops"
You can manage tagging permissions using [az devops security permission](manage-tokens-namespaces.md) or the [TFSSecurity](/azure/devops/server/command-line/tfssecurity-cmd#tagging-permissions) command-line tools. Contributors can add tags to work items and use them to quickly filter a backlog, board, or query results view.
::: moniker-end
::: moniker range="< azure-devops"
You can manage tagging permissions using the [TFSSecurity command-line tool](/azure/devops/server/command-line/tfssecurity-cmd#tagging-permissions). Contributors can add tags to work items and use them to quickly filter a backlog, board, or query results view.
   ::: moniker-end
:::row:::
   :::column span="1":::
   ### Permission (UI)   
   `Namespace permission`  
   :::column-end:::
   :::column span="2":::
   ### Description 
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="1":::
   <a id="create-tag-definition-permission"></a> Create tag definition  
   `Tagging, Create`  
   :::column-end:::
   :::column span="2":::
   
   [Can create new tags and apply them to work items.](../../boards/queries/add-tags-to-work-items.md)
   Users without this permission can only select from the existing set of tags for the project.

   By default, Contributors are assigned the **Create tag definition** permission. Although the **Create tag definition** permission appears in the security settings at the project-level, tagging permissions are actually collection-level permissions that are scoped at the project level when they appear in the user interface. To scope tagging permissions to a single project when you're using a command-line tool, you must provide the GUID for the project as part of the command syntax. Otherwise, your change applies to the entire collection. Keep this in mind when changing or setting these permissions.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="delete-tag-definition-permission"></a> Delete tag definition  
   `Tagging, Delete`  
   :::column-end:::
   :::column span="2":::
   Can remove a tag from the list of available tags for that project.
   
   This permission doesn't appear in the UI. You can only set it by using a command-line tool. There's also no UI to explicitly delete a tag. Instead, when a tag has not been in use for three days, the system automatically deletes it.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="enumerate-tag-definition-permission"></a> Enumerate tag definition  
   `Tagging, Enumerate`  
   :::column-end:::
   :::column span="2":::   
   Can view a list of tags available for the work item within the project.
   Users without this permission don't have a list of available tags
   from which to choose in the work item form or in the query editor.
 
   This permission doesn't appear in the UI. It can only be set by using a command-line tool. The **View project-level information** implicitly allows users to view existing tags.
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="update-tag-definition-permission"></a> Update tag definition  
   `Tagging, Update`  
   :::column-end:::
   :::column span="2":::
   Can rename a tag by using the REST API.
   
   This permission doesn't appear in the UI. It can only be set by using a command-line tool. 
   :::column-end:::
:::row-end:::

<a id="release_management">  </a>
<a id="release-management">  </a>

## Release (object-level) 

Manage permissions [for each release defined in the web portal](../../pipelines/policies/permissions.md#pipeline-permissions). Project Administrators and Release Administrators are granted all release management permissions. These permissions work in a hierarchical model at the project level, for a specific release pipeline, or for a specific environment in a release pipeline. Within this hierarchy, permissions can be inherited from the parent or overridden.

:::image type="content" source="media/permissions/release-object-level-permissions.png" alt-text="Screenshot showing Releases object-level permissions.":::

> [!NOTE]   
> The project-level Release Administrator's group gets created when you define your first release pipeline. 

In addition, you can assign approvers to specific steps within a release pipeline to ensure that the applications being deployed meet quality standards.

The following permissions are defined in Release Management. The scope column explains whether the permission can be set at the project, release pipeline, or environment level.

:::row:::
   :::column span="1":::
   **Permission**
   :::column-end:::
   :::column span="2":::
   **Description**
   :::column-end:::
   :::column span="1":::
   **Scopes**
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="1":::
   <a id="admin-release-permission"></a> Administer release permissions
   :::column-end:::
   :::column span="2":::
   
   Can change any of the other permissions listed here.

   :::column-end:::
   :::column span="1":::
   
   Project, Release pipeline, Environment

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="create-releases-permission"></a> Create releases
   :::column-end:::
   :::column span="2":::
   
   Can create new releases.

   :::column-end:::
   :::column span="1":::
   
   Project, Release pipeline

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="delete-release-pipeline-permission"></a> Delete release pipeline
   :::column-end:::
   :::column span="2":::
   
   Can delete release pipelines.

   :::column-end:::
   :::column span="1":::
   
   Project, Release pipeline

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="delete-release-environment-permission"></a> Delete release environment
   :::column-end:::
   :::column span="2":::
   
   Can delete environments in release pipelines.

   :::column-end:::
   :::column span="1":::
   
   Project, Release pipeline, Environment

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="delete-releases-permission"></a> Delete releases
   :::column-end:::
   :::column span="2":::
   
   Can delete releases for a pipeline.  

   :::column-end:::
   :::column span="1":::
   
   Project, Release pipeline

   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="edit-release-permission"></a> Edit release pipeline
   :::column-end:::
   :::column span="2":::
   Can add and edit a release pipeline, including configuration variables, triggers, artifacts, and retention policy as well as configuration within an environment of the release pipeline. To make changes to a specific environment in a release pipeline, the user also needs **Edit release environment** permission. 
   :::column-end:::
   :::column span="1":::
   Project, Release pipeline 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="edit-release-environment-permission"></a> Edit release environment
   :::column-end:::
   :::column span="2":::
   Can edit environments in release pipelines. To save the changes to the release pipeline, the user also needs **Edit release pipeline** permission. This permission also controls whether a user can edit the configuration inside the environment of a specific release instance. The user also needs **Manage releases** permission to save the modified release.
   :::column-end:::
   :::column span="1":::
   Project, Release pipeline, Environment  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="manage-deployments-permission"></a> Manage deployments
   :::column-end:::
   :::column span="2":::  
  Can initiate a direct deployment of a release to an environment. This permission is only for direct deployments that are manually initiated by selecting the **Deploy** action in a release. If the condition on an environment is set to any type of automatic deployment, the system automatically initiates deployment without checking the permission of the user that created the release.  
   :::column-end:::
   :::column span="1":::
   Project, Release pipeline, Environment
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="manage-release-environment-permission"></a> Manage release approvers
   :::column-end:::
   :::column span="2":::
   Can add or edit approvers for environments in release pipelines. This permission also controls whether a user can edit the approvers inside the environment of a specific release instance.  
   :::column-end:::
   :::column span="1":::
   Project, Release pipeline, Environment
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="manage-releases-permission"></a> Manage releases
   :::column-end:::
   :::column span="2":::
   Can edit a release configuration, such as stages, approvers, and variables. To edit the configuration of a specific environment in a release instance, the user also needs **Edit release environment** permission.  
   :::column-end:::
   :::column span="1":::
   Project, Release pipeline
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="view-release-environment-permission"></a> View release pipeline
   :::column-end:::
   :::column span="2":::
   Can view release pipelines. 
   :::column-end:::
   :::column span="1":::
   Project, Release pipeline 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="view-releases-permission"></a> View releases
   :::column-end:::
   :::column span="2":::
   Can view releases belonging to release pipelines.  
   :::column-end:::
   :::column span="1":::
   Project, Release pipeline 
   :::column-end:::
:::row-end:::

Default values for all of these permissions are set for team project collections and project groups. For example,
**Project Collection Administrators**, **Project Administrators**, and
**Release Administrators** are given all of the above permissions by
   default. **Contributors** are given all permissions except
**Administer release permissions**. **Readers**, by default,
   are denied all permissions except **View release pipeline** and
**View releases**.

<a id="task-group">  </a>

## Task group (Build and Release) permissions

Manage permissions [for task groups from the **Build and Release** hub](../../pipelines/policies/permissions.md#pipeline-permissions) of the web portal. Project, Build, and Release Administrators are granted all permissions. Task group permissions follow a hierarchical model. Defaults for all the permissions can be set at the project level and can be overridden on an individual task group definition.

Use task groups to encapsulate a sequence of tasks already defined in a build or a release definition into a single reusable task. [Define and manage task groups](../../pipelines/library/task-groups.md) in the **Task groups** tab of the **Build and Release** hub.
 
> | Permission | Description | 
> |------------|-------------| 
> | **Administer task group permissions** | Can add and remove users or groups to task group security. |
> | **Delete task group** | Can delete a task group. | 
> | **Edit task group** | Can create, modify, or delete a task group. | 

<a id="alerts">  </a>

## Notifications or alerts 

::: moniker range="=azure-devops-2020"
There are no UI permissions associated with [managing email notifications or alerts](../../organizations/notifications/manage-your-personal-notifications.md). Instead, you can manage them using the [TFSSecurity](/azure/devops/server/command-line/tfssecurity-cmd#tagging-permissions) command-line tool.
::: moniker-end

- By default, members of the project level **Contributors** group can subscribe to alerts for themselves.
- Members of the **Project Collection Administrators** group,
  or users who have the **Edit collection-level information**
  can set alerts in that collection for others or for a team.
- Members of the **Project Administrators** group,
  or users who have the **Edit project-level information**
  can set alerts in that project for others or for a team.

::: moniker range="< azure-devops"

You can manage alert permissions using [TFSSecurity](/azure/devops/server/command-line/tfssecurity-cmd).

:::row:::
   :::column span="":::
  **TFSSecurity Action**
   :::column-end:::
   :::column span="":::
  **TFSSecurity Namespace**
   :::column-end:::
   :::column span="":::
  **Description**
   :::column-end:::
   :::column span="":::
  **Project Collection Administrators &**  
  **Project Collection Service Accounts**
   :::column-end:::
:::row-end:::
---
:::row:::
   :::column span="":::
  `CREATE_SOAP_SUBSCRIPTION`
   :::column-end:::
   :::column span="":::
  `EventSubscription`
   :::column-end:::
   :::column span="":::
  Can create a SOAP-based web service subscription.
   :::column-end:::
   :::column span="":::
  ✔️ 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
  `GENERIC_READ` 
   :::column-end:::
   :::column span="":::
  `EventSubscription`
   :::column-end:::
   :::column span="":::
  Can view subscription events defined for a project.
   :::column-end:::
   :::column span="":::
  ✔️ 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
  `GENERIC_WRITE` 
   :::column-end:::
   :::column span="":::
  `EventSubscription`
   :::column-end:::
   :::column span="":::
  Can create alerts for other users or for a team.
   :::column-end:::
   :::column span="":::
  ✔️ 
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
  `UNSUBSCRIBE`
   :::column-end:::
   :::column span="":::
 `EventSubscription`
   :::column-end:::
   :::column span="":::
  Can unsubscribe from an event subscription.
   :::column-end:::
   :::column span="":::
  ✔️ 
   :::column-end:::
:::row-end:::

::: moniker-end

## Related content

- [Get started with permissions, access, and security groups](about-permissions.md)   
- [Security namespace and permission reference for Azure DevOps](namespace-reference.md)    
- [Add users to an organization (Azure DevOps Services)](../accounts/add-organization-users.md)  
- [Add users to a team or a project](../../organizations/security/add-users-team-project.md)     
- [Make a user a team administrator](../settings/manage-teams.md)  
- [Troubleshoot permissions](troubleshoot-permissions.md)
