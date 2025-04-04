---
title: Lock a branch in your Git repo
titleSuffix: Azure Repos
description: Use the branches page to lock a branch in Azure DevOps Services or TFS, preventing pushes to the branch.
ms.assetid: 9eecbacc-e3f2-44cb-887e-6c886001d2b6
ms.service: azure-devops-repos
ms.topic: conceptual
ms.date: 10/11/2018
monikerRange: '<= azure-devops'
ms.subservice: azure-devops-repos-git
---


# Lock a branch

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]

Prevent updates to a Git [branch](./create-branch.md) by locking the branch. 
Locking a branch prevents other users from changing the existing commit history. 
Locking also blocks any new commits from being added to the branch by others. 

## Locking limitations

Locking is ideal for preventing new changes that might conflict with an important merge or to place a branch into a read-only state. 
Use [branch policies](branch-policies.md) and [pull requests](pull-requests.md) with locking to ensure that changes in a branch get reviewed before they get merged and prevent changes in the locked branch.

Locking doesn't prevent cloning of a repo or fetching updates made in the branch into your local repo.
Share with your team the reason for the locking of the branch and make sure your team knows what to 
do to work with the branch after it is unlocked. 

## Prerequisites

| Category | Requirements |
|-------------|-------------|
|**Permissions**|User who locked the branch or [**Remove Others' Locks** permissions](set-git-repository-permissions.md#git-repository) for the branch.|

## Lock a branch using the Branches view

1. Open your repo on the web and [select the **Branches** view](manage-your-branches.md).

2. Locate your branch on the **Branches** view. You can search for your branch using the **Search all branches** box in the upper right.

3. Lock the branch by selecting the **...** icon next to the branch name and then selecting **Lock** from the menu. A lock icon will appear next to the branch name.
   Unlock a locked branch by selecting **Unlock** from the same menu.

   ![Lock a branch from the branches context menu](media/branches/branches_context_menu_lock.png)