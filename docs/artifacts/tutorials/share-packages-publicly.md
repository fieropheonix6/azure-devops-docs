---
title: Share Packages publicly with public feeds
description: Use Azure Artifacts public feeds to share packages publicly.
ms.service: azure-devops-artifacts
ms.custom:
ms.date: 07/07/2023
monikerRange: 'azure-devops'
---

# Share packages publicly

[!INCLUDE [version-eq-azure-devops](../../includes/version-eq-azure-devops.md)]

Azure Artifacts provides an easy way to share packages to users outside your organization and even external customers using public feeds. Packages that are stored in public feeds can be restored and installed by anyone on the Internet.

## Prerequisites

- An Azure DevOps organization. [Create an organization](../../organizations/accounts/create-organization.md), if you don't have one already.
- A public project. [Create a public project](../../organizations/projects/create-project.md) if you don't have one already.

## Create a public feed

> [!NOTE]
> Public feeds are only available in Azure DevOps Services.

Public feeds are project-scoped feeds in a public project. Public feeds inherit the visibility settings of the hosting project.

1. Sign in to your Azure DevOps organization, and then navigate to your public project.

1. Select **Artifacts**, and then select **Create Feed**.

    :::image type="content" source="../media/new-feed-devops.png" alt-text="A screenshot showing how to create a new feed.":::

1. Give your feed a **Name**, select **Project: PublicProject (Recommended)** for its scope, and then select **Create** when you're done.

    :::image type="content" source="../media/new-public-feed.png" alt-text="A screenshot showing how to create a new public feed.":::

## Publish packages (CLI)

#### [NuGet](#tab/nuget)

- [Publish NuGet packages - (NuGet.exe)](../nuget/publish.md#publish-packages-to-a-feed-in-the-same-organization)
- [Publish NuGet packages - (dotnet)](../nuget/dotnet-exe.md#publish-packages-to-a-feed-in-the-same-organization)

#### [Npm](#tab/npm)

- [Publish npm packages](../npm/publish.md)

#### [Maven](#tab/maven)

- [Publish Maven Artifacts](../get-started-maven.md#publish-packages)

#### [Gradle](#tab/gradle)

- [Publish Artifacts using Gradle](../maven/publish-with-gradle.md)

#### [Python](#tab/python)

- [Publish Python packages](../quickstarts/python-cli.md#publish-packages)

#### [Cargo](#tab/cargo)

- [Publish Cargo packages](../get-started-cargo.md)

#### [Universal Packages](#tab/universalpackages)

- [Publish Universal Packages](../quickstarts/universal-packages.md#publish-universal-packages)

- - -

## Publish packages with Azure Pipelines

#### [NuGet](#tab/nuget)

- [Publish NuGet packages](../../pipelines/artifacts/nuget.md#publish-nuget-packages-to-a-feed-in-the-same-organization)

#### [Npm](#tab/npm)

- [Publish npm packages](../../pipelines/artifacts/npm.md#publish-packages-to-a-feed-in-the-same-organization)

#### [Maven](#tab/maven)

- [Publish Maven Artifacts](../../pipelines/artifacts/publish-maven-artifacts.md)

#### [Gradle](#tab/gradle)

- [Publish Artifacts with Gradle](../../pipelines/artifacts/build-publish-artifacts-gradle.md)

#### [Python](#tab/python)

- [Publish Python packages](../../pipelines/artifacts/pypi.md#publish-python-packages-to-a-feed)

#### [Cargo](#tab/cargo)

- [Publish Cargo packages (YAML/Classic)](../../pipelines/artifacts/cargo-pipelines.md)

#### [Universal Packages](#tab/universalpackages)

- [Publish Universal Packages](../../pipelines/artifacts/universal-packages.md#publish-a-universal-package)

- - -

> [!NOTE]
> If your organization is using a firewall or a proxy server, make sure you allow [Azure Artifacts Domain URLs and IP addresses](../../organizations/security/allow-list-ip-url.md#azure-artifacts).

## Share packages

To share your packages publicly, you can simply share your feed URL E.g. `https://dev.azure.com/<ORGANIZATION_NAME>/<PROJECT-NAME>/_artifacts/feed/<FEED_NAME>` or share individual packages with [package badges](../package-badges.md).

As long as your project is kept public, anyone can view and download packages from your public feed. Anonymous users won't be able to create new feeds or access the recycle bin.

:::image type="content" source="../media/packages-public-feed.png" alt-text="A screenshot showing the content of a public feed.":::

## Related articles

- [Package sizes and count limits](../reference/limits.md)
- [Follow a package for publish alerts](../how-to/follow-package-notifications.md)
- [Delete and recover packages](../how-to/delete-and-recover-packages.md)
