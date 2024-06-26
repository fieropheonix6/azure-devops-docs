---
title: Disable Request Access policy
titleSuffix: Azure DevOps Services
ms.custom: 
description: Learn how to stop your users from requesting access to your organization or project within your organization by disabling the Request Access policy.
ms.subservice: azure-devops-organizations
ms.assetid: 
ms.topic: conceptual
ms.author: chcomley
author: chcomley
ms.date: 05/30/2024
monikerRange: 'azure-devops'
---

# Disable your organization's Request Access policy

[!INCLUDE [version-eq-azure-devops](../../includes/version-eq-azure-devops.md)]

To prevent users from requesting access to your organization or a project within your organization, disable the 'Request Access' policy. When this policy is enabled, users can request access to a resource. Such requests trigger email notifications to administrators, prompting them to review and grant access as necessary.

Disabling the 'Request Access' policy prevents users from requesting access. Administrators don’t receive email notifications for access requests when the policy is disabled.

## Prerequisites

You must be a member of the [Project Collection Administrators group](../security/look-up-project-collection-administrators.md) and have at least Basic access. Organization owners are automatically members of this group.

## Disable Request Access policy

1. Sign in to your organization (```https://dev.azure.com/{yourorganization}```).

2. Choose ![gear icon](../../media/icons/gear-icon.png) **Organization settings**.

   ![Choose the gear icon, Organization settings](../../media/settings/open-admin-settings-vert.png)

3. Select **Policies** to find the *Request Access policy* and move the toggle to *off*.

   ![Disable the Request Access policy in Organization settings](media/request-access-policy-settings.png)

4. Provide the URL to your internal process for gaining access. Users see this URL in the error report when they try to access the organization or a project within the organization that they don't have access to.

   ![Enter the URL to your organization's internal process for gaining access.](media/disable-request-access-provide-url.png)

**Results:**

- For users who are already part of the organization: If they lack permission to access a specific project, they get a 404 error. To maintain confidentiality, the 404 error doesn’t reveal whether the project exists or not, and so doesn't provide a link to request access.
- For users who are **not** part of the organization: If they attempt to access a resource, they get a 401 error, which includes a link to the configured custom URL for requesting access.

## Related articles

- [Need help?](faq-configure-customize-organization.yml#get-support)
- [Assign access levels by group membership](assign-access-levels-by-group-membership.md)
- [Manage Conditional Access](change-application-access-policies.md)
- [Change application access policies](change-application-access-policies.md)
