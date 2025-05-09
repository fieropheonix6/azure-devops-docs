---
ms.subservice: azure-devops-security
ms.author: chcomley
author: chcomley
ms.topic: include
ms.date: 05/05/2025
---

The following table lists the permissions assigned at the project-level. All these permissions are granted to members of the **Project Administrators** group, except for the **Delete shared Analytics views** and **Edit shared Analytics views** permissions. For a description of each permission, see [Permissions and groups reference, Groups](../permissions.md#project-level-permissions).

> [!NOTE]   
> Permissions associated with Analytics require that the Inherited process model is selected for an on-premises project collection.

:::row:::
   :::column span="":::

      **General**

      ::: moniker range="azure-devops"

      - Delete team project
      - Edit project-level information
      - Manage project properties
      - Rename team project
      - Suppress notifications for work item updates
      - Update project visibility
      - View project-level information

      ::: moniker-end
      ::: moniker range="<azure-devops"

      - Delete team project
      - Edit project-level information
      - Manage project properties
      - Rename team project
      - Suppress notifications for work item updates
      - View project-level information

      ::: moniker-end

      **Boards**

      - Bypass rules on work item updates
      - Change process of team project
      - Create tag definition
      - Delete and restore work items
      - Move work items out of this project
      - Permanently delete work items

   :::column-end:::
   :::column span="":::
   
      **Analytics**

      - Delete shared Analytics views
      - Edit shared Analytics views
      - View analytics

      **Test Plans**

      - Create test runs
      - Delete test runs
      - Manage test configurations
      - Manage test environments
      - View test runs

   :::column-end:::
:::row-end:::