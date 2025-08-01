---
title: Azure DevOps Released Features
author: gloridelmorales
ms.author: glmorale
ms.date: 6/30/2025
ms.topic: article
ms.service: azure-devops
ms.subservice: azure-devops-release-notes
description: Azure DevOps release notes and server build numbers
hide_comments: true
---
# Azure DevOps Released Features

---

\| <a href="https://aka.ms/azuredevops/releasenotes" target="blank">What's New</a>
\| <a href="https://developercommunity.visualstudio.com/spaces/21/index.html" target="blank">Developer Community</a>
\| <a href="https://devblogs.microsoft.com/devops/" target="blank">DevOps Blog</a>
\| <a href="/azure/devops/?view=azure-devops&preserve-view=true" target="blank">Documentation</a> \|

---

## Released features
## Azure DevOps Services

The released features timeline lists significant features delivered to Azure DevOps Services and the corresponding version of Azure DevOps Server.
Versions in the "Server" column are linked to the appropriate download location. 

You can also [view the build numbers for each version](#azure-devops-server-build-numbers). Versions in italics are planned for the future and subject to change.

<table>
    <thead>
        <tr>
            <th>Service Update</th>
            <th>Feature</th>
            <th>Area</th>
            <th>Server</th>
        </tr>
    </thead>
<tr>
    <td rowspan="6"><a href="2025/sprint-258-update.md" data-raw-source="[30 June 2025](2025/sprint-258-update.md)"> June 30 2025</a></td>
    <td>Azure DevOps MCP Server public preview</td><td>General</td><td>N/A</td></tr>
    <td>New organizations won't offer public projects</td><td>General</td><td>N/A</td></tr>
    <td>One click enablement for dependency scanning now in public preview</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Service hooks for GitHub Advanced Security for Azure DevOps alerts generally available</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Syntax highlighting support for Kusto Query Language</td><td>Repos</td><td>Future</td></tr>
    <td>Ability to associate Java, JavaScript and Python tests to manual test cases</td><td>Test Plans</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="13"><a href="2025/sprint-257-update.md" data-raw-source="[16 June 2025](2025/sprint-257-update.md)"> June 16 2025</a></td>
    <td>GitHub Advanced Security is now available as GitHub Secret Protection and Code Security for Azure DevOps</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Restrict personal access token (PAT) creation organization policy now in public preview</td><td>General</td><td>Future</td></tr>
    <td>Removal of expired Azure DevOps OAuth Apps</td><td>General</td><td>N/A</td></tr>
    <td>New Microsoft Entra OAuth scopes</td><td>General</td><td>Future</td></tr>
    <td>Request Access URL availability</td><td>General</td><td>Future</td></tr>
    <td>Managed DevOps Pools - Image Deprecations</td><td>Pipelines</td><td>N/A</td></tr>
    <td>New Triggers page</td><td>Pipelines</td><td>Future</td></tr>
    <td>StringList parameter type</td><td>Pipelines</td><td>Future</td></tr>
    <td>See the full YAML code of a pipeline run</td><td>Pipelines</td><td>Future</td></tr>
    <td>Introducing New Test Plans directory</td><td>Test Plans</td><td>Future</td></tr>
    <td>Advanced Test Case result history</td><td>Test Plans</td><td>Future</td></tr>
    <td>View Test Case State in Execute tab</td><td>Test Plans</td><td>Future</td></tr>
    <td>Default resume for paused test case</td><td>Test Plans</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="7"><a href="2025/sprint-256-update.md" data-raw-source="[19 May 2025](2025/sprint-256-update.md)"> May 19 2025</a></td>
    <td>Advanced Security now accepts results with URI locations</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>GitHub Integration: Pull Request Mentions</td><td>Boards</td><td>Future</td></tr>
    <td>Windows Server 2019 hosted image deprecation schedule</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Support for Jupyter Notebook Diffing in PR</td><td>Repos</td><td>Future</td></tr>
    <td>Support for YAML pipelines in Test Plans</td><td>Test Plans</td><td>Future</td></tr>
    <td>View Recent Test Results in Test Case</td><td>Test Plans</td><td>Future</td></tr>
    <td>Available Data for Rollup Columns in backlog</td><td>Reporting</td><td>Future</td></tr>
<tr>
    <td rowspan="3"><a href="2025/sprint-255-update.md" data-raw-source="[23 April 2025](2025/sprint-255-update.md)"> 23 April 2025</a></td>
    <td>Manage high privilege scopes, pipeline decorators, and unpublished extensions</td><td>General</td><td>Future</td></tr>
    <td>Advanced Security now accepts results with URI locations</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>GitHub Integration: State Transition Support</td><td>Boards</td><td>Future</td></tr>
<tr>
    <td rowspan="13"><a href="2025/sprint-254-update.md" data-raw-source="[3 April  2025](2025/sprint-253-update.md)"> 3 April  2025</a></td>
    <td>No new Azure DevOps OAuth apps beginning April 2025 </td><td>General</td><td>Future</td></tr>
    <td>Server Name Indication (SNI) now mandatory for Azure DevOps Services </td><td>General</td><td>Future</td></tr>
    <td>GitHub Integration: Improvements linking to commits, branches and pull requests</td><td>Boards</td><td>Future</td></tr>
    <td>GitHub Integration: Show build status for YAML pipelines</td><td>Boards</td><td>Future</td></tr>
    <td>Delivery Plans limit increased</td><td>Boards</td><td>Future</td></tr>
    <td>TFVC check-in policies changes </td><td>Repos</td><td>Future</td></tr>
    <td>Enhancement to GetRepository API</td><td>Repos</td><td>Future</td></tr>
    <td>Enhancement to Pull Requests Query API</td><td>Repos</td><td>Future</td></tr>
    <td>Improved visibility into YAML pipeline stage dependencies</td><td>Pipelines</td><td>Future</td></tr>
    <td>New Agent CDN</td><td>Pipelines</td><td>Future</td></tr>
    <td>Node 16 will be removed from pipelines-* Pipeline agent packages</td><td>Pipelines</td><td>Future</td></tr>
    <td>Retirement of action logging and switch to screen recording</td><td>Test Plans</td><td>Future</td></tr>
    <td>Auto-pause manual test run</td><td>Test Plans</td><td>Future</td></tr>
 <tr>
    <td rowspan="13"><a href="2025/sprint-253-update.md" data-raw-source="[20 March  2025](2025/sprint-253-update.md)"> 20 March  2025</a></td>
    <td>Overlapping secrets for Azure DevOps OAuth </td><td>General</td><td>Future</td></tr>
    <td>Deprecation of Languages statistics tags from the Project Summary Page </td><td>General</td><td>Future</td></tr>
    <td>Delivery Plans permission added </td><td>General</td><td>Future</td></tr>
    <td>Security overview risk page enhanced with new columns and filtering options</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Multi-repository publishing scenarios supported for GitHub Advanced Security for Azure DevOps</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Service hooks for GitHub Advanced Security alerts for Azure DevOps (preview)</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>pnpm 9 support comes to GitHub Advanced Security for Azure DevOps dependency scanning </td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Hosted image updates</td><td>Pipelines</td><td>Future</td></tr>
    <td>Workload identity federation uses Entra issuer</td><td>Pipelines</td><td>Future</td></tr>
    <td>Gradle@4 task</td><td>Pipelines</td><td>Future</td></tr>
    <td>Identity of user who requested a stage to run</td><td>Pipelines</td><td>Future</td></tr>
    <td>Improvements on the Publish code coverage results v2 task</td><td>Test Plans</td><td>Future</td></tr>
    <td>Export test cases with custom columns in XLSX</td><td>Test Plans</td><td>Future</td></tr>
  <tr>
    <td rowspan="11"><a href="2025/sprint-252-update.md" data-raw-source="[24 February  2025](2025/sprint-253-update.md)"> 24 February  2025</a></td>
    <td>Microsoft Entra profile information (preview) </td><td>General</td><td>Future</td></tr>
    <td>Basic access included with GitHub Enterprise </td><td>General</td><td>Future</td></tr>
    <td>Azure DevOps Allowed IP addresses</td><td>General</td><td>Future</td></tr>
    <td>One click enablement for dependency scanning preview</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Deleted branches removed from Advanced Security branch picker</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>GitHub Integration: Linking the Merge Commit </td><td>Boards</td><td>Future</td></tr>
    <td>Increase Limit of Connected GitHub Repositories</td><td>Boards</td><td>Future</td></tr>
    <td>Update on New Boards Hub Rollout</td><td>Boards</td><td>Future</td></tr>
    <td>Pipelines using Ubuntu 24.04 will show warnings for certain tasks</td><td>Pipelines</td><td>Future</td></tr>
    <td>Informational runs</td><td>Pipelines</td><td>Future</td></tr>
    <td>Undo test step in web and desktop runner</td><td>Test Plans</td><td>Future</td></tr>    
<tr>
    <td rowspan="14"><a href="2025/sprint-251-update.md" data-raw-source="[12 February  2025](2025/sprint-251-update.md)"> 12 February  2025</a></td>
    <td>Removal of Generate Git Credentials Button in Repos and Wiki </td><td>General</td><td>Future</td></tr>
    <td>Update to Azure DevOps Allowed IP addresses </td><td>General</td><td>Future</td></tr>
    <td>GitHub Advanced Security updates for default branch changes</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>CodeQL installation for self-hosted agents supports proxy configurations</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Alerts branch picker now displays all branches with a successful scan</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Enhanced pull request annotations in GitHub Advanced Security </td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Improvements for Get alerts API</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Azure Classic Service Connections are being retired</td><td>Pipelines</td><td>Future</td></tr>
    <td>Managed DevOps Pools is generally available</td><td>Pipelines</td><td>Future</td></tr>
    <td>New tasks to implement secret-less access to Azure storage accounts</td><td>Pipelines</td><td>Future</td></tr>
    <td>Direct link from Test Plan work item to Test Plans page</td><td>Test Plans</td><td>Future</td></tr>
    <td>Azure Test Plans bug fixes</td><td>Test Plans</td><td>Future</td></tr>
    <td>Export test cases with custom columns in XLSX</td><td>Test Plans</td><td>N/A</td></tr>
    <td>Auto-pause manual test case run</td><td>Test Plans</td><td>Future</td></tr>
<tr>
    <td rowspan="7"><a href="2025/sprint-248-update.md" data-raw-source="[17 January 2025](2025/sprint-248-update.md)"> 17 January 2025</a></td>
    <td>Tool specific security overview coverage</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Azure Boards Integration with GitHub Enterprise Cloud with Data Residency </td><td>Boards</td><td>Future</td></tr>
    <td>Sparse checkout for Azure Repos</td><td>Repos</td><td>Future</td></tr>
    <td>Make cross-repo policies case-sensitive</td><td>Repos</td><td>Future</td></tr>
    <td>New pipeline expression function</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Enhancements to ManualValidation task</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Azure Test Plans bug fixes</td><td>Test Plans</td><td>Future</td></tr>
<tr>
    <td rowspan="10"><a href="2024/sprint-247-update.md" data-raw-source="[13 November 2024](2024/sprint-247-update.md)"> 13 November 2024</a></td>
    <td>Commit-less builds supported for dependency scanning</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>File previews and annotations for CodeQL scans using sourcesFolder</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>New REST API limit on work item comments </td><td>Boards</td><td>Future</td></tr>
    <td>Search pull requests by title on PR listing page</td><td>Repos</td><td>Future</td></tr>
    <td>macOS-15 Sequoia is available in preview</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Improvements to service connection App registration attribution</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Azure Test Runner version 1.2.2</td><td>Test Plans</td><td>Future</td></tr>
    <td>New sorting capabilities in Test Plans directory</td><td>Test Plans</td><td>Future</td></tr>
    <td>Auto Pause for Test Case Run preview</td><td>Test Plans</td><td>Future</td></tr>
    <td>New release version for Test and Feedback Extensions (TFE)</td><td>Test Plans</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="16"><a href="2024/sprint-246-update.md" data-raw-source="[16 October 2024](2024/sprint-246-update.md)"> 16 October 2024</a></td>
    <td>Copy code block to clipboard </td><td>General</td><td>Future</td></tr>
    <td>Entra Profile information </td><td>General</td><td>Future</td></tr>
    <td>Pull request annotations for dependency and code scanning</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>New pip detection strategy for dependency scanning</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Alert rule IDs now integrated into result fingerprints </td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Enhanced tag management on work item form </td><td>Boards</td><td>N/A</td></tr>
    <td>Improved image support in work item comments</td><td>Boards</td><td>N/A</td></tr>
    <td>GitHub pull request insights</td><td>Boards</td><td>N/A</td></tr>
    <td>Configure target branches for pull requests</td><td>Repos</td><td>Future</td></tr>
    <td>Support mermaid diagrams in markdown file preview</td><td>Repos</td><td>Future</td></tr>
    <td>Ubuntu 24.04 on Azure Pipelines hosted agents</td><td>Pipelines</td><td>Future</td></tr>
    <td>Use Workload identity federation in Azure integration tests</td><td>Pipelines</td><td>Future</td></tr>
    <td>New Azure service connection creation experience with improved Managed identity support</td><td>Pipelines</td><td>Future</td></tr>
    <td>Run children stages when parent stage fails</td><td>Pipelines</td><td>Future</td></tr>
    <td>Authentication to Azure Artifacts using a public feed and Cargo</td><td>Artifacts</td><td>N/A</td></tr>
    <td>Improve pasting of HTML based content into Wikis</td><td>Wiki</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="14"><a href="2024/sprint-245-update.md" data-raw-source="[26 September 2024](2024/sprint-245-update.md)"> 26 September 2024</a></td>
    <td>Pull request branches now visible in Advanced Security branch picker </td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Automatic updates for default branch changes in Advanced Security</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Generic third-party SARIF support for Advanced Security</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Alert rule IDs now integrated into result fingerprints </td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Pull request annotations feature in public preview </td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>AB# links on GitHub pull requests</td><td>Boards</td><td>N/A</td></tr>
    <td>REST API support for connecting GitHub repositories</td><td>Boards</td><td>N/A</td></tr>
    <td>Permanently delete attachments</td><td>Boards</td><td>Future</td></tr>
    <td>New Health and usage panel in repo file hub </td><td>Repos</td><td>Future</td></tr>
    <td>Azure Pipeline agent v4 runs on .NET 8</td><td>Pipelines</td><td>Future</td></tr>
    <td>Preview mode for shell tasks arguments validation</td><td>Pipelines</td><td>Future</td></tr>
    <td>Seamless build Pipeline integration for test case execution</td><td>Test Plans</td><td>Future</td></tr>
    <td>Test and feedback extension in Manifest V3 (Edge release)</td><td>Test Plans</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="7"><a href="2024/sprint-244-update.md" data-raw-source="[4 September 2024](2024/sprint-244-update.md)"> 4 September 2024</a></td>
    <td>New Advanced Security API endpoint to retrieve all branches with successful Advanced Security analyses</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Advanced Security List Alerts API return all alerts across all branches</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Area and iteration level fields</td><td>Boards</td><td>Future</td></tr>
    <td>UI support of Git Submodules</td><td>Repos</td><td>Future</td></tr>
    <td>Announcing deprecation of Pipeline Tasks</td><td>Pipelines</td><td>Future</td></tr>
    <td>The Pipelines agent will show warnings for agents running Operating Systems not supported by .NET 8</td><td>Pipelines</td><td>Future</td></tr>
    <td>Enhanced Visibility for Usage Limits in Azure DevOps</td><td>Reporting</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="8"><a href="2024/sprint-243-update.md" data-raw-source="[13 August 2024](2024/sprint-242-update.md)"> 13 August 2024</a></td>
    <td>Advanced Security meter usage API now returns user identities</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Advanced Security code scanning for C# and Java projects without builds</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Managed DevOps Pools (Preview)</td><td>Pipelines</td><td>Future</td></tr>
    <td>Azure Pipelines tasks use Node 20</td><td>Pipelines</td><td>Future</td></tr>
    <td>Create build pipeline permission</td><td>Pipelines</td><td>Future</td></tr>
    <td>Exclusive lock check at stage level</td><td>Pipelines</td><td>Future</td></tr>
    <td>Template information in pipeline runs</td><td>Pipelines</td><td>Future</td></tr>
    <td>Manually triggered YAML pipeline stages</td><td>Pipelines</td><td>Future</td></tr>
<tr>
    <td rowspan="3"><a href="2024/sprint-242-update.md" data-raw-source="[25 July 2024](2024/sprint-242-update.md)"> 25 July  2024</a></td>
    <td>Connect to GitHub repository search improvements</td><td>Boards</td><td>Future</td></tr>
    <td>Create GitHub branch from work item</td><td>Boards</td><td>Future</td></tr>
    <td>Unskippable stages</td><td>Pipelines</td><td>Future</td></tr>
<tr>
    <td rowspan="4"><a href="2024/sprint-241-update.md" data-raw-source="[3 July 2024](2024/sprint-241-update.md)"> 3 July  2024</a></td>
    <td>New authentication format for Azure DevOps personal access tokens available</td><td>General</td><td>Future</td></tr>
    <td>Automated self-hosted agent install for code scanning bits in Advanced Security</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>AzureFileCopy, AzurePowerShell, and SqlAzureDacpacDeployment tasks use Az modules only</td><td>Pipelines</td><td>Future</td></tr>
    <td>Use Workload identity federation for container jobs, resources, and tasks</td><td>Pipelines</td><td>Future</td></tr>
<tr>
    <td rowspan="9"><a href="2024/sprint-240-update.md" data-raw-source="[14 June 2024](2024/sprint-240-update.md)"> 14 June  2024</a></td>
    <td>Security overview API documentation now available</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Change for deleting area and iteration paths</td><td>Boards</td><td>Future</td></tr>
    <td>Access Azure Bus from Pipelines using Microsoft Entra ID authentication</td><td>Pipelines</td><td>Future</td></tr>
    <td>Pipelines and tasks populate variables to customize Workload identity federation authentication</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Retries for server tasks </td><td>Pipelines</td><td>Future</td></tr>
    <td>Tasks that use an end-of-life Node runner version to execute emit warnings</td><td>Pipelines</td><td>Future</td></tr>
    <td>DockerCompose@0 uses Docker Compose v2 in v1 compatibility mode</td><td>Pipelines</td><td>Future</td></tr>
    <td>New setting to disable creation of TFVC repositories</td><td>Repos</td><td>Future</td></tr>
    <td>Test and Feedback Extension in Manifest V3 </td><td>Test Plans</td><td>Future</td></tr>
<tr>
    <td rowspan="5"><a href="2024/sprint-238-update.md" data-raw-source="[2 May 2024](2024/sprint-238-update.md)"> 2 May  2024</a></td>
    <td>Improve Search Results with wildcard prefixes and substrings</td><td>General</td><td>Future</td></tr>
    <td>Security overview risk view links to repository alerts</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Publish task for integrating with third-party providers</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>macOS-14 Sonoma preview and macOS-11 retirement </td><td>Pipelines</td><td>Future</td></tr>
    <td>Node 10 removed from pipelines-* Pipeline agent packages</td><td>Pipelines</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="8"><a href="2024/sprint-237-update.md" data-raw-source="[10 April 2024](2024/sprint-237-update.md)"> 10 April  2024</a></td>
    <td>Expanded set of Secret Scanning detections</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Secret Scanning now detects non-provider patterns</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Add link to GitHub commit or pull request</td><td>Boards</td><td>Future</td></tr>
    <td>AB# links on GitHub pull requests (preview)</td><td>Boards</td><td>Future</td></tr>
    <td>Connect to GitHub repository search improvements</td><td>Boards</td><td>Future</td></tr>
    <td>Edit queue build configuration permission</td><td>Pipelines</td><td>Future</td></tr>
    <td>TFX validates whether a task is using an End or Life Node runner</td><td>Pipelines</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="4"><a href="2024/sprint-236-update.md" data-raw-source="[26 March 2024](2024/sprint-236-update.md)"> 26 March  2024</a></td>
    <td>Personal access token (PAT) APIs to return maximum allowed lifespan</td><td>General</td><td>N/A</td></tr>
    <td>Azure service connections indicate when a secret has expired</td><td>Pipelines</td><td>Future</td></tr>
    <td>New AzureFileCopy@6 task supports secret-less configurations</td><td>Pipelines</td><td>Future</td></tr>
    <td>Resource utilization alerts for Azure Pipeline agents</td><td>Pipelines</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="5"><a href="2024/sprint-235-update.md" data-raw-source="[29 February 2024](2024/sprint-235-update.md)"> 29 February  2024</a></td>
    <td>Show GitHub pull request details (preview)</td><td>Boards</td><td>Future</td></tr>
    <td>Preparation for SSH-RSA deprecation in future Server version</td><td>Repos</td><td>2022.2</td></tr>
    <td>Rerun a single stage</td><td>Pipelines</td><td>Future</td></tr>
    <td>Quick Copy and Import with Test Plan or Suite ID</td><td>Test Plans</td><td>2022.2</td></tr>
    <td>Update for Azure Test Runner</td><td>Test Plans</td><td>2022.2</td></tr>
<tr>
<tr>
    <td rowspan="15"><a href="2024/sprint-234-update.md" data-raw-source="[9 February 2024](2024/sprint-234-update.md)"> 9 February  2024</a></td>
    <td>Code snippets now available in alert details view</td><td>General</td><td>Future</td></tr>
    <td>Final notice of alternate credentials deprecation</td><td>General</td><td>N/A</td></tr>
    <td>Azure Devops OAuth self-service secret rotation</td><td>General</td><td>N/A</td></tr>
    <td>Linked Azure subscription required for GitHub Advanced Security for Azure DevOps enablement</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>    
    <td>New Boards Hub Improvements</td><td>Boards</td><td>Future</td></tr>
    <td>Development and Deployment Controls</td><td>Boards</td><td>2022.2</td></tr>
    <td>Workload identity federation for Azure Resource Manager service connections is now generally available</td><td>Pipelines</td><td>Future</td></tr>
    <td>Out-of-band installation of Node 6 task runner</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Deferred approval</td><td>Pipelines</td><td>Future</td></tr>
    <td>Sequencing approvals and checks</td><td>Pipelines</td><td>Future</td></tr>
    <td>Validate and Save by default when editing YAML pipelines</td><td>Pipelines</td><td>Future</td></tr>
    <td>Prevention for unauthorized users to configure pipeline as a Build Policy</td><td>Repos</td><td>2022.2</td></tr>
    <td>Support for Rust Crates is generally available</td><td>Artifacts</td><td>N/A</td></tr>
    <td>Azure Artifacts support for npm audit</td><td>Artifacts</td><td>2022.2</td></tr>
<tr>
<tr>
    <td rowspan="6"><a href="2024/sprint-233-update.md" data-raw-source="[19 January 2024](2024/sprint-233-update.md)"> 19 January  2024</a></td>
    <td>Custom CodeQL queries now supported in GitHub Advanced Security for Azure DevOps</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>    
    <td>Team Automation Rules</td><td>Boards</td><td>Future</td></tr>
    <td>Update deprecated tasks before January 31</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Microsoft hosted agents use PowerShell 7.4</td><td>Pipelines</td><td>N/A</td></tr>
    <td>New Azure service connection secrets expire in three months</td><td>Pipelines</td><td>N/A</td></tr>
<tr>
<tr>
    <td rowspan="3"><a href="2024/sprint-232-update.md" data-raw-source="[11 January   2024](2024/sprint-232-update.md)"> 11 January  2024</a></td>
    <td>Select a geography when creating a new Azure DevOps organization</td><td>General</td><td>N/A</td></tr>
    <td>Removed Visual Studio Subscriber option from group rules</td><td>General</td><td>N/A</td></tr>
    <td>Code Coverage results for folders</td><td>Test Plans</td><td>2022.2</td></tr>
<tr>
<tr>
    <td rowspan="3"><a href="2023/sprint-231-update.md" data-raw-source="[5 December   2023](2023/sprint-231-update.md)"> 5 December  2023</a></td>
    <td>Switch between HTML or Markdown on comments</td><td>Boards</td><td>Future</td></tr>
    <td>Improved YAML validation</td><td>Pipelines</td><td>2022.2</td></tr>
    <td>Checks scalability Phase 3</td><td>Pipelines</td><td>N/A</td></tr>
<tr>
<tr>
    <td rowspan="10"><a href="2023/sprint-230-update.md" data-raw-source="[16 November  2023](2023/sprint-230-update.md)"> 16 November 2023</a></td>
    <td>New version of the Azure DevOps Web Extension SDK </td><td>General</td><td>2022.2</td></tr>    
    <td>Azure Pipelines tasks use Node 16</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Announcing retirement of deprecated tasks</td><td>Pipelines</td><td>N/A</td></tr>
    <td>AzureRmWebAppDeployment task supports Microsoft Entra ID authentication</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Improvements to Approvals REST API</td><td>Pipelines</td><td>2022.2</td><tr>   
    <td>Bypass Approvals and Checks</td><td>Pipelines</td><td>2022.2</td></tr>  
    <td>Support for GitHub enterprise server in required template check</td><td>Pipelines</td><td>2022.2</td></tr>
    <td>Rerun invoke Azure function checks</td><td>Pipelines</td><td>2022.2</td></tr>
    <td>Work item filtering</td><td>Reporting</td><td>2022.2</td></tr>
<tr>
<tr>
    <td rowspan="5"><a href="2023/sprint-229-update.md" data-raw-source="[26 October 2023](2023/sprint-229-update.md)"> 26 October 2023</a></td>
    <td>REST API documentation now available for Advanced Security </td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Publish Test Results Task</td><td>General</td><td>2022.2</td></tr>
    <td>Building PRs from forked GitHub repositories</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Deprecation announcement for NuGet Restore v1 and NuGet Installer v0 pipeline tasks</td><td>Artifacts</td><td>N/A</td></tr>
    <td>New Dashboard directory experience</td><td>Reporting</td><td>2022.2</td></tr>
<tr>
<tr>
    <td rowspan="8"><a href="2023/sprint-228-update.md" data-raw-source="[4 October 2023](2023/sprint-227-update.md)"> 4 October 2023</a></td>
    <td>Managed identity and service principal support for Azure DevOps now in general availability (GA)</td><td>General</td><td>N/A</td></tr>
    <td>New Azure DevOps scopes available for Microsoft Identity OAuth delegated flow apps</td><td>General</td><td>N/A</td></tr>
    <td>Changes to Code Scanning (CodeQL) user input task and variables</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Publish task is no longer required for Setting up code Scanning</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>CodeQL code scanning now supports Swift</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>    
    <td>Pipeline logs now contain resource utilization</td><td>Pipelines</td><td>2022.2</td></tr>  
    <td>Azure Pipelines agent now supports Alpine Linux</td><td>Pipelines</td><td>N/A</td></tr>
<tr>
<tr>
    <td rowspan="8"><a href="2023/sprint-227-update.md" data-raw-source="[14 September 2023](2023/sprint-227-update.md)"> 14 September 2023</a></td>
    <td>Limits for area and iteration paths</td><td>Boards</td><td>2022.2</td></tr>
    <td>Pipeline agents can be registered using Azure Active Directory instead of a PAT</td><td>Pipelines</td><td>Future</td></tr>
    <td>Workload identity federation for Azure Pipelines (public preview)</td><td>Pipelines</td><td>Future</td></tr>
    <td>REST APIs for Environments</td><td>Pipelines</td><td>Future</td></tr>
    <td>Prevent Unintended Pipeline Runs</td><td>Pipelines</td><td>2022.2</td></tr>
    <td>Build GitHub Repositories Securely by Default</td><td>Pipelines</td><td>Future</td><tr>   
    <td>Disabled override of code coverage policy status to Failed when build is failing </td><td>Pipelines</td><td>2022.2</td></tr>  
    <td>Blobless and treeless filter support</td><td>Repos</td><td>2022.2</td></tr>
<tr>
<tr>
    <td rowspan="6"><a href="2023/sprint-226-update.md" data-raw-source="[23 August 2023](2023/sprint-226-update.md)"> 23 August 2023</a></td>
    <td>Project and organization-level enablement for Advanced Security </td><td>General</td><td>N/A</td></tr>
    <td>Estimated committer count during Advanced Security enablement </td><td>General</td><td>N/A</td></tr>
    <td>Retry a stage when approvals and checks time out</td><td>Pipelines</td><td>2022.2</td></tr>
    <td>Administrator role for all Environments</td><td>Pipelines</td><td>2022.2</td></tr>
    <td>Centralized control for building PRs from forked GitHub repos</td><td>Pipelines</td><td>Future</td></tr>
    <td>Azure Artifacts support for Cargo Crates (public preview) </td><td>Artifacts</td><td>2022.2</td></tr>  
<tr>
<tr>
    <td rowspan="3"><a href="2023/sprint-225-update.md" data-raw-source="[2 August 2023](2023/sprint-225-update.md)"> 2 August 2023</a></td>   
    <td>Disable creation of classic pipelines for new organizations (pre-announcement)</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Increased Azure Pipeline limits to align with the 4 MB maximum Azure Resource Manager (ARM) template size</td><td>Pipelines</td><td>2022.1</td></tr>
<tr>
<tr>
    <td rowspan="8"><a href="2023/sprint-224-update.md" data-raw-source="[11 July 2023](2023/sprint-223-update.md)"> 11 July 2023</a></td>
    <td>Alert dismissals for dependency scanning alerts in Advanced Security</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Copy link to work item</td><td>Boards</td><td>Future</td></tr>
    <td>Kubernetes tasks now support kubelogin</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Updates to YAML cron schedules</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Disable a check</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Improvements to Approvals REST API</td><td>Pipelines</td><td>Future</td></tr>
    <td>New toggles to control creation of classic pipelines</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Removing "Edit policies" permission to branch creator</td><td>Repos</td><td>2022.1</td></tr>  
<tr>
<tr>
    <td rowspan="8"><a href="2023/sprint-223-update.md" data-raw-source="[21 June 2023](2023/sprint-223-update.md)"> 21 June 2023</a></td>
    <td>Organization profile image</td><td>General</td><td>Future</td></tr>
    <td>Checks user experience improvements</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Scalable Invoke Azure Function and REST API checks changes</td><td>Pipelines</td><td>Future</td></tr>
    <td>Instructions for manual pre-installation of Node 6 on Pipeline agents</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Pipeline task changelog</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Release tasks use Microsoft Graph API</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Specify agent version in Agent VM extension</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Introducing resolved as completed in burndown and burnup charts</td><td>Reporting</td><td>2022.1</td></tr>
<tr>
<tr>
    <td rowspan="6"><a href="2023/sprint-222-update.md" data-raw-source="[6 June 2023](2023/sprint-222-update.md)"> 6 June 2023</a></td>
    <td>GitHub Advanced Security for Azure DevOps (public preview)</td><td>GitHub Advanced Security for Azure DevOps</td><td>N/A</td></tr>
    <td>Fixed a bug that allowed users to bypass restrict global personal access token (PAT) creation</td><td>General</td><td>Future</td></tr>
    <td>Markdown support for comments (private preview)</td><td>Boards</td><td>Future</td></tr>
    <td>Improvements to YAML pipeline traceability</td><td>Pipelines</td><td>Future</td></tr>
    <td>Automatic tokens created for Kubernetes Service Connection</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Preview of macOS 13 Ventura for Azure Pipeline hosted pools</td><td>Pipelines</td><td>N/A</td></tr>
<tr>
    <td rowspan="4"><a href="2023/sprint-221-update.md" data-raw-source="[9 May 2023](2023/sprint-221-update.md)"> 9 May 2023</a></td>
    <td>Swimlane rules</td><td>Boards</td><td>Future</td></tr>
    <td>Pipeline settings audit improvements</td><td>Pipelines</td><td>Future</td></tr>
    <td>Pull Request widget for multiple repos is now generally available</td><td>Reporting</td><td>2022.1</td></tr>
<tr>
<tr>
    <td rowspan="3"><a href="2023/sprint-220-update.md" data-raw-source="[20 April 2023](2023/sprint-220-update.md)"> 20 April 2023</a></td>
    <td>Sticky "Save" and "Save and Close" button </td><td>Boards</td><td>Future</td></tr>
    <td>Stage quick actions</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Analytics Views are now generally available</td><td>Reporting</td><td>2022.1</td></tr>
<tr>
    <td rowspan="3"><a href="2023/sprint-219-update.md" data-raw-source="[31 March 2023](2023/sprint-219-update.md)"> 31 March 2023</a></td>
    <td>Service principal and managed identity support in Azure DevOps (public preview) </td><td>General</td><td>N/A</td></tr>
    <td>REST API support for connecting GitHub repositories (preview)</td><td>Boards</td><td>Future</td></tr>   
    <td>Pipeline Agent end of support for Debian 9, Fedora 32, macOS 10.14 and others</td><td>Pipelines</td><td>N/A</td></tr>
 <tr>
    <td rowspan="5"><a href="2023/sprint-218-update.md" data-raw-source="[8 March 2023](2023/sprint-218-update.md)"> 8 March 2023</a></td>
    <td>Node runner download task</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Updated TFX Node runner validation</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Service hook for job state change</td><td>Pipelines</td><td>Future</td></tr>
    <td>Improved security when creating GitHub Enterprise Server (hosted Pipelines)</td><td>Pipelines</td><td>Future</td></tr>
    <td>Dashboards last accessed date and modified By</td><td>Reporting</td><td>2022.1</td></tr>
<tr>
    <td rowspan="5"><a href="2023/sprint-217-update.md" data-raw-source="[17 February 2023](2023/sprint-217-update.md)"> 17 February 2023</a></td>
    <td>License source column in user list export</td><td>General</td><td>Future</td></tr>
    <td>Interactive boards reports</td><td>Boards</td><td>2022.1</td></tr>
    <td>Search for filter stages in side panel</td><td>Pipelines</td><td>Future</td></tr>
    <td>Pipeline agent v3 (.NET 6) rolling out</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Pull request widget for multiple repos (private preview)</td><td>Reporting</td><td>2022.1</td></tr>
<tr>
    <td rowspan="5"><a href="2023/sprint-216-update.md" data-raw-source="[7 February 2023](2023/sprint-216-update.md)"> 7 February 2023</a></td>
    <td>New save comments permission</td><td>Boards</td><td>2022.1</td></tr>
    <td>Red Hat 6 will no longer receive Pipeline agent updates</td><td>Pipelines</td><td>Future</td></tr>
    <td>Pipeline stages side panel</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Restrict opening protected resources to resource administrators</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Copy Dashboard</td><td>Reporting</td><td>Future</td></tr>   
<tr>
    <td rowspan="9"><a href="2023/sprint-215-update.md" data-raw-source="[25 January 2023](2023/sprint-215-update.md)"> 25 January 2023</a></td>
    <td>Prevent editing of shareable picklists fields</td><td>Boards</td><td>2022.1</td></tr>
    <td>Swimlane colors</td><td>Boards</td><td>Future</td></tr>
    <td>Experience improvements to pipeline permissions</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Ability to disable masking for short secrets</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>New PAT Scope for managing pipeline authorization and approvals and checks</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Variables as inputs in checks</td><td>Pipelines</td><td>Future</td></tr>
    <td>Script to self-validate pipeline agent version</td><td>Pipelines</td><td>Future</td></tr>
    <td>Pipeline run status overview icon</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Support for subpages table</td><td>Wiki</td><td>Future</td></tr>
<tr>
    <td rowspan="7"><a href="2023/sprint-214-update.md" data-raw-source="[12 January 2023](2023/sprint-214-update.md)"> 12 January 2023</a></td>
    <td>Extensions should display their Scopes</td><td>General</td><td>2022.1</td></tr>
    <td>Card resize logic in Delivery Plans</td><td>Boards</td><td>2022.1</td></tr>
    <td>Batch update improvements</td><td>Boards</td><td>2022.1</td></tr>
    <td>Batch delete API</td><td>Boards</td><td>2022.1</td></tr>
    <td>Support for Tokyo version of ServiceNow</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>New predefined system variable</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>General Availability of templates support in YAML editor</td><td>Pipelines</td><td>Future</td></tr>
<tr>
<tr>
    <td rowspan="11"><a href="2022/sprint-213-update.md" data-raw-source="[8 December 2022](2022/sprint-213-update.md)"> 8 December 2022</a></td>
    <td>Copy comment links</td><td>Boards</td><td>Future</td></tr>
    <td>Container Registry service connections can now use Azure Managed Identities</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Audit log events related to pipeline permissions</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Ensure your organization only uses YAML pipelines</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Service hook for job state change</td><td>Pipelines</td><td>Future</td></tr>
    <td>New PAT scope required to update pipeline General Settings</td><td>Pipelines</td><td>Future</td></tr>
    <td>Fine-grained access management for agent pools</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Prevent granting all pipelines access to protected resources</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Improved security when building pull requests from forked GitHub repositories</td><td>Pipelines</td><td>Future</td></tr>
    <td>Macos-latest label will point to macos-12 image</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Ubuntu-latest label will point to ubuntu-22.04 image</td><td>Pipelines</td><td>N/A</td></tr>
<tr>
    <td rowspan="8"><a href="2022/sprint-212-update.md" data-raw-source="[2 November 2022](2022/sprint-212-update.md)"> 2 November 2022</a></td>
    <td>Edit work item link types</td><td>Boards</td><td>Future</td></tr>
    <td>Create temporary query REST endpoint</td><td>Boards</td><td>2022.1</td></tr>    
    <td>@CurrentIteration macro in Delivery Plans</td><td>Boards</td><td>2022.1</td></tr>
    <td>Template Expressions in Repository Resource Definition</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Template Expressions in Container Resource Definition</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Audit Events for Changes to Approvals</td><td>Pipelines</td><td>Future</td></tr>
    <td>Task library exposes Agent hosting model</td><td>Pipelines</td><td>Future</td></tr>
</tr>
    <td rowspan="5"><a href="2022/sprint-211-update.md" data-raw-source="[11 October 2022](2022/sprint-211-update.md)"> 11 October 2022</a></td>
    <td>Create personal access tokens to deploy to the Marketplace</td><td>Platform</td><td>Future</td></tr>
    <td>Option to maintain hierarchy with filters</td><td>Boards</td><td>Future</td></tr>
    <td>Copy work item attachment URL</td><td>Boards</td><td>Future</td></tr>
    <td>Pipeline Agent supports Group Managed Service Accounts as service account</td><td>Pipelines</td><td>Future</td></tr>
    <td>Show Parent in Query Results Widget</td><td>Reporting</td><td>2022.1</td></tr>
</tr>
    <td rowspan="6"><a href="2022/sprint-210-update.md" data-raw-source="[4 October 2022](2022/sprint-210-update.md)"> 4 October 2022</a></td>
    <td>All Public REST APIs support granular PAT scopes</td><td>General</td><td>2022.1</td></tr>
    <td>Move to column and move to swimlane</td><td>Boards</td><td>Future</td></tr>
    <td>Windows PowerShell task performance improvement</td><td>Pipelines</td><td>Future</td></tr>
    <td>Pipelines Agent on .NET 6 pre-announcement</td><td>Pipelines</td><td>Future</td></tr>
    <td>Node 16 task runner in pipeline agent</td><td>Pipelines</td><td>Future</td></tr>
    <td>New user interface for upstream package search</td><td>Artifacts</td><td>2022.1</td></tr>
</tr>
    <td rowspan="8"><a href="2022/sprint-209-update.md" data-raw-source="[12 September 2022](2022/sprint-209-update.md)"> 12 September 2022</a></td>
    <td>Increase Delivery Plans team limit from 15 to 20</td><td>Boards</td><td>2022.1</td></tr>
    <td>Fixed bug in Reporting Work Item Links Get API</td><td>Boards</td><td>2022.1</td></tr>
    <td>New Boards Hub bug fixes</td><td>Boards</td><td>2022.1</td></tr>
    <td>Disable showing the last commit message for a pipeline run</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Consumed resources and template parameters in Pipelines Runs Rest API</td><td>Pipelines</td><td>2022.1</td></tr>    
    <td>Add support for string split function in YAML expression</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Do not sync tags when fetching a Git repository</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Updated brownout schedule for Ubuntu 18.04 images</td><td>Pipelines</td><td>N/A</td></tr>
</tr>
    <td rowspan="3"><a href="2022/sprint-208-update.md" data-raw-source="[12 August 2022](2022/sprint-208-update.md)"> 12 August 2022</a></td>
    <td>Improved error message when failing to load pipelines</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>General availability of Ubuntu 22.04 for Azure Pipelines hosted pools</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Announcing deprecation of Ubuntu 18.04 images</td><td>Pipelines</td><td>N/A</td></tr>
</tr>
    <td rowspan="9"><a href="2022/sprint-207-update.md" data-raw-source="[28 July 2022](2022/sprint-207-update.md)"> 28 July 2022</a></td>
    <td>Pipelines REST API Security Improvements</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Use proxy URLs for GitHub Enterprise integration</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Scheduled builds improvements</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Updates to "Run stage state changed" service hook event</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Change in the default scope of access tokens in classic build pipelines</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Azure Pipelines support for San Diego release of ServiceNow</td><td>Pipelines</td><td>2022.1</td></tr>
    <td>Announcing retirement of Windows 2016 image</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Announcing deprecation of macOS 10.15 Catalina images</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Updated default feed permissions</td><td>Artifacts</td><td>2022.1</td></tr>
</tr>
    <td rowspan="5"><a href="2022/sprint-206-update.md" data-raw-source="[14 July 2022](2022/sprint-206-update.md)"> 14 July 2022</a></td>
    <td>Filter on work item history</td><td>Boards</td><td>Future</td></tr> 
    <td>Last Accessed column on Delivery Plans page</td><td>Board</td><td>2022.1</td></tr>
    <td>Visualize all dependencies on Delivery Plans</td><td>Boards</td><td>2022.1</td></tr>
    <td>New work item revision limits</td><td>Boards</td><td>2022.1</td></tr>
    <td>Current project set as default scope for build access token in classic pipelines</td><td>Pipelines</td><td>2022.1</td></tr>
</tr>
    <td rowspan="7"><a href="2022/sprint-205-update.md" data-raw-source="[27 June 2022](2022/sprint-205-update.md)"> 27 June 2022</a></td>
    <td>Project Collection Administrators can opt in for notifications related to personal access tokens found in a GitHub public repository</td><td>General</td><td>N/A</td></tr> 
    <td>Enforcing security validation for all Azure DevOps requests</td><td>General</td><td>N/A</td></tr>
    <td>Assigned To children in Kanban cards</td><td>Boards</td><td>2022</td></tr>
    <td>General availability of Query by Parent ID</td><td>Boards</td><td>Future</td></tr>
    <td>Support Group Managed Service Accounts as agent service account</td><td>Pipelines</td><td>2022</td></tr>
    <td>Informational runs</td><td>Pipelines</td><td>2022</td></tr>
    <td>Build Definition REST API retentionRules property is obsolete</td><td>Pipelines</td><td>2022</td></tr>
</tr>
    <td rowspan="4"><a href="2022/sprint-204-update.md" data-raw-source="[2 June 2022](2022/sprint-204-update.md)"> 2 June 2022</a></td> 
    <td>Improved "Show more items" UX</td><td>Boards</td><td>2022</td></tr>
    <td>General availability of Copy Dashboard</td><td>Boards</td><td>2022</td></tr>
    <td>Ubuntu 22.04 in preview for Azure Pipelines hosted pools</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Preview of macOS 12 Monterey for Azure Pipeline hosted pools</td><td>Pipelines</td><td>N/A</td></tr>
</tr>
    <td rowspan="4"><a href="2022/sprint-203-update.md" data-raw-source="[4 May 2022](2022/sprint-203-update.md)"> 4 May 2022</a></td>    
    <td>Move to column position on Kanban Board</td><td>Boards</td><td>2022</td></tr>
    <td>Added "Will not Fix" value to Bug reason field</td><td>Boards</td><td>2022</td></tr>
    <td>Upstream cross-organization packages</td><td>Artifacts</td><td>N/A</td></tr>
</tr>
    <td rowspan="6"><a href="2022/sprint-202-update.md" data-raw-source="[20 April 2022](2022/sprint-202-update.md)"> 20 April 2022</a></td> 
    <td>Auditing is now an opt-in feature for your organization</td><td>General</td><td>N/A</td></tr>
    <td>Fixed looping login issue due to incorrectly configured IP conditional access policies</td><td>General</td><td>N/A</td></tr>
    <td>Guest users will only see public user data</td><td>General</td><td>N/A</td></tr>
    <td>New Boards Hub now available in public preview</td><td>Boards</td><td>2022</td></tr>
    <td>Extend YAML pipelines template to pass stage, job, and deployment context information</td><td>Pipelines</td><td>2022</td></tr>
    <td>Updated retirement date for Windows 2016 hosted images</td><td>Pipelines</td><td>N/A</td></tr>
</tr>
    <td rowspan="4"><a href="2022/sprint-201-update.md" data-raw-source="[29 March 2022](2022/sprint-201-update.md)">29 March 2022</a></td> 
    <td>Remove the ability to download a deleted attachment from work item history</td><td>Boards</td><td>2022</td></tr>
    <td>New extension points for Pipelines details view</td><td>Pipelines</td><td>2022</td></tr>
    <td>Improved migration to Azure DevOps Services</td><td>Pipelines</td><td>2022</td></tr>
    <td>Improvement to Pipelines Runs REST API</td><td>Pipelines</td><td>2022</td></tr>
</tr> 
    <td rowspan="3"><a href="2022/sprint-200-update.md" data-raw-source="[28 February 2022](2022/sprint-200-update.md)">28 February 2022</a></td> 
    <td>Updates to Azure File Copy task</td><td>Pipelines</td><td>2022</td></tr>
    <td>Improvement to user interface</td><td>Artifacts</td><td>N/A</td></tr>
    <td>Support for additional diagram types in wiki pages</td><td>Wiki</td><td>2022</td></tr>
</tr> 
    <td rowspan="3"><a href="2022/sprint-199-update.md" data-raw-source="[11 February 2022](2022/sprint-199-update.md)">11 February 2022</a></td> 
    <td>Improvements to strengthen security in Azure DevOps</td><td>General</td><td>N/A</td></tr>
    <td>Changes to third-party applications access</td><td>General</td><td>N/A</td></tr>
    <td>Pipelines Agent runtime upgrade planning</td><td>Pipelines</td><td>N/A</td></tr>
</tr> 
    <td rowspan="2"><a href="2022/sprint-198-update.md" data-raw-source="[19 January 2022](2022/sprint-198-update.md)">19 January 2022</a></td> 
    <td>The default agent specification for pipelines will be Windows-2022 </td><td>Pipelines</td><td>2022</td></tr>
    <td>Pipeline folder rename validates permissions</td><td>Pipelines</td><td>2022</td></tr>
    <td rowspan="2"><a href="2021/sprint-196-update.md" data-raw-source="[6 December 2021](2021/sprint-196-update.md)">6 December 2021</a></td> 
    <td>Announcing retirement of macOS 10.14 Mojave images</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Brownout schedule for Windows 2016 hosted images</td><td>Pipelines</td><td>N/A</td></tr>
    <td rowspan="7"><a href="2021/sprint-195-update.md" data-raw-source="[16 November 2021](2021/sprint-195-update.md)">16 November 2021</a></td> 
    <td>Assign Azure DevOps Administrator role to an Azure AD group</td><td>General</td><td>N/A</td></tr>
    <td>Automatic retries for a task</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Consume inputs from another task in a decorator</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Improvements to service connections usage history</td><td>Pipelines</td><td>N/A</td></tr>
    <td>The default agent specification for Classic pipelines is now Windows-2019</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Improvements to Copy Dashboard</td><td>Reporting</td><td>2022</td></tr>
    <td>Filter on null values in burndown chart widget</td><td>Reporting</td><td>2022</td></tr>
    <td rowspan="5"><a href="2021/sprint-194-update.md" data-raw-source="[19 October 2021](2021/sprint-194-update.md)">19 October 2021</a></td> 
    <td>Post neutral status to GitHub when a build is skipped</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Access to all pipelines is turned off by default in protected resources</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Inject task before or after specified target tasks using a decorator</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Announcing a deprecation schedule for Windows 2016 hosted images</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Announcing deprecation of macOS 10.14 hosted images</td><td>Pipelines</td><td>N/A</td></tr>
    <td rowspan="7"><a href="2021/sprint-193-update.md" data-raw-source="[28 September 2021](2021/sprint-193-update.md)">28 September 2021</a></td> 
    <td>Improved tenant switch requests reliability</td><td>General</td><td>N/A</td></tr>
    <td>Emphasize tags in Delivery Plans using colors</td><td>Boards</td><td>2022</td></tr>
    <td>Filter cards based on boolean field types in Delivery Plans</td><td>Boards</td><td>2022</td></tr>
    <td>Work item titles are always visible in Delivery Plan cards</td><td>Boards</td><td>2022</td></tr>
    <td>Show light green colored dependency icon for work items that have dependencies with no issues</td><td>Boards</td><td>2022</td></tr>
    <td>macOS-latest label will soon point to macOS-11 image</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Updated schedule for removal of Ubuntu 16.04 image on Microsoft-hosted agents</td><td>Pipelines</td><td>N/A</td></tr>
    </tr> 
    <td rowspan="10"><a href="2021/sprint-192-update.md" data-raw-source="[8 September 2021](2021/sprint-192-update.md)">8 September 2021</a></td>
    <td>New YAML conditional expressions</td><td>Pipelines</td><td>2022</td></tr>
    <td>Support for wild cards in path filters</td><td>Pipelines</td><td>2022</td></tr>
    <td>Support for multiple statuses in Bitbucket</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Allow contributors to skip seeking PR comments prior to build validation</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Windows Server 2022 with Visual Studio 2022 is now available on Microsoft-hosted agents (preview)</td><td>Pipelines</td><td>N/A</td></tr>
    <td>General availability of macOS 11 Big Sur on Microsoft-hosted agents</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Removal of Ubuntu 16.04 image on Microsoft-hosted agents</td><td>Pipelines</td><td>N/A</td></tr>
    <td>New TFVC pages are generally available</td><td>Repos</td><td>2022</td></tr>
    <td>Configure branch creators to not get "Manage permissions" on their branches</td><td>Repos</td><td>2022</td></tr>
    <td>Prevent fork users from voting on their upstream PRs</td><td>Repos</td><td>2022</td></tr>
    </tr>   
    <td rowspan="3"><a href="2021/sprint-191-update.md" data-raw-source="[19 August 2021](2021/sprint-191-update.md)">19 August 2021</a></td>
    <td>Improve web experience to better handle re-authentication requests</td><td>General</td><td>N/A</td></tr>
    <td>Improvements to Delivery Plans</td><td>Boards</td><td>2022</td></tr>
    <td>Support for environment variables in Linux Scale Set agents</td><td>Pipelines</td><td>N/A</td></tr>
    </tr>   
    <td rowspan="5"><a href="2021/sprint-190-update.md" data-raw-source="[4 August 2021](2021/sprint-190-update.md)">29 July 2021</a></td>
    <td>Display correct persona on commit links</td><td>Boards</td><td>2022</td></tr>
    <td>Support queuing or serial deployments as an option in exclusive lock check</td><td>Pipelines</td><td>2022</td></tr>
    <td>Support for Quebec version of ServiceNow</td><td>Pipelines</td><td>2022</td></tr>
    <td>Change in .NET SDK preinstallation policy on Microsoft hosted Windows and macOS agents</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Changes to PublishBuildArtifacts and DownloadBuildArtifacts tasks</td><td>Pipelines</td><td>N/A</td></tr>
    </tr>    
    <td rowspan="6"><a href="2021/sprint-188-update.md" data-raw-source="[17 June 2021](2021/sprint-188-update.md)">17 June 2021</a></td>
    <td>Restrict personal access token (PAT) scope and lifespan via Azure AD tenant policy</td><td>General</td><td>N/A</td></tr>
    <td>Conditional access policy support for IPv6 traffic</td><td>General</td><td>N/A</td></tr>
    <td>Retain pipelines that are consumed in other pipelines</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Changes in the automatic creation of environments</td><td>Pipelines</td><td>2022</td></tr>
    <td>Remove Insights dialogue from Build Pipeline</td><td>Pipelines</td><td>2022</td></tr>
    <td>Updates to Team Foundation Version Control (TFVC) Windows Shell extension for Visual Studio 2019</td><td>Pipelines</td><td>N/A</td></tr>
    </tr>    
    <td rowspan="7"><a href="2021/sprint-187-update.md" data-raw-source="[26 May 2021](2021/sprint-187-update.md)">26 May 2021</a></td>
    <td>Delivery Plans 2.0 general availability</td><td>Board</td><td>2022</td></tr>
    <td>New iteration capacity REST API</td><td>Board</td><td>N/A</td></tr>
    <td>Copy Dashboard is now available in public preview</td><td>Board</td><td>2022</td></tr>
    <td>Change in .NET SDK preinstallation policy on Microsoft hosted Ubuntu agents</td><td>Pipelines</td><td>N/A</td></tr>
    <td>Permissions and checks on variable groups and secure files</td><td>Pipelines</td><td>2022</td></tr>
    <td>Preview of templates support in YAML editors</td><td>Pipelines</td><td>2022</td></tr>
    <td>Ubuntu-16.04 will be removed from Microsoft-hosted pools in September 2021</td><td>Pipelines</td><td>N/A</td></tr>
    </tr>
    <td rowspan="4"><a href="2021/sprint-186-update.md" data-raw-source="[05 May 2021](2021/sprint-186-update.md)">05 May 2021</a></td>
    <td>PAT lifecycle management API general availability</td><td>General</td><td>N/A</td></tr>
    <td>Fixed several issues with Delivery Plans 2.0</td><td>Board</td><td>2022</td></tr>
    <td>Repos as a protected resource in YAML pipelines</td><td>Pipelines</td><td>2022</td></tr>
    <td>Enable empty recycle bin for feeds</td><td>Artifacts</td><td>N/A</td></tr>
    </tr>
    <td rowspan="2"><a href="2021/sprint-185-update.md" data-raw-source="[13 April 2021](2021/sprint-185-update.md)">13 April 2021</a></td>
    <td>Delivery Plans 2.0 Dependency tracking cleanup</td><td>Boards</td><td>2022</td></tr>
    </tr>
    <tr><td>Display custom work item types in burndown widget</td><td>Reporting</td><td>2022</td></tr>
    <tr>
    <td rowspan="6"><a href="2021/sprint-184-update.md" data-raw-source="[23 March 2021](2021/sprint-184-update.md)">23 March 2021</a></td>
    <td>Changes to Azure Pipelines free grants</td><td>Pipelines</td><td>N/A</td></tr>
    </tr>
    <tr><td>Removal of per-pipeline retention policies in classic builds</td><td>Pipelines</td><td>2022</td></tr>
    <tr><td>New controls for environment variables in pipelines</td><td>Pipelines</td><td>2022</td></tr>
    <tr><td>Generate unrestricted token for fork builds</td><td>Pipelines</td><td>2022</td></tr>
    <tr><td>Change in Az, Azure, and Azure RM preinstalled modules</td><td>Pipelines</td><td>N/A</td></tr>
    <tr><td>Disable a repository</td><td>Repos</td><td>2022</td></tr>
    <tr>
    <td rowspan="7"><a href="2021/sprint-183-update.md" data-raw-source="[03 March 2021](2021/sprint-183-update.md)">03 March 2021</a></td>
    <td>Limit user visibility and collaboration to specific projects</td><td>General</td><td>N/A</td></tr>
    </tr>
    <tr><td>Hide Organization Settings</td><td>General</td><td>N/A</td></tr>
    <tr><td>Token management events now in Audit Logs</td><td>General</td><td>N/A</td></tr>
    <tr><td>PAT lifecycle management API (private preview)</td><td>General</td><td>N/A</td></tr>
    <tr><td>Approver details available in audit logs</td><td>Pipelines</td><td>N/A</td></tr>
    <tr><td>Change in process for obtaining free pipelines grant in public projects</td><td>Pipelines</td><td>N/A</td></tr>
    <tr><td>Changes to Azure Artifacts upstream behavior</td><td>Artifacts</td><td>N/A</td></tr>
    <tr>
    <td rowspan="5"><a href="2021/sprint-182-update.md" data-raw-source="[04 February 2021](2021/sprint-182-update.md)">04 February 2021</a></td>
    <td>Limited people-picker search and tagging</td><td>General</td><td>N/A</td>
    </tr>
    <tr><td>Removed items on work items hub</td><td>Boards</td><td>2022</td></tr>
    <tr><td>Delivery Plans 2.0: Increase team limit to 15</td><td>Boards</td><td>2022</td></tr>
    <tr><td>.NET Core 3.0 to be removed from Linux and macOS hosted agents</td><td>Pipelines</td><td>N/A</td></tr>
    <tr><td>Group By Tags available in chart widgets</td><td>Reporting</td><td>2022</td></tr>
    <tr>
    <td rowspan="4"><a href="2021/sprint-181-update.md" data-raw-source="[14 January 2021](2021/sprint-181-update.md)">14 January 2021</a></td>
    <td>Delivery Plans: Rollup Information</td><td>Boards</td><td>2022</td>
    </tr>
    <tr><td>Delivery Plans: Condensed views</td><td>Boards</td><td>2022</td></tr>
    <tr><td>"uses" statement for pre-declaring resources</td><td>Pipelines</td><td>N/A</td></tr>
    <tr><td>Manual Validation for YAML pipelines</td><td>Pipelines</td><td>N/A</td></tr>
    <tr>
    <td rowspan="10"><a href="2020/sprint-179-update.md" data-raw-source="[03 December 2020](2020/sprint-179-update.md)">03 December 2020</a></td>
    <td>Single-click to toggle between inline and diff views</td><td>Repos</td><td>Future</td>
    </tr>
    <tr><td>Navigation to parent commits</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Preserve scroll position when resizing diff pane in PR files tab</td><td>Repos</td><td>Future</td></tr>
    <tr><td>New Test Plans page general availability</td><td>Test Plans</td><td>Future</td></tr>
    <tr><td>Search for a commit on a mobile device</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Improved usage of space for new PR file diff mobile view</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Enhanced images in PR summary view</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Enhanced branch experience when creating a new PR</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Historical graph for agent pools (Preview)</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>ServiceNow change management integration with YAML pipelines</td><td>Pipelines</td><td>Future</td></tr>
    <tr>
    <td rowspan="4"><a href="2020/sprint-178-update.md" data-raw-source="[12 November 2020](2020/sprint-178-update.md)">12 November 2020</a></td>
    <td>Removed items on the Work Items page</td><td>Boards</td><td>2020.1</td>
    </tr>
    <tr><td>Delivery Plans (Preview)</td><td>Boards</td><td>2022</td></tr>
    <tr><td>Improve YAML conversion in the classic build designer</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>New Test Plans page general availability</td><td>Test Plans</td><td>Future</td></tr>
    <tr>
    <td rowspan="4"><a href="2020/sprint-177-update.md" data-raw-source="[22 October 2020](2020/sprint-177-update.md)">22 October 2020</a></td>
    <td>Removing "Assigned To" rule on Bug work item type</td><td>Boards</td><td>2020.1</td>
    </tr>
    <tr><td>A batch of improvements to the Pull Request experience</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Node 14 in the Azure Pipelines agent</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Save an unhealthy agent for investigation in scale set agents</td><td>Pipelines</td><td>Future</td></tr>
    <tr>
    <td rowspan="5"><a href="2020/sprint-176-update.md" data-raw-source="[01 October 2020](2020/sprint-176-update.md)">01 October 2020</a></td>
    <td>Customize work item state when pull request is merged</td><td>Boards</td><td>Future</td>
    </tr>
    <tr><td>Parent field on the task board</td><td>Boards</td><td>2020.1</td></tr>
    <tr><td>Org-level setting for default branch</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Add a new auth scope for contributing PR comments</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Configure draft PR validation for GitHub repositories</td><td>Pipelines</td><td>Future</td></tr>
    <tr>
    <td rowspan="8"><a href="2020/sprint-175-update.md" data-raw-source="[10 September 2020](2020/sprint-175-update.md)">10 September 2020</a></td>
    <td>Allow stakeholders to move work items across board columns</td><td>Boards</td><td>2020.1</td>
    </tr>
    <tr><td>Link your work item to builds in another project</td><td>Boards</td><td>2020.1</td></tr>
    <tr><td>Editing description (help text) on system fields</td><td>Boards</td><td>2020.1</td></tr>
    <tr><td>General availability of scale-set agents</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Run this job next</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Template expressions allowed in YAML resources block</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Control over automated task updates from Marketplace</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>The Test and Feedback extension is now available in the Microsoft Edge store</td><td>Test Plans</td><td>Future</td></tr>
    <tr>
    <td rowspan="13"><a href="2020/sprint-174-update.md" data-raw-source="[24 August 2020](2020/sprint-174-update.md)">24 August 2020</a></td>
    <td>System work item types on backlogs and boards</td><td>Boards</td><td>2020.1</td>
    </tr>
    <tr><td>Audit logging event</td><td>Boards</td><td>Future</td></tr>
    <tr><td>Azure Boards GitHub app repo limit raised</td><td>Boards</td><td>2020.1</td></tr>
    <tr><td>Customize work item state when pull request is merged</td><td>Boards</td><td>2020.1</td></tr>
    <tr><td>Pipelines images announcements</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Agent log uploads improved</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Optionally mount container volumes read-only</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Fine-grained control over container start/stop</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Unzip task bundles for each step</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Improve release security by restricting scope of access tokens</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>YAML preview API enhancements</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Configure upstream sources for Universal Packages</td><td>Artifacts</td><td>Future</td></tr>
    <tr><td>Update Package Version REST API now available for Maven packages</td><td>Artifacts</td><td>Future</td></tr>
    <tr>
    <td rowspan="5"><a href="2020/sprint-173-update.md" data-raw-source="[03 August 2020](2020/sprint-173-update.md)">03 August 2020</a></td>
    <td>Allow stakeholders to drag and drop work items</td><td>Boards</td><td>Future</td>
    </tr>
    <tr><td>Default branch name preference</td><td>Repos</td><td>Future</td></tr>
    <tr><td>Updates to macOS 10.14 (Mojave) image </td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>[Feedback] Git Draft Pull Requests should not trigger the pipeline</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Multi-repo triggers for Azure Repos</td><td>Pipelines</td><td>Future</td></tr>
    <tr>
    <td rowspan="9"><a href="2020/sprint-172-update.md" data-raw-source="[10 July 2020](2020/sprint-172-update.md)">10 July 2020</a></td>
    <td>State transition restriction rules</td><td>Boards</td><td>2020.1</td>
    </tr>
    <tr><td>Copy work item to copy children</td><td>Boards</td><td>2020.1</td></tr>
    <tr><td>Improved rules for activated and resolved fields</td><td>Boards</td><td>2020.1</td></tr>
    <tr><td>System work item types on backlogs and boards (private preview)</td><td>Boards</td><td>Future</td></tr>
    <tr><td>Exclusive deployment lock policy</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Stages filters for pipeline resource triggers</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Generic webhook based triggers for YAML pipelines</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>YAML resource trigger issues support and traceability</td><td>Pipelines</td><td>Future</td></tr>
    <tr><td>Ability to create org-scoped feeds from UI</td><td>Artifacts</td><td>Future</td></tr>
    <tr>
    <td rowspan="5"><a href="2020/sprint-171-update.md" data-raw-source="[18 June 2020](2020/sprint-171-update.md)">18 June 2020</a></td>
        <td>Restrict new user invitations from Project and Team Administrators</td><td>General</td><td>2020.1</td>
    </tr>
    <tr><td>State transition restriction rules (private preview)</td><td>Boards</td><td>TBD</td></tr>
    <tr><td>Tag filter support for pipeline resources</td><td>Pipelines</td><td>2020.1</td></tr>
    <tr><td>Additional agent platform: ARM64</td><td>Pipelines</td><td>2020.1</td></tr>
    <tr><td>Control which tasks are allowed in pipelines</td><td>Pipelines</td><td>2020.1</td></tr>
    <tr>
    <td rowspan="8"><a href="2020/sprint-170-update.md" data-raw-source="[28 May 2020](2020/sprint-170-update.md)">01 June 2020</a></td>
        <td>Add "Parent Work Item" filter to the task board and sprint backlog</td><td>Boards</td><td>2020</td>    
        </tr>
        <tr><td>Improve error handling experience –– required fields on Bug/Task</td><td>Boards</td><td>N/A</td></tr>
        <tr><td>Preview of scale set agents</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>GitHub packages support in YAML pipelines</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Ubuntu 20.04 in preview for Azure Pipelines hosted pools</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Notifications for disabled upstream sources</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>License expressions and embedded licenses</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Lightweight authentication tasks</td><td>Artifacts</td><td>2020</td></tr>
    <tr>
        <td rowspan="6"><a href="2020/sprint-169-update.md" data-raw-source="[11 May 2020](2020/sprint-169-update.md)">11 May 2020</a></td>
        <td>Pipelines YAML CD features now generally available</td><td>Pipelines</td><td>2020</td>
        </tr>
        <tr><td>Service connections new UI as default experience</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Role-based access for service connections</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Showing associated CD pipeline info in CI pipeline</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Cross-project sharing of service connections is now public</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Pipeline resource version picker in the create run dialogue</td><td>Pipelines</td><td>2020</td></tr>
    </tr>  
    <tr>
        <td rowspan="9"><a href="2020/sprint-168-update.md" data-raw-source="[4 May 2020](2020/sprint-168-update.md)">4 May 2020</a></td>
        <td>Azure DevOps now allows team admin(s) to create subscriptions from MS Teams & Slack</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>MS Teams & Slack notifications for Repos events</td><td>General</td><td>2020.1</td></tr>
        <tr><td>Add attachments while creating a pull request</td><td>Repos</td><td>2020.1</td></tr>
        <tr><td>New web platform conversion - Team Foundation Version Control Hubs</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Limit build service repos scope access</td><td>Pipeline</td><td>N/A</td></tr>
        <tr><td>Run conditional job depending on variables from prior stage</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Getting details at runtime about multiple repositories</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Multi stage pipelines GA</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Configure Deployment Strategies from Azure portal</td><td>Pipelines</td><td>N/A</td>
    </tr>    
       <tr>
            <td rowspan="10"><a href="2020/sprint-167-update.md" data-raw-source="[13 April 2020](2020/sprint-167-update.md)">13 April 2020</a></td>
            <td>Support for Team Admins to create subscriptions for messaging apps in Slack and Teams</td></td><td>General</td><td>2020</td>
        </tr>
        <tr><td>Multitenant support for Azure Boards, Repos and Pipelines app in Microsoft Teams</td></td><td>General</td><td>2020</td></tr>
        <tr><td>Sync GitHub Issues to Azure DevOps Work Items</td><td>Boards</td><td>2019</td></tr>
        <tr><td>Improved PR actionability</td><td>Repos</td><td>2020.1</td></tr>
        <tr><td>Improved comment-related filtering within pull requests</td><td>Repos</td><td>2020.1</td></tr>
        <tr><td>Add built-in checks & extensibility using marketplace extensions</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Approval notification</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Accessibility improvements</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Auditing events are now available</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>npm performance improvements</td><td>Artifacts</td><td>N/A</td></tr>
        <tr>
            <td rowspan="4"><a href="2020/sprint-166-update.md" data-raw-source="[9 March 2020](2020/sprint-166-update.md)">16 March 2020</a></td>
            <td>Pay for users once across multiple organizations</td><td>General</td><td>2020</td>
        </tr>
        <tr><td>Assign a new owner to your orphaned organization</td><td>General</td><td>2020</td></tr>
        <tr><td>Runtime parameters</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Agent diagnostics</td><td>Pipelines</td><td>2020</td></tr>
        <tr>
        <tr>
            <td rowspan="5"><a href="2020/sprint-165-update.md" data-raw-source="[17 February 2020](2020/sprint-163-update.md)">17 February 2020</a></td>
            <td>Disable Request Access policy</td><td>General</td><td>Future</td>
        </tr>
        <tr><td>Preview fully parsed YAML document without running the pipeline</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Disable automatic agents upgrades at a pool level</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Azure File Copy Task now supports AzCopy V10</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Custom notification subscription for draft pull requests</td><td>Repos</td><td>2020</td></tr>
        <tr>
            <td rowspan="5"><a href="2020/sprint-164-update.md" data-raw-source="[28 January 2020](2020/sprint-164-update.md)">28 January 2020</a></td>
            <td>Restrict organization creation via Azure AD tenant policy</td><td>General</td><td>Future</td>
        </tr>
        <tr><td>Read-only variables</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Support for output variables in deployment job</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Avoid rollback of critical changes</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Removing older images in Azure Pipelines hosted pools</td><td>Pipelines</td><td>Future</td></tr>
        <tr>
            <td rowspan="7"><a href="2020/sprint-163-update.md" data-raw-source="[13 January 2020](2020/sprint-163-update.md)">13 January 2020</a></td>
            <td>Get compact and organized notifications in the Microsoft Teams app from Azure Boards, Azure Pipelines and Azure Repos</td><td>General</td><td>N/A</td>
        </tr> 
        <tr><td>Delete bulk subscriptions created in a Microsoft Teams or Slack channel</td><td>General</td><td>N/A</td></tr>
        <tr><td>Use pipeline decorators to inject steps automatically in a deployment job</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Allow repository references to other Azure Repos organizations</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Step targeting and command isolation</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Builds and releases auditing</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Enhancements to evaluate artifacts checks policy in pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr>
            <td rowspan="12"><a href="2019/sprint-162-update.md" data-raw-source="[16 December 2019](2019/sprint-162-update.md)">16 December 2019</a></td>
            <td>New web platform conversion landing pages</td><td>Repos</td><td>2020</td>
        </tr> 
        <tr><td>Support for Kotlin language</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Updated multi-stage pipelines UI</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>VSTest TestResultsDirectory option is available in the task UI</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Use extends keyword in pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Markdown support in automated test error messages</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Collect automatic and user-specified metadata from pipeline</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updates to service connections UI</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>VM deployments with Environments</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Skipping stages in a YAML pipeline</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Inline sprint burndown thumbnail</td><td>Reporting</td><td>2020</td></tr>
        <tr><td>Create a dashboard without a team</td><td>Reporting</td><td>2020</td></tr>
        <tr>
            <td rowspan="8"><a href="2019/sprint-161-update.md" data-raw-source="[2 December 2019](2019/sprint-161-update.md)">2 December 2019</a></td>
            <td>Use publish profile to deploy Azure WebApps for Windows from the Deployment Center</td><td>General</td><td>2020</td>
        </tr>
        <tr><td>Checkout multiple repositories in Azure Pipelines</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Use GitHub Actions to trigger a run in Azure Pipelines</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Updated ServiceNow integration with Azure Pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Set VSTest tasks to fail if a minimum number of tests are not run</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>UCS-4 support for Python 2.7</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Create bulk subscriptions in Azure Pipelines app for Slack and Microsoft Teams</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Create bulk subscriptions in Azure Repos app for Slack and Microsoft Teams</td><td>Repos</td><td>N/A</td></tr>
        <tr>
            <td rowspan="23"><a href="2019/sprint-160-update.md" data-raw-source="[4 November 2019](2019/sprint-160-update.md)">4 November 2019</a></td>
            <td>Cross-repo branch policy administration</td><td>Repos</td><td>2020</td>
        </tr>
        <tr><td>Multi-stage pipelines UX</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Orchestrate canary deployment strategy on environment for Kubernetes</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Approval policies for YAML pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>ACR as a first-class pipeline resource</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Pipeline resource meta-data as predefined variables</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Traceability for pipelines and ACR resources</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Simplified resource authorization in YAML pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Improve pipeline security by restricting the scope of access tokens</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Evaluate artifact check</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Markdown support in automated test error messages</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Diagnosing cron schedules in YAML</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updates to the ARM template deployment task</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Project level security for service connections</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Ubuntu 18.04 pool</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Service Mesh Interface based canary deployments in KubernetesManifest task</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>ReviewApp in Environment</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updated Connect to feed experience</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Public feeds are now generally available with upstream support</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Create project-scoped feeds from the portal</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>A Sprint Burndown widget with everything you've been asking for</td><td>Reporting</td><td>2020</td></tr>
        <tr><td>Synchronous scroll for editing wiki pages</td><td>Wiki</td><td>2020</td></tr>
        <tr><td>Page visits for wiki pages</td><td>Wiki</td><td>2020</td></tr>
        <tr>
            <td rowspan="17"><a href="2019/sprint-159-update.md" data-raw-source="[14 October 2019](2019/sprint-159-update.md)">14 October 2019</a></td>
            <td>Azure Boards app for Microsoft Teams</td><td>Boards</td><td>N/A</td>
        </tr>
        <tr><td>Import work items from a CSV file</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Add parent field to work item cards</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Add parent field to backlog and queries</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Quick navigation in Azure Boards search</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Azure Repos app for Microsoft Teams</td><td>Repos</td><td>N/A</td></tr>
        <tr><td>Mark files as reviewed in a pull request</td><td>Repos</td><td>2020</td></tr>
        <tr><td>New Web UI for Azure Repos landing pages (preview)</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Proximity support for code search</td><td>Repos</td><td>Future</td></tr>
        <tr><td>Deploy Azure Resource Manager (ARM) to subscription and management group level</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>CD capabilities for your multi-stage YAML pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Bitbucket integration and other improvements in getting started with pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Support for PowerShell scripts in Azure CLI task</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Search for wiki pages across accounts</td><td>Wiki</td><td>Future</td></tr>
        <tr><td>Access recently visited wiki pages</td><td>Wiki</td><td>Future</td></tr>
        <tr><td>Instant search for wiki</td><td>Wiki</td><td>Future</td></tr>
        <tr>
            <td rowspan="21"><a href="2019/sprint-158-update.md" data-raw-source="[23 September 2019](2019/sprint-1578-update.md)">23 September 2019</a></td>
            <td>User assignment-based billing and default access level</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>New UI to manage organization and project permissions</td><td>General</td><td>2020</td></tr>
        <tr><td>New rule to hide fields in a work item form based on condition</td><td>Boards</td><td>2020</td></tr>  
        <tr><td>Custom work item notification settings</td><td>Boards</td><td>2020</td></tr>  
        <tr><td>Link work items to deployments</td><td>Boards</td><td>2020</td></tr>  
        <tr><td>Use service account based authentication to connect to AKS</td><td>Repos</td><td>2020</td></tr>  
        <tr><td>Preview Markdown files in pull request Side-by-side diff</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Build policy expiration for manual builds</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Retry failed stages</td><td>Pipelines</td><td>2020</td></tr>  
        <tr><td>Enhancements to approvals in YAML pipelines</td><td>Pipelines</td><td>2020</td></tr>  
        <tr><td>Container structure testing support in Azure Pipelines</td><td>Pipelines</td><td>2020</td></tr>  
        <tr><td>Flaky bug management and resolution</td><td>Pipelines</td><td>2020</td></tr>  
        <tr><td>Enhancements to Azure Pipelines app for Slack and Microsoft Teams</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>N/A</td></tr>  
        <tr><td>Open Policy Agent installer task</td><td>Pipelines</td><td>2020</td></tr>  
        <tr><td>Pipeline decorators for release pipelines</td><td>Pipelines</td><td>2020</td></tr>  
        <tr><td>New Test Plans page</td><td>Test Plans</td><td>2020</td></tr>  
        <tr><td>Support for custom fields in Rollup columns</td><td>Reporting</td><td>2020</td></tr> 
        <tr><td>Inline sprint burndown using story points</td><td>Reporting</td><td>2020</td></tr> 
        <tr><td>Short and readable Wiki page URLs</td><td>Wiki</td><td>2020</td></tr> 
        <tr><td>Mermaid diagram support in wiki</td><td>Wiki</td><td>Future</td></tr>   
        <tr>
            <td rowspan="20"><a href="2019/sprint-157-update.md" data-raw-source="[3 September 2019](2019/sprint-157-update.md)">3 September 2019</a></td>
            <td>Get personalized notifications with @mention support in Slack apps</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>Download a list of organizations to a directory</td><td>General</td><td>2020</td></tr>      
        <tr><td>Track the progress of parent items using Rollup on Boards backlog</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Taskboard live updates</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Policy to block files with specified patterns</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Resolve work items via commits using key words</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Granularity for automatic reviewers</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Get latest Universal Package with Semantic Versioning (SemVer) wildcard</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Azure Artifacts feeds in the Visual Studio Package Manager</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Create Azure Pipelines from VS Code</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>New task for configuring Azure App Service app settings</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Azure App Service now supports Swap with preview</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>YAML templates for Python and .NET Functions apps</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Service hooks for YAML pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Enhancement to Azure Pipelines app for Jira</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>GitHub release task enhancements</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Stage level filter for Azure Container Registry and Docker Hub artifacts</td><td>Pipelines</td><td>2020</td></tr>            
        <tr><td>Sovereign cloud support in Kubernetes service connection</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Lead and Cycle Time widgets advanced filtering</td><td>Reporting</td><td>2020</td></tr>
        <tr>
            <td rowspan="27"><a href="2019/sprint-156-update.md" data-raw-source="[12 August 2019](2019/sprint-156-update.md)">12 August 2019</a></td>
            <td>New UI to request access to an organization</td><td>General</td><td>2020</td>
        </tr>
        <tr><td>Read-only and required rules for group membership</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Customize system picklist values</td><td>Boards</td><td>2020</td></tr>
        <tr><td>New work item URL parameter</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Mention people, work items and PRs in text fields</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Reactions on discussion comments</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Pin Azure Boards reports to the dashboard</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Azure Repos app for Slack</td><td>Repos</td><td>N/A</td></tr>
        <tr><td>Configure upstreams in different organizations within an Azure AD tenant</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Use Python Credential Provider to authenticate pip and twine with Azure Artifacts feeds</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Pipelines caching improvements</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Increase in gates timeout limit and frequency</td><td>Pipelines</td><td>2020</td></tr>    
        <tr><td>New build image template for Dockerfile</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Arguments input in Docker Compose task</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Fix warning in large test attachments</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Support for Bitbucket repositories in Deployment Center for AKS and Web App for containers</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Linux Web App support for Java workflows in Azure DevOps Projects</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Pipeline variable group and variable management commands</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Run pipeline for a PR branch</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Skip the first pipeline run</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Service endpoint command enhancement</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Test Plan progress report (public preview)</td><td>Test Plans</td><td>2020</td></tr>
        <tr><td>Enhancement to Test Plans page</td><td>Test Plans</td><td>2020</td></tr>
        <tr><td>Improvement to the Query Results widget</td><td>Reporting</td><td>2020</td></tr>
        <tr><td>Comments in wiki pages</td><td>Wiki</td><td>2020</td></tr>
        <tr><td>Hide folders and files starting with "." in wiki tree</td><td>Wiki</td><td>2020</td></tr>
        <tr>
            <td rowspan="29"><a href="2019/sprint-155-update.md" data-raw-source="[22 July 2019](2019/sprint-155-update.md)">22 July 2019</a></td>
            <td>Invite GitHub collaborators into Azure DevOps</td><td>General</td><td>2020</td>
        </tr>
        <tr><td>Get insights into your team's health with three new Azure Boards Analytics reports</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Azure Boards app for Slack</td><td>Boards</td><td>N/A</td></tr>
        <tr><td>Customize taskboard columns</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Toggle to show or hide completed child work items on the backlog</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Search for boards, backlogs, queries, and sprint from the instant search box</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Most recent tags displayed when tagging a work item</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Improved code search filtering options</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Share your packages publicly with public feeds (preview)</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Code coverage metrics and branch policy for pull requests</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Filter comment notifications from pull requests</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Service hooks for pull request comments</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Approvals in multi-stage YAML pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Manage pipeline variables in YAML editor</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>New predefined variables in YAML pipeline</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Cancel stage in a multi-stage YAML pipeline run</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Show correct pool information on each job</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Link work items with multi-stage pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>CI triggers for new branches</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Pipeline caching (public preview)</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Single hosted pool</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>kustomize and kompose as bake options in KubernetesManifest task</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Support for cluster admin credentials in HelmDeploy task</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>In-product support for flaky test management</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Improvements to the Deployment Center for WebApp in the Azure portal</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Enhancements to DevOps Project for virtual machine</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Terraform integration with Azure Pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Integration with Google Analytics</td><td>Pipelines</td><td>2020</td></tr>
        <tr>
            <td rowspan="28"><a href="2019/sprint-154-update.md" data-raw-source="[1 July 2019](2019/sprint-154-update.md)">1 July 2019</a></td>
            <td>Azure DevOps CLI general availability</td><td>General</td><td>2020</td>
        </tr>
        <tr><td>Work item live reload</td><td>General</td><td>2020</td></tr>
        <tr><td>Manage iteration and area paths from the command line</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Work item parent column as column option</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Instant search for work items</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Search for a work item as you type</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Change the process used by a project</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Hide custom fields from layout</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Azure Pipelines app for Jira</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Improvements to the Azure Pipelines app for Slack</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Add a GitHub release as an artifact source</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Updated Agent Pool interface in organization settings</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Single hosted pool</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Deployments in YAML pipeline</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Control variables that can be overridden at queue time</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Optimizely integration</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Support for large test attachments</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Pay for additional pipelines from the Azure DevOps portal</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Approve releases directly from Releases hub</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Azure Kubernetes Service Cluster link in Kubernetes environments resource view</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Release folder filters in notification subscriptions</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Deploy external Git repositories to Azure Kubernetes Services (AKS)</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Support for Bitbucket repositories in DevOps Projects</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Select a Dockerfile in deployment center for AKS and WebApp Containers</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>New Test Plan page public preview</td><td>Test Plans</td><td>2020</td></tr>
        <tr><td>Auditing for Azure Repos events</td><td>Repos</td><td>2020</td></tr>
        <tr><td>Rich editing for code wiki pages</td><td>Wiki</td><td>2020</td></tr>
        <tr><td>Create and embed work items from a wiki page</td><td>Wiki</td><td>2020</td></tr>
        <tr>
        <tr>
            <td rowspan="16"><a href="2019/sprint-153-update.md" data-raw-source="[10 June 2019](2019/sprint-153-update.md)">10 June 2019</a></td>
            <td>Changes to Azure DevOps IP address ranges</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>Auditing public preview</td><td>General</td><td>N/A</td></tr>
        <tr><td>Manage security groups and permissions from the command line</td><td>General</td><td>N/A</td></tr>
        <tr><td>Quickly view linked GitHub activity from the Kanban board</td><td>Boards</td><td>2019.1</td></tr>
        <tr><td>Copy work items with attachments and links</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Preview text files on work item</td><td>Boards</td><td>2020</td></tr>
        <tr><td>See all teams in Boards, Backlogs, and Sprints pickers</td><td>Boards</td><td>2020</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>A simpler way to work with artifacts</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Use cron syntax to specify schedules in a YAML file</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Updates to multi-stage pipelines public preview</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Go get command support in Azure Repos</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Filtered downloads for Universal Packages</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Package Search</td><td>Artifacts</td><td>2020</td></tr>
        <tr><td>Support for queries with tree of work items</td><td>Wiki</td><td>2019</td></tr>
        <tr><td>Top publisher certification program</td><td>Marketplace</td><td>N/A</td></tr>
        <tr>
        <tr>
            <td rowspan="15"><a href="2019/sprint-152-update.md" data-raw-source="[20 May 2019](2019/sprint-152-update.md)">20 May 2019</a></td>
            <td>Manage extensions from the command line</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>Invoke REST APIs from the command line</td><td>General</td><td>N/A</td></tr>
        <tr><td>Manage users from the command line</td><td>General</td><td>N/A</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Create and manage pipelines from a command line</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Manage build tags from the command line</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Share test run results via URL</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Filter by target branch in pull requests (PR)</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Allow extensions to add syntax highlighting and autocomplete</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Manage git references from the command line</td><td>Repos</td><td>N/A</td></tr>
        <tr><td>Update repository name and default branch from the command line</td><td>Repos</td><td>N/A</td></tr>
        <tr><td>Manage artifacts in a pipeline run from the command line</td><td>Artifacts</td><td>N/A</td></tr>
        <tr><td>New modern user experience</td><td>Wiki</td><td>2019</td></tr>
        <tr><td>Support for HTML tags</td><td>Wiki</td><td>2019.1</td></tr>
        <tr><td>Improved table creation and editing</td><td>Wiki</td><td>2019</td></tr>
        <tr>
        <tr>
            <td rowspan="6"><a href="2019/build-may.md" data-raw-source="[13 May 2019](2019/build-may.md)">13 May 2019</a></td>
            <td>Signing into Azure DevOps using your GitHub credentials</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>Kubernetes integration for Azure Pipelines</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Multi-stage YAML pipelines</td><td>Pipelines</td><td>2020</td></tr>
        <tr><td>Pay-per-GB</td><td>Artifacts</td><td>N/A</td></tr>
        <tr><td>General availability of Python and Universal Packages</td><td>Artifacts</td><td>Future</td></tr>
        <tr><td>A simpler way to buy Azure DevOps</td><td>Administration</td><td>N/A</td></tr>
        <tr><br/>        <tr>
            <td rowspan="7"><a href="2019/sprint-151-update.md" data-raw-source="[30 April 2019](2019/sprint-151-update.md)">30 April 2019</a></td>
            <td>Add Azure Boards from the GitHub Marketplace</td><td>Boards</td><td>N/A</td>
        </tr>
        <tr><td>Accept and execute on issues in GitHub while planning in Azure Boards</td><td>Boards</td><td>2019.1</td></tr>
        <tr><td>Taskboard people switcher</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Repository creation extension point</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Improved encoding support</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Azure Pipelines app for Microsoft Teams</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Updates to pipeline creation experience</td><td>Pipelines</td><td>Future</td></tr>
        <tr><br/>        <tr>
            <td rowspan="26"><a href="2019/sprint-150-update.md" data-raw-source="[8 April 2019](2019/sprint-150-update.md)">8 April 2019</a></td>
            <td>Dark theme general availability</td><td>General</td><td>2019.1</td>
        </tr>
        <tr><td>Query work based on Azure Active Directory groups</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Share your team's board using a badge</td><td>Boards</td><td>2019.1</td></tr>
        <tr><td>Query for work relative to the start of the day, week, month, or year</td><td>Boards</td><td>2019.1</td></tr>
        <tr><td>Export query results to a CSV file</td><td>Boards</td><td>2019.1</td></tr>
        <tr><td>New merge types for completing pull requests</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Kubernetes manifest task</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Upgrades to Docker task</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Kubectl tool installer</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Azure Container Registry in Docker registry service connection</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>cgroup support on hosted Ubuntu pool</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Run once agent</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Support for Visual Studio 2019 (VS2019) in Visual Studio test task</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Agent pool user interface update</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Task assistant for editing YAML files</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Hosted pipelines image updates</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Improvements to ServiceNow integration</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Support for Azure PowerShell Az module</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Resource authorization improvements</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Simplified retention policies for build pipelines</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Pipeline artifacts fetched automatically in release</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Cobertura code coverage report updates</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Build failure and duration reports</td><td>Reporting</td><td>Future</td></tr>
        <tr><td>General availability of Analytics</td><td>Reporting</td><td>2019</td></tr>
        <tr><td>Notifications on wiki pages</td><td>Wiki</td><td>2019.1</td></tr>
        <tr><td>Manage billing for your organization from Azure DevOps</td><td>Administration</td><td>Future</td></tr>
        <tr>
            <td rowspan="16"><a href="2019/sprint-149-update.md" data-raw-source="[19 March 2019](2019/sprint-149-update.md)">19 March 2019</a></td>
            <td>Navigate to Azure Boards work items directly from mentions in any GitHub comment</td><td>Boards</td><td>2019.1</td>
        </tr>
        <tr><td>Updates to work item transition rules</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Azure Boards GitHub Enterprise support</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Edit and delete comments in work item</td><td>Boards</td><td>2019.1</td></tr>
        <tr><td>State value order on work item form</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Choose the directory of checked out code in YAML pipelines</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Private projects now get 60 minutes of run time per pipeline job</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Updates to hosted pipeline images</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Duffle tool installer task in build and release pipeline</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Approve Azure Pipelines deployments from Slack</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>All source providers included in the new build pipeline wizard</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>GitHub comments trigger optimizations</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Publish CTest and PHPUnit test results</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Upstream sources for Maven</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td>Analytics services OData version change for test entity sets</td><td>Reporting</td><td>Future</td></tr>
        <tr><td>Resolve Azure Active Directory (Azure AD) disconnected users</td><td>Administration</td><td>Future</td></tr>
        <tr>
            <td rowspan="21"><a href="2019/sprint-148-update.md" data-raw-source="[25 February 2019](2019/sprint-148-update.md)">25 February 2019</a></td>
            <td>Azure DevOps CLI extension</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>Navigate to Azure Boards work items directly from GitHub pull request mentions</td><td>Boards</td><td>2019.1</td></tr>
        <tr><td>Deploy your local Git web apps for Windows, Linux, and Containers to Azure</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>New Azure subscription option in Kubernetes service connection</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Notifications on failure of a release creation request</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Azure Pipelines app for Slack</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Skip continuous integration (CI) for a commit</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Updates to hosted pipelines images</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Contribution point for variables in the create release dialog</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Support for Python Function Apps in DevOps Projects</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Schedule releases on source or pipeline change</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Build and release log viewer enhancements</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Publish to Azure Service Bus session queues</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Search by folder name in release definitions</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Simplified publishing of test results</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Azure Active Directory device code authentication flow for pipelines agent</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Support for Red Hat Enterprise Linux 6</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>All Artifacts package types supported in releases</td><td>Artifacts</td><td>Future</td></tr>
        <tr><td>Artifacts views supported in releases</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td>Retention policies can skip packages downloaded recently</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td><xref href="mention" data-throw-if-not-resolved="False" data-raw-source="@mention"></xref> users and groups</td><td>Wiki</td><td>2019.1</td></tr>
        <tr>
            <td rowspan="15"><a href="2019/sprint-147-update.md" data-raw-source="[04 February 2019](2019/sprint-147-update.md)">04 February 2019</a></td>
            <td>Show work item status in #ID mentions</td><td>Boards</td><td>Future</td>
        </tr>
        <tr><td>View just the left or right file in a pull request</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Restore deleted release pipelines</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>YAML files for a new pipeline are committed by your identity, not our bot</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Create pipelines from an existing YAML file in any branch or path</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Run pipelines using GitHub pull request comments</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Limit pull request validation builds to authorized team members</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Publish build artifacts with long file paths</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>New extension contribution points in the Pipelines Test tab</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Proxy support for Artifacts-related tasks</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td>Delegate who can manage feeds</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td>Test result trend widget</td><td>Reporting</td><td>2019.1</td></tr>
        <tr><td>Permalinks for wiki pages</td><td>Wiki</td><td>2019.1</td></tr>
        <tr><td>Show work item status in wiki pages</td><td>Wiki</td><td>2019.1</td></tr>
        <tr><td>All users now on New Navigation</td><td>Administration</td><td>N/A</td></tr>
        <tr>
            <td rowspan="27"><a href="2019/sprint-146-update.md" data-raw-source="[14 January 2019](2019/sprint-146-update.md)">14 January 2019</a></td>
            <td>Simplify the organization of your work using the Basic process</td><td>Boards</td><td>Future</td>
        </tr>
        <tr><td>GitHub Enterprise support in the pipeline wizard</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Automatic GitHub service connections in pipelines</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Display status for each pipeline job in GitHub Checks</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Default authorization for YAML resources in GitHub</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Service containers for YAML pipelines</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Work items linked to GitHub commit in Release Summary</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>New Azure App Service tasks optimized for YAML</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Azure AD authentication support for Azure SQL task</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Grafana annotations service hook</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Query Azure Monitor alerts tasks</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Inline input of spec file in Deploy to Kubernetes task</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Docker CLI Installer task</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Java long-term support (LTS) on Microsoft hosted agents</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>YAML support for Bitbucket Cloud pipelines</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Avoid triggering multiple CI builds for pull requests</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Change build numbers, upload, and download artifacts in forked repository builds</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>New option in &#39;Publish Test Results&#39; task to fail build on failed tests</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Updates to the Azure portal for creating an Azure DevOps project</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Use the Azure portal to set up and deploy to a Cosmos DB database</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Setup builds and release pipelines for Functions in Azure portal</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Package usage stats</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td>Monospaced font for Wiki markdown editor</td><td>Wiki</td><td>2019.1</td></tr>
        <tr><td>Bold Wiki page titles</td><td>Wiki</td><td>Future</td></tr>
        <tr><td>Insert Markdown table</td><td>Wiki</td><td>Future</td></tr>
        <tr><td>Embed Azure Boards query results in Wiki</td><td>Wiki</td><td>2019.1</td></tr>
        <tr><td>Restore deleted projects</td><td>Administration</td><td>N/A</td></tr>
        <tr>
            <td rowspan="14"><a href="2018/sprint-144-update.md" data-raw-source="[04 December 2018](2018/sprint-144-update.md)">04 December 2018</a></td>
            <td>Link GitHub commits and pull requests to Azure Boards work items</td><td>Boards</td><td>2019</td>
        </tr>
        <tr><td>Acquire Azure Boards as a service</td><td>Boards</td><td>N/A</td></tr>
        <tr><td>Rerun expired build for autocomplete pull requests</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Manage GitHub releases using pipelines</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>VS Code extension for YAML-based pipelines</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Web editor with IntelliSense for YAML pipelines</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>ServiceNow Change Management integration</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Links to specific lines in a build log</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Specify multi-platform pipeline in a single file</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Automatically redeploy on failure</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Python Package Index (PyPI) public preview</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td>Service health portal</td><td>General</td><td>N/A</td></tr>
        <tr><td>Markdown templates for formulas and videos</td><td>Wiki</td><td>2019.1</td></tr>
        <tr><td>Restore deleted projects</td><td>Administration</td><td>N/A</td></tr>
        <tr>
            <td rowspan="13"><a href="2018/sprint-143-update.md" data-raw-source="[12 November 2018](2018/sprint-143-update.md)">12 November 2018</a></td>
            <td>REST API version 5.0</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>New work item text editor</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Improved branch picker</td><td>Repos</td><td>2019</td></tr>
        <tr><td>Draft pull requests</td><td>Repos</td><td>2019.1</td></tr>
        <tr><td>Trigger YAML pipelines with tags</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Setting to auto cancel an existing pipeline when a pull request is updated</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Declare container resources inline</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Changes to default permissions for new projects</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Deploy to failed targets in a Deployment Group</td><td>Pipelines</td><td>2019.1</td></tr>
        <tr><td>Support for Infrastructure as Code</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Exclude files in artifact uploads</td><td>Artifacts</td><td>N/A</td></tr>
        <tr><td>Provenance information on packages</td><td>Artifacts</td><td>2019.1</td></tr>
        <tr><td>Azure Artifacts REST API documentation updates</td><td>Artifacts</td><td>N/A</td></tr>
        <tr>
            <td rowspan="20"><a href="2018/sprint-142-update.md" data-raw-source="[22 October 2018](2018/sprint-142-update.md)">22 October 2018</a></td>
            <td>New navigation is on for all users</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>Dark Theme</td><td>General</td><td>Future</td></tr>
        <tr><td>Organize reference materials with richer work item attachments</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Manage dependencies by linking work items across your Organizations</td><td>Boards</td><td>Future</td></tr>
        <tr><td>Open work items from search</td><td>Boards</td><td><em>2019</em></td></tr>
        <tr><td>Extension authors can query context about the current repo</td><td>Repos</td><td><em>2019</em></td></tr>
        <tr><td>Add custom build counters to your builds</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Use YAML to specify branches to build for pull requests</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Use YAML template expressions inline</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Improve troubleshooting with the pipeline initialization log</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Default retention for YAML pipelines</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Build on Linux/ARM and Windows 32-bit platforms</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Clone variable groups</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>See commits and work items for all linked sources</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Run from Package supported in Azure App Service deployments</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Deploy Linux containers with the App Server Deploy task</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Azure Test Runner runs manual tests for desktop applications</td><td>Test Plans</td><td><em>2019</em></td></tr>
        <tr><td>Public preview of Pipeline Artifacts</td><td>Artifacts</td><td><em>2019</em></td></tr>
        <tr><td>Publish code as wiki with Contribute permissions</td><td>Wiki</td><td><em>2019</em></td></tr>
        <tr><td>PATs enforce CAP</td><td>Administration</td><td>N/A</td></tr>
        <tr>
            <td rowspan="10"><a href="2018/sprint-141-update.md" data-raw-source="[1 October 2018](2018/sprint-141-update.md)">1 October 2018</a></td>
            <td>Azure Policy compliance and security validations in Pipelines</td><td>Pipelines</td><td><em>2019</em></td>
        </tr>
        <tr><td>Simplified continuous delivery to Azure VMs</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>The Xcode task supports newly released Xcode 10</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Performance improvements when queuing a build</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Create Azure service connection with service principal that authenticates with a certificate</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>View test analytics in Pipelines</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Change the target branch of a pull request</td><td>Repos</td><td><em>2019</em></td></tr>
        <tr><td>Protect Git repos with cross platform compatibility settings</td><td>Repos</td><td>N/A</td></tr>
        <tr><td>Expanded search box</td><td>General</td><td><em>2019</em></td></tr>
        <tr><td>Support Azure AD users in MSA accounts</td><td>Administration</td><td>N/A</td></tr>
        <tr>
            <td rowspan="10"><a href="2018/sprint-140-update.md" data-raw-source="[20 September 2018](2018/sprint-140-update.md)">20 September 2018</a></td>
            <td>Control-specific build dependencies using container jobs</td><td>Pipelines</td><td>Future</td>
        </tr>
        <tr><td>Enable code coverage in .NET Core task</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Leverage restructured Process REST APIs</td><td>Boards</td><td><em>2019</em></td></tr>
        <tr><td>Simplify authentication using the new cross-platform Credential Provider for NuGet</td><td>Artifacts</td><td><em>2019</em></td></tr>
        <tr><td>Store artifacts using Universal Packages</td><td>Artifacts</td><td>Future</td></tr>
        <tr><td>Compress symbols when publishing to a file share</td><td>Artifacts</td><td><em>2019</em></td></tr>
        <tr><td>Embed a video in wiki</td><td>Wiki</td><td><em>2019</em></td></tr>
        <tr><td>Rename a wiki</td><td>Wiki</td><td><em>2019</em></td></tr>
        <tr><td>Insert a wiki table of contents from the format pane</td><td>Wiki</td><td><em>2019</em></td></tr>
        <tr><td>Manage your personal access tokens with filtering and paging</td><td>Administration</td><td><em>2019</em></td></tr>
        <tr>
            <td rowspan="15"><a href="2018/sep-10-azure-devops-launch.md" data-raw-source="[10 September 2018](2018/sep-10-azure-devops-launch.md)">10 September 2018</a></td>
            <td>Azure DevOps Services</td><td>General</td><td>N/A</td>
        </tr>
        <tr><td>Add Azure Pipelines from the GitHub Marketplace</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Build open-source projects with Azure Pipelines for free</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Configure builds using YAML</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Create YAML build pipelines using the new wizard</td><td>Pipelines</td><td>Future</td></tr>
        <tr><td>Manage build pipelines using the new Builds page</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Rebuild GitHub pull request builds</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>New build status badge URL</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Leverage even more tools on Microsoft-hosted Linux agents</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Track GitHub commits and associated issues in releases</td><td>Pipelines</td><td>N/A</td></tr>
        <tr><td>Manage build and deployment completion emails better using improved formatting</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Follow the new unified Azure Pipelines terminology</td><td>Pipelines</td><td><em>2019</em></td></tr>
        <tr><td>Leverage the latest extension categories</td><td>Marketplace</td><td>N/A</td></tr>
        <tr><td>Switch existing organizations to use the new domain name URL</td><td>Administration</td><td>N/A</td></tr>
        <tr><td>Add Stakeholder users to save on Azure Pipelines license costs</td><td>Administration</td><td>N/A</td></tr>
        <tr>
            <td rowspan="6"><a href="2018/aug-21-vsts.md" data-raw-source="[21 August 2018](2018/aug-21-vsts.md)">21 August 2018</a></td>
            <td>Create table of contents for wiki pages</td><td>Wiki</td><td><em>2019</em></td>
        </tr>
        <tr><td>Ease customization by migrating projects to the Inheritance process model</td><td>Work</td><td>N/A</td></tr>
        <tr><td>Chat about the latest status using the improved Microsoft Teams integration</td><td>Work</td><td>2017.2</td></tr>
        <tr><td>Standardize pull request descriptions using templates</td><td>Code</td><td><em>2019</em></td></tr>
        <tr><td>Perform additional testing using a pull request release trigger</td><td>Build and Release</td><td><em>2019</em></td></tr>
        <tr><td>Deploy Go apps to Azure Kubernetes Service (AKS) using Azure DevOps Projects</td><td>Build and Release</td><td>N/A</td></tr>
        <tr>
            <td rowspan="9"><a href="2018/aug-03-vsts.md" data-raw-source="[3 August 2018](2018/aug-03-vsts.md)">3 August 2018</a></td>
            <td>Surface metadata for wiki pages and code preview using YAML tags</td><td>Wiki</td><td><em>2019</em></td>
        </tr>
        <tr><td>View work for your team in the Work Items hub</td><td>Work</td><td><em>2019</em></td></tr>
        <tr><td>Check installed software on Microsoft-hosted agent pools</td><td>Build and Release</td><td>N/A</td></tr>
        <tr><td>Review summarized test results</td><td>Test</td><td><em>2019</em></td></tr>
        <tr><td>View package download and user metrics</td><td>Package</td><td><em>2019</em></td></tr>
        <tr><td>Browse dependencies in npm packages</td><td>Package</td><td><em>2019</em></td></tr>
        <tr><td>View VSTS dashboards within Microsoft Teams</td><td>Reporting</td><td>N/A</td></tr>
        <tr><td>Investigate build history through a new build dashboard widget</td><td>Reporting</td><td><em>2019</em></td></tr>
        <tr><td>Manage billing for your organization directly through the Azure portal</td><td>Admin</td><td>N/A</td></tr>
        <tr>
            <td rowspan="14"><a href="2018/jul-10-vsts.md" data-raw-source="[10 July 2018](2018/jul-10-vsts.md)">10 July 2018</a></td>
            <td>Create pull requests without a default team as reviewer</td><td></td><td><em>2019</em></td>
        </tr>
        <tr><td>Allow bypassing branch policies without giving up push protection</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Link to headings within a page</td><td></td><td><em>2019</em></td></tr>
        <tr><td>View broken links</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Attach files and images in folders</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Open page in new tab</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Build and release with Microsoft-hosted Linux and macOS agents</td><td></td><td>N/A</td></tr>
        <tr><td>Azure DevOps Projects now generally available</td><td></td><td>N/A</td></tr>
        <tr><td>Automatically deploy to new targets in a deployment group</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Hold deployments until gates succeed consistently</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Get started with pre-installed Package Management</td><td></td><td>N/A</td></tr>
        <tr><td>Connect or disconnect Azure Active Directory as a Project Collection Admin</td><td></td><td>N/A</td></tr>
        <tr><td>Public projects available in preview for all organizations</td><td></td><td>N/A</td></tr>
        <tr><td>Adopt the word &quot;organization&quot; when referring to a collection of projects in VSTS</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="17"><a href="2018/jun-19-vsts.md" data-raw-source="[19 June 2018](2018/jun-19-vsts.md)">19 June 2018</a></td>
            <td>Preview our new navigation hub</td><td></td><td><em>2019</em></td>
        </tr>
        <tr><td>New Work hubs</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Queries hub generally available</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Easily find existing work items in linking and mention experiences</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Modernized experience in the Builds hub</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Pass environment variables to tasks</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Ignore a release gate for a deployment</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Set a variable at release time</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Organize your release definitions in folders</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Use improved Windows remote PowerShell based tasks</td><td></td><td><em>2019</em></td></tr>
        <tr><td>GitHub artifacts show associated commits deployed in a release</td><td></td><td>N/A</td></tr>
        <tr><td>Use upstream sources in legacy feeds</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Use arbitrary public npm feeds as upstream sources</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Improved experiences in the Test tab</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Exclude items completed before a certain date in analytics views</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Easily navigate to dashboards</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Get notified for PAT expirations</td><td></td><td><em>2019</em></td></tr>
        <tr>
            <td rowspan="11"><a href="2018/may-30-vsts.md" data-raw-source="[30 May 2018](2018/may-30-vsts.md)">30 May 2018</a></td>
            <td>Import and export Inherited Processes</td><td></td><td>Future</td>
        </tr>
        <tr><td>Customize column options in the Work Items hub</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Receive notifications when pull request policies are bypassed</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Favorite a branch from within a pull request</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Visualize release progress</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Run inline or file-based Python scripts in your pipeline</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Use Anaconda tools for data science in your pipeline</td><td></td><td>N/A</td></tr>
        <tr><td>Simplify definitions with multiple agentless tasks per phase</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Manage limits on self-hosted, concurrent CI/CD jobs</td><td></td><td>N/A</td></tr>
        <tr><td>Streamline authentication from agent VMs to Azure Resource Manager</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Guard your user account using alternate authentication notifications</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="15"><a href="2018/may-07-vsts.md" data-raw-source="[7 May 2018](2018/may-07-vsts.md)">7 May 2018</a></td>
            <td>Query for empty rich text fields</td><td></td><td><em>2019</em></td>
        </tr>
        <tr><td>Build Ruby apps based on a variety of Ruby versions</td><td></td><td>N/A</td></tr>
        <tr><td>Build, test, and publish Python apps based on a variety of Python versions</td><td></td><td>N/A</td></tr>
        <tr><td>Build Java apps on hosted agents with Java 10</td><td></td><td>N/A</td></tr>
        <tr><td>Leverage improved Xcode build and test output from xcpretty</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Progressively expose and phase deployments using release gates</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Deploy to Azure Kubernetes Service (AKS) and Azure Service Fabric using Azure DevOps Projects</td><td></td><td>N/A</td></tr>
        <tr><td>Deploy to Azure SQL Database using Azure DevOps Projects</td><td></td><td>N/A</td></tr>
        <tr><td>Release hybrid applications to Azure Stack</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Control Helm version used in Release</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Follow packages</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Control who can pull packages from upstream sources</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Change feed settings without having to manually save</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Manage test plans using the new Test Plans hub</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Fix broken links when moving pages</td><td></td><td><em>2019</em></td></tr>
        <tr>
            <td rowspan="15"><a href="2018/apr-16-vsts.md" data-raw-source="[16 Apr 2018](2018/apr-16-vsts.md)">16 Apr 2018</a></td>
            <td>Find phrases and code with special characters faster</td><td></td><td><em>2019</em></td>
        </tr>
        <tr><td>Query work in the Area Paths of a Team with the new <xref href="TeamAreas" data-throw-if-not-resolved="False" data-raw-source="@TeamAreas"></xref> macro</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Trigger CI builds from YAML</td><td></td><td>Future</td></tr>
        <tr><td>Continuously deploy to Azure Database for MySQL</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Streamline deployment to Kubernetes using Helm</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Deploy Ruby on Rails applications</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Configure Go and Ruby applications using Azure DevOps Projects</td><td></td><td>N/A</td></tr>
        <tr><td>Continuously deploy builds tagged by post-build processing</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Filter branches for GitHub Enterprise or external Git artifacts</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Subscribe to package update notifications</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Use upstream NuGet packages from elsewhere in VSTS</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Enable nuget.org upstream sources in more feeds</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Quickly link to other wiki pages using suggestions</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Filter search results by Wiki name</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Move a VSTS account between Azure subscription or resource group</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="12"><a href="2018/apr-03-vsts.md" data-raw-source="[3 Apr 2018](2018/apr-03-vsts.md)">3 Apr 2018</a></td>
            <td>Quickly describe pull requests using commit messages</td><td></td><td><em>2019</em></td>
        </tr>
        <tr><td>Perform TFVC commands right from Windows Explorer</td><td></td><td>N/A</td></tr>
        <tr><td>Chain related builds together using build completion triggers</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Scale deployments to VMs using Deployment Groups</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Build applications written in Go</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Extend release gates with task extensions</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Use upstream npm packages from elsewhere in VSTS</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Maintain feed query speed with retention policies</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Publish Markdown files from a Git repository as a Wiki</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Retain special characters in Wiki page titles</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Extend Wiki using REST APIs</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Integrate Power BI with VSTS Analytics using views</td><td></td><td><em>2019</em></td></tr>
        <tr>
            <td rowspan="13"><a href="2018/mar-05-vsts.md" data-raw-source="[5 Mar 2018](2018/mar-05-vsts.md)">5 Mar 2018</a></td>
            <td>Avoid overwrites and protect performance using repository settings</td><td></td>
            <td><em>2018.2</em></td>
        </tr>
        <tr><td>Focus on important work using the Work Items hub</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Query work across the iteration schedule with +/- <xref href="CurrentIteration" data-throw-if-not-resolved="False" data-raw-source="@CurrentIteration"></xref></td><td></td><td><em>2019</em></td></tr>
        <tr><td>Clarify query iteration schedules with the <xref href="CurrentIteration" data-throw-if-not-resolved="False" data-raw-source="@CurrentIteration"></xref> Team parameter</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Improve release times by partially downloading artifacts</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Retain more control of your app by deploying your Azure DevOps Project to a Virtual machine</td><td></td><td>N/A</td></tr>
        <tr><td>Improve code quality with the latest extensions from SonarSource</td><td></td><td>N/A</td></tr>
        <tr><td>Trace GitHub sources to builds using build tags</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Isolate Azure Resource Manager service endpoints to Resource Groups</td><td></td><td>N/A</td></tr>
        <tr><td>Manage entity-specific security</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Share deployment status using a badge</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Deploy selectively based on the artifact triggering a release</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Leverage your existing subscription using an Azure AD-based alternate email account</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="20"><a href="2018/feb-14-vsts.md" data-raw-source="[14 Feb 2018](2018/feb-14-vsts.md)">14 Feb 2018</a></td>
            <td>Recover a recently deleted repository via API</td><td></td>
            <td><em>2018.2</em></td>
        </tr>
        <tr><td>Discuss work items in Microsoft Teams using the VSTS messaging extension</td><td></td><td>N/A</td></tr>
        <tr><td>Mention a group in work item and pull request discussions</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Use VSTS as a symbol server</td><td></td><td>N/A</td></tr>
        <tr><td>Filter branches for GitHub artifacts</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Filter branches using include and exclude</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Release from Azure Container Registry and Docker Hub</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Propagate Jenkins artifacts to Azure Storage</td><td></td><td>N/A</td></tr>
        <tr><td>Specify a default version for Jenkins artifacts</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Scope a variable group to specific environments</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Install tasks from the Marketplace directly from the build or release definition</td><td></td><td>N/A</td></tr>
        <tr><td>Seamlessly use public packages using upstream sources</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>View quality of a package version in the package list</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Link to packages from anywhere</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Share your packages using a badge</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Recycle and restore packages</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Manage access and extensions for large numbers of users using groups</td><td></td><td>N/A</td></tr>
        <tr><td>Reduced latency for Azure AD group membership changes</td><td></td><td>N/A</td></tr>
        <tr><td>Manage users with Graph REST APIs Public Preview</td><td></td><td>N/A</td></tr>
        <tr><td>Leave account</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="22"><a href="2018/jan-24-vsts.md" data-raw-source="[24 Jan 2018](2018/jan-24-vsts.md)">24 Jan 2018</a></td>
            <td>View Analytics Widgets as a Stakeholder</td><td></td>
            <td><em>2019</em></td>
        </tr>
        <tr><td>Integrate Power BI with VSTS Analytics using new views</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Views pull request merge commit</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Help reviewers using pull request labels</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>View remaining policy criteria for pull request autocomplete</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Discuss math in pull requests</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Control who can contribute to pull requests</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Integrate using the pull request status API and branch policy</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Move work using suggested Areas and Iterations</td><td></td><td><em>2019</em></td></tr>
        <tr><td>Build GitHub pull requests from repository forks</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Build with continuous integration from GitHub Enterprise</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Build with the appropriate agent by default</td><td></td><td>N/A</td></tr>
        <tr><td>Screenshot desktop apps through the Chrome browser</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Filter large test results by Test Name</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Run Functional Tests and Deploy Test Agent tasks are now deprecated</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Wiki Search now Generally Available</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Print Wiki pages</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Contribute to Wiki pages with ease using keyboard shortcuts</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Calculate price without leaving the extension page</td><td></td><td>N/A</td></tr>
        <tr><td>Manage permissions directly on Azure AD groups</td><td></td><td>N/A</td></tr>
        <tr><td>Consider warning of single Project Collection Administrator</td><td></td><td>N/A</td></tr>
        <tr><td>Connect or disconnect a VSTS account to Azure Active Directory via new Azure portal</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="22"><a href="/previous-versions/azure/devops/2017/dec-11-vsts" data-raw-source="[11 Dec 2017](/previous-versions/azure/devops/2017/dec-11-vsts)">11 Dec 2017</a></td>
            <td>Track code pushes to a Git repo to builds and releases</td><td></td>
            <td><em>2018.2</em></td>
        </tr>
        <tr><td>Blame now has history</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>SSH URLs are changing</td><td></td><td>N/A</td></tr>
        <tr><td>Generate YAML templates from existing build definitions</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Enhancements to multi-phase build</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Hide empty contributed sections in build results page</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Skip scheduled builds if nothing has changed in the repo</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Run UI tests and install software on Hosted VS2017 agents</td><td></td><td>N/A</td></tr>
        <tr><td>ASP.NET Core 2.0 agents</td><td></td><td>N/A</td></tr>
        <tr><td>Release trigger for a Package Management artifact</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Default artifact versions</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Release triggers branch enhancements</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Filter large test results</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Identify flaky tests</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Pass parameters to your test run using. testsettings file</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Access information pertinent to test cases in your automated tests when running in the CI/CD pipeline</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Automated tests that use TestCase as a data source can now be run using the VSTest task</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Improved Marketplace experience</td><td></td><td>N/A</td></tr>
        <tr><td>Refreshed publisher management portal</td><td></td><td>N/A</td></tr>
        <tr><td>Virus scan of all public extensions on Marketplace</td><td></td><td>N/A</td></tr>
        <tr><td>TFX CLI changes for extension publish</td><td></td><td>N/A</td></tr>
        <tr><td>Cloud Solution Provider purchasing now generally available</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="44"><a href="/previous-versions/azure/devops/2017/nov-28-vsts" data-raw-source="[28 Nov 2017](/previous-versions/azure/devops/2017/nov-28-vsts)">28 Nov 2017</a></td>
            <td>Azure DevOps Project</td><td></td>
            <td>N/A</td>
        </tr>
        <tr><td>Configuration as code (YAML) builds in Public Preview</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Release gates in Public Preview</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Hosted Mac agents for CI/CD pipelines in Public Preview</td><td></td><td>N/A</td></tr>
        <tr><td>TFS Database Import Service now Generally Available</td><td></td><td>N/A</td></tr>
        <tr><td>VSTS CLI in Public Preview</td><td></td><td>N/A</td></tr>
        <tr><td>Query last run by information</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Create work items from the Queries hub</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Expand/collapse requirements/people on the Task board</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Grant the bypassrule permission to specific users</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Rendered Markdown in email notifications</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Pull request comment notifications include the thread context</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Pull request service hooks merge events</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Improved error messages for work items completing with a pull request</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Improved Azure Active Directory integration for pull requests</td><td></td><td>N/A</td></tr>
        <tr><td>Path filters for pull request policies</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Pull request suggestions for forks</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Editor settings</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Recently used reviewers</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>SSH: Support additional ciphers/keys and deprecate outdated ciphers</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Improved repository settings performance</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Use VSTS as a symbol server</td><td></td><td>N/A</td></tr>
        <tr><td>Agentless build tasks</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Apple provisioning profiles can be installed from source repositories</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Secure files can be downloaded to agents during build or release</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Specific Java Development Kits (JDKs) can be installed during builds and releases</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Improved Xcode build configuration</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Updates to the Hosted VS2017 pool</td><td></td><td>N/A</td></tr>
        <tr><td>Docker Hub or Azure Container Registry as an artifact source</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Enable Continuous Monitoring on Azure web apps</td><td></td><td>N/A</td></tr>
        <tr><td>Jenkins multi-branch pipeline support and link jobs organized in folders</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Jenkins work items in release for JIRA and VSTS Work Items</td><td></td><td>N/A</td></tr>
        <tr><td>Save packages from NuGet.org in your feed</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Maven supports now generally available</td><td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td></tr>
        <tr><td>Easier feed creation and editing</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Previous package versions are now a full-page list</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Promote, unlist, and deprecate multiple packages</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Wiki Search</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Link work items and Wiki pages</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Rich Markdown rendering in code repo Markdown</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Wiki supports mathematical formulas</td><td></td><td><em>2018.2</em></td></tr>
        <tr><td>Analytics OData in Public Preview</td><td></td><td>N/A</td></tr>
        <tr><td>Deprecating the PowerBI.com Content Pack</td><td></td><td>N/A</td></tr>
        <tr><td>Inviting directory guests to Azure AD-backed VSTS accounts</td><td></td><td>N/A</td></tr>
        <tr>
            <td rowspan="12"><a href="/previous-versions/azure/devops/2017/oct-30-vsts" data-raw-source="[30 Oct 2017](/previous-versions/azure/devops/2017/oct-30-vsts)">30 Oct 2017</a></td>
            <td>Modernized column options</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Added support for Not In query operator</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Filtering on Plans</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Add support for read-only to work item rules</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Mention a pull request</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Toggle word wrap and white space in diff views</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Filtering in Package Management</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Revamped create release experience</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Inline GitHub connection as a release artifact source</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Azure Resource Group task - Deployment outputs as variables</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Circle avatars</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Project tags</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td rowspan="13"><a href="/previous-versions/azure/devops/2017/oct-06-vsts" data-raw-source="[06 Oct 2017](/previous-versions/azure/devops/2017/oct-06-vsts)">06 Oct 2017</a></td>
            <td>New experience for code and work items searches</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Pull request comments follow renamed files</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Enhanced filter capability for commits with more than 1000 files changed</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Ctrl+S to save Wiki page</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Reference work items in Wiki</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Enable Wiki home page to show on the Project description page</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Custom Project image on Project description page</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Updated Plans navigation</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Use Azure Key Vault secrets in your CI build</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>New software updates available on hosted VS2017 agents</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Bulk Deploy environments manually from Release view</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Process parameters for deployment templates</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Default properties for Git/GitHub artifact types</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td rowspan="25"><a href="/previous-versions/azure/devops/2017/sep-15-team-services" data-raw-source="[15 Sep 2017](/previous-versions/azure/devops/2017/sep-15-team-services)">15 Sep 2017</a></td>
            <td>New Queries experience</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>Keyboard shortcuts in the work item form</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Contextual actions in the Work Items hub</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>HTML tags stripped in work item grids</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Filtering to the Process and Fields pages in the Process admin</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Create a folder in a repository using web</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Get a permanent link to code</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Filter text highlighting</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Wiki page deep linking</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Move page in Wiki using keyboard</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Preview content as you edit Wiki pages</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Paste rich content as HTML</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Multi-phase builds</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Personalized notifications for releases</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Manage variables using the List and Grid views in the new release definition editor</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Branch filters in environment triggers</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Improved Deployment Groups UI</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Run webtests using the VSTest task</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Chart widget for test plans and test suites</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Preview improvements and support for different log types generated by Visual Studio Test task</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Gulp, Yarn, and more authenticated feed support</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Package feed default permissions now include Project Administrators</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Burndown and Burnup widgets</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>Refreshed error page and seamless tenant switching hint</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Marketplace moves to new markdown-it parser</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="29"><a href="/previous-versions/azure/devops/2017/aug-28-team-services" data-raw-source="[28 Aug 2017](/previous-versions/azure/devops/2017/aug-28-team-services)">28 Aug 2017</a></td>
            <td>Work Items hub</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>Customizable work item rules</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Mentioned support for the My work items page</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Custom Fields and Tags in Notifications</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Inline add on Delivery Plans</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Forks</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>File minimap</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Bracket matching</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Toggle white space</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Updated email templates for push notification</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Complete Work Items settings</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Find lost commits due to a Force Push</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Update default repo permissions for admins</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>CI builds for Bitbucket repositories</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Pauses build definitions</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Task input validations support</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>New Release Definition Editor general availability</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Enhancements in new Release Definition editor</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Release Template Extensibility</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Conditional release tasks and phases</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Approve multiple environments</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Requests history for service endpoints</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Upload attachments to test runs and test results</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Test batching</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>JMeter 3.2 for load testing</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Streamlined user management general availability</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Adding User to Projects and Teams</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Graph REST APIs in Public Preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Profile Card</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td rowspan="30"><a href="/previous-versions/azure/devops/2017/aug-04-team-services" data-raw-source="[4 Aug 2017](/previous-versions/azure/devops/2017/aug-04-team-services)">4 Aug 2017</a></td>
            <td>Copy work item processes</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Updated order of the last column in the Kanban board</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>See the projects using a process</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Filtering on Kanban board</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Wiki in Public Preview</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Improvements in Wiki edit experience</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Revert a Wiki revision</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Create a Wiki page from a broken link</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Setting to turn off web editing for TFVC repos</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Identify stale branches</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Search for a deleted branch and re-create it</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Branch updates page is now Pushes</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Retain filename when moving from Files to Commits</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Pull Request Status Extensibility in Public Preview</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Let contributed build sections control section visibility</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Variable group support</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>dotnet task supports authenticated feeds, web projects</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Ansible Extension on Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Variable groups, Retention, and Options tab now available in the new Release Definition Editor</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Release status badge-in Code hub</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Enhancements to Build definition menu when adding artifacts</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Revert your release definition to older version</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr><br/>        <tr>
            <td>Exploratory testing traceability improvements for work item links, iterations, and area paths</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Screenshot and annotation support for desktop apps with Chrome browser for manual tests</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Filters for Test Case work items in Test Plans and Suites in Test Hub</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Test trend charts for Release Environments and Test Runs</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Markdown formatting support for Test Run and Test Result comments</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Add link to existing bug for a failing test</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Reorder favorite groups</td>
            <td></td><td><em>2018.2</em></td>
        </tr>
        <tr>
            <td>Enable Visual Studio Code direct install option in Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="20"><a href="/previous-versions/azure/devops/2017/jul-14-team-services" data-raw-source="[14 Jul 2017](/previous-versions/azure/devops/2017/jul-14-team-services)">14 Jul 2017</a></td>
            <td>Migrate team projects between two inherited processes with the same parent</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Filtering on Backlogs, Sprints, and Queries</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Expand to show empty fields on a Kanban card</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Automatically complete work items when completing pull requests</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Policies: Reset votes on push/new iteration</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Notifications: Great email templates for pull request workflows</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Pull request details: View original diff for code comments</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Task lists in pull request descriptions and comments</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Ability to &quot;Like&quot; comments in pull requests</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Pull request build variables</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Faster publishing of artifacts from Windows agents to file shares</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Code information in Release with Jenkins CI</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Task group References</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Task group versioning</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Multi Configuration support in Server Side (Agentless) tasks</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Task group import and export</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>New Release Definition Editor (Preview)</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Velocity Widget for the Analytics Extension</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>Notifications: Give team admins control over the delivery of notifications targeting the team</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Constraints on SVG images, screenshots, and badges</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="24"><a href="/previous-versions/azure/devops/2017/jun-22-team-services" data-raw-source="[22 Jun 2017](/previous-versions/azure/devops/2017/jun-22-team-services)">22 Jun 2017</a></td>
            <td>Fields can be shared across processes</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>Work item type icons</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Show/hide work item field borders</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Allow extensions to block work item save</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Collapsible pull request comments</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Improved workflow when approving with suggestions</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Filters pull request tree by file name</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Pull request callout on commit details page becomes richer</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Filter tree view in Code</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Git tags web view</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Export and import build definitions</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Visual Studio latest and hosted agent pools</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Build definition menu on build summary page</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Release Triggers: Continuous deployment for changes pushed to a Git repository</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Enhancements to Server tasks</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Consume Secrets from an Azure Key Vault as variables</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Package Management experience updates</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Packages build task updates</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Project Collection Administrators can link/make initial purchase</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Deep link to easily remove your spending limit during a Marketplace purchase</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Improvements to OAuth permissions page</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>Streamlined user management (preview)</td>
            <td></td><td>N/A</td>
        </tr>
                <tr>
            <td>Enhanced Publisher experience with Sales Transactions for Paid extensions</td>
            <td></td><td>N/A</td>
        </tr>
                <tr>
            <td>Setup Power BI Content Pack</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="19"><a href="/previous-versions/azure/devops/2017/jun-01-team-services" data-raw-source="[1 Jun 2017](/previous-versions/azure/devops/2017/jun-01-team-services)">1 Jun 2017</a></td>
            <td>Mobile work item form general availability</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>New widgets for Analytics extension</td>
            <td></td><td><em>2019</em></td>
        </tr>
        <tr>
            <td>Path filtering support for Git notifications</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>More pull request comments filtering options</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Search for a commit in branches starting with a prefix</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Visual Studio Enterprise benefit for pipelines in Team Services</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Work with secure files such as Apple certificates</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Extensions with build templates</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Deprecate a task in an extension</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Task group references</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Variables Support in Manual Intervention task</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Control releases to an environment based on the source branch</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Release Triggers for Git repositories as an artifact source</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>On-demand triggering of automated tests</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Acquisition data in Extension Hub for Marketplace publishers</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Q&amp;A for Marketplace publishers</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>GitHub and Custom Q&amp;A support for marketplace extensions</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Retain VSTS identity when navigating to Marketplace from VSTS</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Azure AD sign in address renames</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="25"><a href="/previous-versions/azure/devops/2017/may-11-team-services" data-raw-source="[11 May 2017](/previous-versions/azure/devops/2017/may-11-team-services)">11 May 2017</a></td>
            <td>VM deployment (Public Preview)</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Azure virtual machine scale set</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Built-in tasks for building and deploying container-based applications</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Azure Web App deployment updates</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Install an SSH key during a build or release</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Retiring the old editor</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Tasks fail if Visual Studio 2017 is specified but not present on agent</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Automatic linking from work items to builds</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Delivery Plans general availability</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Work item search general availability</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Updated process customization experience</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Modify out of the box fields</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Files hub improvements</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Git LFS file locking</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>New branch policies configuration experience</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Shares pull requests with teams</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Default notifications for PR comments</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Improved team PR notifications</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>New tree view control</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Maven for Package Management (Public Preview)</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>NuGet Restore, Command, and Tool Installer build tasks</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Combined email recipients for notifications now enabled by default</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Out of the box notifications out of preview</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Enhanced publisher experience in the Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Owner and contributor roles can purchase through the Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="19"><a href="/previous-versions/azure/devops/2017/apr-19-team-services" data-raw-source="[19 Apr 2017](/previous-versions/azure/devops/2017/apr-19-team-services)">19 Apr 2017</a></td>
            <td>Delivery timeline markers</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Visualize your git repository</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Git commits comments use the new discussion control</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Improved package list</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Build tool installers</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>SSH deployment improvements</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Deploy to Azure Government Cloud</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Timeout enhancements for the Manual Intervention task</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Release Logs Page Improvements</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Azure App Service task enhancements and templates for Python and PHP applications</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Deploy Java to Azure Web Apps</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Java code coverage enhancements</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Maven and SonarQube improvements</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Improved Jenkins integration</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Google Play extension enhancements</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>iOS DevOps enhancements</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Contact extension customers</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Marketplace feedback excluded from ratings</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Reports for Marketplace Publishers</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="17"><a href="/previous-versions/azure/devops/2017/mar-29-team-services" data-raw-source="[29 Mar 2017](/previous-versions/azure/devops/2017/mar-29-team-services)">29 Mar 2017</a></td>
            <td>Work item search for discussions</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Pull Request filtering by people</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Reason required when bypassing pull request policies</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Add and view Git tags</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Updated Changeset and Shelveset pages</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Import repositories from TFVC to Git</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Multiple recipients included on the same email (preview)</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Conditional build tasks</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Package Management adds npm READMEs and download button</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Updated Package Management experience available to all accounts</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Override template parameters in Azure resource group deployments</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Continuous Delivery in the Azure portal supports any Git repo</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Separation of duties for deployment requester and approvers</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Set maximum number of parallel deployments</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Q&amp;A support for Marketplace extensions</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Enhancements to display publisher's terms, license, and privacy policy in Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Improved sign-out</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="14"><a href="/previous-versions/azure/devops/2017/mar-08-team-services" data-raw-source="[8 Mar 2017](/previous-versions/azure/devops/2017/mar-08-team-services)">8 Mar 2017</a></td>
            <td>Delivery Plans field criteria</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>New mobile discussion experience</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Optimized mobile identity picker</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018](/visualstudio/releasenotes/tfs2018-relnotes)">2018</a></td>
        </tr>
        <tr>
            <td>Customized backlog levels</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Custom work item identity fields</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Pull Request improvements for teams</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>New policy for no active comments</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Build agent upgrade status</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>GitHub pull request builds</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Keep track of your free hosted agent minutes</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Out of the box notifications enabled by default</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Getting notified when extensions are installed, require attention, and more</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Release level approvals</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>.NET Core tasks support project files</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td rowspan="13"><a href="/previous-versions/azure/devops/2017/feb-15-team-services" data-raw-source="[15 Feb 2017](/previous-versions/azure/devops/2017/feb-15-team-services)">15 Feb 2017</a></td>
            <td>Improved support for team PR notifications</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Improved CTAs for PR author and reviewers</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Actionable comments</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Updates view shows rebase and force push</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Improved commit filtering</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Maintenance for working directories</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Agent selection improvement</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Run tests using Agent Phases</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Multiple versions of Extension tasks</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Extension management permissions and new email notifications</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Updated Package Management experience</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Support for Azure AD conditional access</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Pipelines queue</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td rowspan="17"><a href="/previous-versions/azure/devops/2017/jan-25-team-services" data-raw-source="[25 Jan 2017](/previous-versions/azure/devops/2017/jan-25-team-services)">25 Jan 2017</a></td>
            <td>Delivery Plans</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Mobile work item form preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Build editor preview</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Repo admin permission changes</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Branch policy improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>PR comment improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Discussion control toolbar</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>View PRs for a commit</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Release views in Package Management</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>npmjs.com upstream now caches packages</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Run tests built using Visual Studio 2017</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Track changes to test steps</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Sorting on work item search results</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Linking to changelog on the Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Release action in Build summary</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Security for variable groups</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Web app deployment history in Azure portal</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td rowspan="21"><a href="/previous-versions/azure/devops/2017/jan-05-team-services" data-raw-source="[5 Jan 2017](/previous-versions/azure/devops/2017/jan-05-team-services)">5 Jan 2017</a></td>
            <td>New account and project home pages</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Attachments in PR discussions</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Support file exclusions in the required reviewer policy</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Highlight the PRs that have updates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Branch policy for PR merge strategy</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Expose merge conflict information</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Team Room Deprecation Announcement</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>New notification settings experience</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>New delivery options for team subscriptions</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Out of the box notifications (preview)</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Updated hosted build image</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Firefox support for Test &amp; Feedback extension</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Favorites for Test Plans</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Test Impact Analysis for managed automated tests</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>SonarQube MSBuild tasks</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Improved experience for Search results</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Release Management parallel execution</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Inline service endpoints</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Multiple release triggers with branch and tag filters</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Set defaults for artifact sources in RM</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Variable groups support in RM</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td rowspan="14"><a href="/previous-versions/azure/devops/2016/nov-23-team-services" data-raw-source="[23 Nov 2016](/previous-versions/azure/devops/2016/nov-23-team-services)">23 Nov 2016</a></td>
            <td>Search for commits in branches</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Search for a file or folder in commit history</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Follow a pull request</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Restart pull request merge</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Completion blocked on rejected pull requests</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Markdown in pull request description</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Task versioning for Build and Release definitions</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Hosted Linux pool preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Build and deploy Docker apps to Azure more easily</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>New licensing model for Build and Release Management</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>NuGet + Credential Provider Bundle updated</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Delete test artifacts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Inline service connections in Build and Release</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Links build artifacts from another team project</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2016/nov-16-team-services" data-raw-source="[16 Nov 2016](/previous-versions/azure/devops/2016/nov-16-team-services)">16 Nov 2016</a></td>
            <td>Package Management General Availability</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Release Management General Availability</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>TFS Database Import Service</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Work Item Search public preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="13"><a href="/previous-versions/azure/devops/2016/nov-02-team-services" data-raw-source="[2 Nov 2016](/previous-versions/azure/devops/2016/nov-02-team-services)">2 Nov 2016</a></td>
            <td>Package Management in India and Brazil</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Microsoft Teams integration</td>
            <td></td><td>2017.2</td>
        </tr>
        <tr>
            <td>Repo Favorites</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Rollbacks build definitions</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Disable the sync and checkout of sources in a build</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Docker extension enhancements</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>.NET Core build task</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Build and release management templates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>ASP.NET Core and NodeJs deployments</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Azure Web App Services manage task</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Release Management available in multiple regions</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>REST client helpers for Test Step operations</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Test case description in Web runner</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td rowspan="15"><a href="/previous-versions/azure/devops/2016/oct-12-team-services" data-raw-source="[12 Oct 2016](/previous-versions/azure/devops/2016/oct-12-team-services)">12 Oct 2016</a></td>
            <td>New navigation on by default</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Cherry-pick and revert</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Commit page improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Configurable compare branch</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Find a file or folder</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Suggested value in work item pick lists</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Xcode 8 Signing and Exporting Packages in the Xcode Task</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>FindBugs in the Gradle build task</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Email support for Azure AD groups</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Multiple schedules in releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Azure resource group improvements</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Azure CLI task</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Simplified Azure endpoint creation</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Test &amp; Feedback extension general availability</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Visual Studio subscribers automatically use their free license</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="13"><a href="/previous-versions/azure/devops/2016/sep-21-team-services" data-raw-source="[21 Sep 2016](/previous-versions/azure/devops/2016/sep-21-team-services)">21 Sep 2016</a></td>
            <td>Attachments live preview</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Work item type layout improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Disable work item types</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Import Repository</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Markdown preview button</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Confirmation for deleting repos</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Add .gitignore during repo creation</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Verify bugs from work item</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Xcode task xcpretty formatting</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Publish Jenkins test and code coverage results</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Build summary for Maven and Gradle tasks</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>FindBugs and CheckStyle in Maven build tasks</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td>Deployment status widget</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=839593" data-raw-source="[2017.1](https://go.microsoft.com/fwlink/?LinkId=839593)">2017.1</a></td>
        </tr>
        <tr>
            <td rowspan="14"><a href="/previous-versions/azure/devops/2016/sep-02-team-services" data-raw-source="[2 Sep 2016](/previous-versions/azure/devops/2016/sep-02-team-services)">2 Sep 2016</a></td>
            <td>Custom work item types</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Work item history tab</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Managing a NuGet package's lifecycle</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Build queue tab</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Hosted build pool build agent migration</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Xamarin license step removed</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Jenkins with untrusted SSL certificates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Apple App Store extension</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Request Feedback</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Checkstyle static analysis</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Deployment manual intervention</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Service endpoint improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>SQL database deployment task</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>User lifecycle management improvements</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="22"><a href="/previous-versions/azure/devops/2016/aug-17-team-services" data-raw-source="[17 Aug 2016](/previous-versions/azure/devops/2016/aug-17-team-services)">17 Aug 2016</a></td>
            <td>Pull Request improvements: <br />
                Redesigned UI <br />
                Overview <br />
                Files <br />
                Updates <br />
                Comments, now with Markdown and emoji <br />
                Auto-complete pull requests waiting on policies</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Clone Git repositories from your browser using Tower</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Download packages without NuGet</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Packages: Get started quickly</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Queue Jenkins jobs from builds and releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Jenkins service hook enhancements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Run SSH commands on remote machines from builds and releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Create archives from builds and releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Copy files over SSH from builds and releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Download Jenkins artifacts to builds and releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Use FTP or FTPS to upload files from builds and releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Google Play Extension improvements</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Maven and Gradle tasks produce a build summary when running a SonarQube analysis</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Work item templates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Quickly "Unfollow" work item</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Drag and drop attachments</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Assigned to Me widget</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Dashboard permissions</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Configure test outcomes for tests across different test suites</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Test Run and Test Result summary – traceability to Releases and manual test artifacts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Unpublish extension – Removing a public extension from the Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Rate Limits – Delaying user requests to avoid outages</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="9"><a href="/previous-versions/azure/devops/2016/jul-29-team-services" data-raw-source="[29 Jul 2016](/previous-versions/azure/devops/2016/jul-29-team-services)">29 Jul 2016</a> </td>
            <td>Git and TFVC – History view and diff view updates</td>
            <td></td><td><a href="/visualstudio/releasenotes/tfs2015-update1-vs" data-raw-source="[2017](/visualstudio/releasenotes/tfs2015-update1-vs)">2017</a></td>
        </tr>
        <tr>
            <td>Restrict Package Management feed creation</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release management improvements – Azure deployments, release policies: <br />
                Agent queue management <br />
                Azure deployments <br />
                Policies – Soft delete releases <br />
                Policies – Retention of releases and builds <br />
                Release definition authoring improvements – linked artifacts improvements <br />
                Release – redeploy after success</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Test traceability and release environments support in Test History</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Exploratory testing improvements – view unexplored work items, capture web page load data</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Dashboard improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Java PMD analysis in Gradle build task</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>User management – export users and licenses</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Backlog extension points</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="18"><a href="/previous-versions/azure/devops/2016/jul-07-team-services" data-raw-source="[7 Jul 2016](/previous-versions/azure/devops/2016/jul-07-team-services)">7 Jul 2016</a>  </td>
            <td>Resizable WIT charts on dashboards</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Filter boards to a parent work item</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Links front and center</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Test settings configuration for Kanban board</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Comment tracking for pull requests</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Browse Code Coverage reports in the web</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Maven and Gradle tasks produce a build summary when running a SonarQube analysis</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Agent queue role-based security</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Task-level time-outs</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Import/Export/Clone release definition</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Web app deployment using ARM</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Partially successful deployments</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>View and download attachments associated with releases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>GitHub artifacts for RM</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>.NET SQL Extension</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Image action log in Web Test runner</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Order tests in Test hub</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Pick a build to test with</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="22"><a href="/previous-versions/azure/devops/2016/jun-17-team-services" data-raw-source="[17 Jun 2016](/previous-versions/azure/devops/2016/jun-17-team-services)">17 Jun 2016</a></td>
            <td>Git &amp; TFVC – Browsing branches</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Git &amp; TFVC – Ahead/behind</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Git &amp; TFVC – Branch picker includes "Mine"</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Git &amp; TFVC – Path control</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Git &amp; TFVC – File type icons</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Work Items – An improved header</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Work Items – Custom states</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Exploratory Testing – Insights</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Exploratory Testing – Auto stop screen recordings</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Screen recording support in Web runner (for Chrome) </td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Bugs filed as children – Web runner / Exploratory testing extension</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Test – History across branches</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Test – Automated testing for SCVMM and VMware</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release – Test status visibility</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release – Support Java PMD analysis in Maven build task</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release – Passing oauth tokens to scripts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Build – Enable path filters for Git CI triggers</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Build – Updated hosted pool software</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Dashboards – Resizable query results widget</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Third-party plugins – Jenkins plug-in to RM</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Marketplace – Publisher review responses</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Team Rooms – Build vNext support</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="1"><a href="https://devblogs.microsoft.com/devops/visual-studio-team-services-is-in-brazil/" data-raw-source="[6 Jun 2016](https://devblogs.microsoft.com/devops/visual-studio-team-services-is-in-brazil/)">6 Jun 2016</a></td>
            <td>Brazil region for Visual Studio Team Services</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="15"><a href="/previous-versions/azure/devops/2016/jun-01-team-services" data-raw-source="[1 Jun 2016](/previous-versions/azure/devops/2016/jun-01-team-services)">1 Jun 2016</a></td>
            <td>Filtering in Kanban board</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Process configuration REST APIs</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Dashboards REST APIs</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>SSH clients can connect to Git repos</td>
            <td></td><td>2015.3</td>
        </tr>
        <tr>
            <td>Redesigned Branches page</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Create and send links to specific sections of code</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>API updates for package management</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Screenshot and system info support in Chrome Web runner</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Ordering of tests in Test Hub</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Docker integration for build and release management</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>SonarQube results in pull request view</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Test results trend for build</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Service hooks for release management</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>TeamCity artifacts for release management</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release Management Client SDK</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="19"><a href="/previous-versions/azure/devops/2016/may-06-team-services" data-raw-source="[6 May 2016](/previous-versions/azure/devops/2016/may-06-team-services)">6 May 2016</a></td>
            <td>Email improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Checkbox control</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Work Item page management</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Turning board annotations on/off</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Clear Formatting command</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Dashboard updates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Adding attachments during manual testing</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Test plan/suite columns</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Build and release summary updates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release Management repository linking</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Copy, Export, and Import release definitions</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Schedule based deployments</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release Management REST APIs</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Simplified Release definition wizard</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>New Release Management job execution variables</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Improved build and pull request traceability</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Team Project rename permission</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Admin settings Work hub</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>UX improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="17"><a href="/previous-versions/azure/devops/2016/apr-13-team-services" data-raw-source="[13 Apr 2016](/previous-versions/azure/devops/2016/apr-13-team-services)">13 Apr 2016</a></td>
            <td>Follow a work item</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Change work item type</td>
            <td></td><td>2019 </td>
        </tr>
        <tr>
            <td>Work Item move (single or bulk)</td>
            <td></td><td>2019</td>
        </tr>
        <tr>
            <td>Kanban board live updates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Pick lists for work Items</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Checklist improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Build to Line number</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Build log view supports much larger logs</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Java Build templates</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Xamarin Build Tasks</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Widget SDK: Reusable CSS and DOM templates</td>
            <td></td><td>2015.3</td>
        </tr>
        <tr>
            <td>Adding users from the team members widget</td>
            <td></td><td>2015.3</td>
        </tr>
        <tr>
            <td>Collection in the domain</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Release Management – Email release summary</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release Management – Dashboard widget for release definition summary</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release Management – Deploy based on conditions in multiple environments</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Release Management – Provision VMs or run a PowerShell script using SCVMM extension</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="11"><a href="/previous-versions/azure/devops/2016/mar-24-team-services" data-raw-source="[24 Mar 2016](/previous-versions/azure/devops/2016/mar-24-team-services)">24 Mar 2016</a></td>
            <td>Commit traceability</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>View Git LFS files in the web</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Git for Windows now includes Team Services authentication by default</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Custom multiline text fields</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Test progress from your cards</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Capture screen recordings</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Queue a Run by specifying your test suite</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Configuration management in the Test Hub</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Enable build result extensions to specify order and column</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Configure status API reporting for a build definition</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Tab contribution point</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="13"><a href="/previous-versions/azure/devops/2016/mar-03-team-services" data-raw-source="[3 Mar 2016](/previous-versions/azure/devops/2016/mar-03-team-services)">3 Mar 2016</a></td>
            <td>View test results for each release environment</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Triggers: Deploy based on completion in multiple environments (join)</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Epic and Feature board drill-down</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Exploratory testing directly from a work item</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Data collection: Image action log</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Create test cases based on Image action log data</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Assigning configurations to test plans, test suites and test cases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Squash merge pull requests</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Clone in IntelliJ, Android Studio, etc.</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Gated builds for Team Foundation Version Control (TFVC)</td>
            <td></td><td>2015.2</td>
        </tr>
        <tr>
            <td>Automated testing on Azure environments</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>NuGet package delist</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Office connector</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="13"><a href="/previous-versions/azure/devops/2016/feb-16-team-services" data-raw-source="[16 Feb 2016](/previous-versions/azure/devops/2016/feb-16-team-services)">16 Feb 2016</a></td>
            <td>Package management is now available in Europe and Australia</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Search for extensions on Visual Studio Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Work item query charts in the dashboard catalog</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Cumulative flow diagram widget</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Flexible build policy for Git</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>SonarQube Quality Gates in Build</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>RM: UI extensibility</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>SCVMM support</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Exploratory Testing improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Azure SQL Database Deployment task</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Delete Test Plan</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>#mention</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Keyboard shortcuts for Kanban board</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td rowspan="17"><a href="/previous-versions/azure/devops/2016/jan-25-team-services" data-raw-source="[25 Jan 2016](/previous-versions/azure/devops/2016/jan-25-team-services)">25 Jan 2016</a></td>
            <td>Public preview of the dashboard widget SDK</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Create branch and links to related artifacts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Build widgets in the catalog</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Markdown widget with file from repository</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Autorefresh dashboards</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Richer visualizations in the build summary page</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>View passed test results and file bugs in build summary page</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Test summary in build status notification email</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Support for editing tags in the bulk edit dialog</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Deleting a custom field</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Keyboard shortcuts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Test plan improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Exploratory testing improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Release orchestration improvements</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>UI extensibility for release management</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Search scope selector</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Search across Git and TFVC projects</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="8"><a href="/previous-versions/azure/devops/2015/dec-10-team-services" data-raw-source="[10 Dec 2015](/previous-versions/azure/devops/2015/dec-10-team-services)">10 Dec 2015</a></td>
            <td>Custom work item fields</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Work item discussion</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Work item history improvements</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Deleting work items</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Dashboards edit mode</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Keyboard shortcuts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>On-premises support for Exploratory Testing extension:</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Scope code search using path filters</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td rowspan="7"><a href="/previous-versions/azure/devops/2015/nov-24-team-services" data-raw-source="[24 Nov 2015](/previous-versions/azure/devops/2015/nov-24-team-services)">24 Nov 2015</a></td>
            <td>Git and TFVC in the same team project</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Package Management build tasks</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Implement a task once for multiple platforms</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Pull Request Widget for Dashboards</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td><xref href="mention" data-throw-if-not-resolved="False" data-raw-source="@mention"></xref> and #ID in code</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Reordering cards on boards</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Global shortcut keys</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td rowspan="7"><a href="/previous-versions/azure/devops/2015/nov-18-team-services" data-raw-source="[18 Nov 2015](/previous-versions/azure/devops/2015/nov-18-team-services)">18 Nov 2015</a></td>
            <td>Extensions and Marketplace</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Release Management public preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Package Management public preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Code Search public preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Test Results in Build</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=615439" data-raw-source="[2015.2](https://go.microsoft.com/fwlink/?LinkId=615439)">2015.2</a></td>
        </tr>
        <tr>
            <td>Exploratory Testing extension</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Test Manager extension</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="6"><a href="/previous-versions/azure/devops/2015/oct-30-team-services" data-raw-source="[30 Oct 2015](/previous-versions/azure/devops/2015/oct-30-team-services)">30 Oct 2015</a></td>
            <td>Dashboards</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Improved pull request experience</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Manual test iteration results</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Retention policy for test results</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Reorder and reparent tasks from the Kanban board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>PREVIEW: New Work Item form</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="5"><a href="/previous-versions/azure/devops/2015/oct-08-team-services" data-raw-source="[8 Oct 2015](/previous-versions/azure/devops/2015/oct-08-team-services)">8 Oct 2015</a></td>
            <td>Azure Active Directory Group support</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Starting with Git, made easy</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Improved commit details</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>SonarQube analysis from a Maven build task</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>PREVIEW: New Work Item form</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td rowspan="7"><a href="/previous-versions/azure/devops/2015/sep-18-team-services" data-raw-source="[18 Sep 2015](/previous-versions/azure/devops/2015/sep-18-team-services)">18 Sep 2015</a></td>
            <td>Inline tasks on the Kanban board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Query and display of Kanban fields</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Multi-select items on the backlog</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Branch policy to require linked work items</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Export test outcomes</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Work item trend and rollup reporting in Power BI</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>Support for publishing xUnit results</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2015/aug-26-team-services" data-raw-source="[26 Aug 2015](/previous-versions/azure/devops/2015/aug-26-team-services)">26 Aug 2015</a></td>
            <td>Rename columns in place</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Choosing users for capacity planning</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Burndown with available capacity</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>SonarQube analysis build tasks</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2015/aug-07-team-services" data-raw-source="[7 Aug 2015](/previous-versions/azure/devops/2015/aug-07-team-services)">7 Aug 2015</a></td>
            <td>Multi-select items on the product backlog</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Reorder cards when changing columns</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Color tags and titles on your cards</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Libraries for integrating with VSTS now available at nuget.org</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="1"><a href="https://devblogs.microsoft.com/devops/reporting-on-work-items-with-power-bi/" data-raw-source="[22 Jul 2015](https://devblogs.microsoft.com/devops/reporting-on-work-items-with-power-bi/)">22 Jul 2015</a></td>
            <td>Power BI reporting on Work Item data</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td rowspan="7"><a href="/previous-versions/azure/devops/2015/jul-17-team-services" data-raw-source="[17 Jul 2015](/previous-versions/azure/devops/2015/jul-17-team-services)">17 Jul 2015</a></td>
            <td>Multiple activities per team member</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Configure settings directly from backlogs/boards</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Hide empty fields on cards</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Card coloring on Taskboard</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Drag any item to an iteration from anywhere</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Build your projects hosted in GitHub</td>
            <td></td><td>Future</td>
        </tr>
        <tr>
            <td>New VSTS integrations</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2015/jul-07-team-services" data-raw-source="[7 Jul 2015](/previous-versions/azure/devops/2015/jul-07-team-services)">7 Jul 2015</a></td>
            <td>Card coloring on Kanban board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Personal access tokens</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/?LinkId=831912" data-raw-source="[2017](https://go.microsoft.com/fwlink/?LinkId=831912)">2017</a></td>
        </tr>
        <tr>
            <td>Adding work directly to a sprint</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2015/jun-03-team-services" data-raw-source="[3 Jun 2015](/previous-versions/azure/devops/2015/jun-03-team-services)">3 Jun 2015</a></td>
            <td>Kanban swim lanes</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>#Mention work items</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Automated testing in Build vNext</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015.1](https://www.microsoft.com/download/details.aspx?id=48260)">2015.1</a></td>
        </tr>
        <tr>
            <td>Team settings API</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td rowspan="7"><a href="/previous-versions/azure/devops/2015/may-15-team-services" data-raw-source="[15 May 2015](/previous-versions/azure/devops/2015/may-15-team-services)">15 May 2015</a></td>
            <td>Build vNext</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Backlog navigation update</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Opt-in to portfolio backlogs</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Improved SAFe support</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Kanban collapsed columns</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Git branch policies</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Power BI &amp; VSO</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2015/may-11-team-services" data-raw-source="[11 May 2015](/previous-versions/azure/devops/2015/may-11-team-services)">11 May 2015</a></td>
            <td>Application Insights: <br />
                iOS and Android support <br />
                Performance counters for Java applications <br />
                Unhandled exceptions in Java apps <br />
                Drag-across to select a time range</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="https://blogs.msdn.com/b/bharry/archive//previous-versions/azure/devops/2015/05/10/vs-online-hosted-in-australia.aspx" data-raw-source="[8 May 2015](https://blogs.msdn.com/b/bharry/archive//previous-versions/azure/devops/2015/05/10/vs-online-hosted-in-australia.aspx)">8 May 2015</a></td>
            <td>Australia region for Visual Studio Team Services</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="https://azure.microsoft.com/blog/announcing-application-insights-public-preview-2/" data-raw-source="[29 April 2015](https://azure.microsoft.com/blog/announcing-application-insights-public-preview-2/)">29 April 2015</a></td>
            <td>Application Insights Public Commercial Preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/azure/devops/integrate/" data-raw-source="[29 April 2015](/azure/devops/integrate/)">29 April 2015</a></td>
            <td>Extensions</td>
            <td></td><td>2015.2</td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2015/apr-27-team-services" data-raw-source="[27 Apr 2015](/previous-versions/azure/devops/2015/apr-27-team-services)">27 Apr 2015</a></td>
            <td>Adding fields to cards</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Kanban board filtering</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Card options on the Taskboard</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Account restore</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2015/apr-24-team-services" data-raw-source="[24 Apr 2015](/previous-versions/azure/devops/2015/apr-24-team-services)">24 Apr 2015</a></td>
            <td>Team Project Rename</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2015/apr-22-team-services" data-raw-source="[22 Apr 2015](/previous-versions/azure/devops/2015/apr-22-team-services)">22 Apr 2015</a></td>
            <td>Application Insights: <br />
                Synthetic data filtering <br />
                New usage experience for ASP.NET, Java, and other applications <br />
                Daily Active User calculations</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="https://devblogs.microsoft.com/devops/general-availability-of-codelens-in-visual-studio-online/" data-raw-source="[17 Apr 2015](https://devblogs.microsoft.com/devops/general-availability-of-codelens-in-visual-studio-online/)">17 Apr 2015</a></td>
            <td>CodeLens General Availability on Visual Studio Team Services</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2015/apr-10-team-services" data-raw-source="[10 Apr 2015](/previous-versions/azure/devops/2015/apr-10-team-services)">10 Apr 2015</a></td>
            <td>Configure cards</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Markdown editing for definition of done</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>CFD options</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Web history view for Git projects</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2015/mar-27-team-services" data-raw-source="[27 Mar 2015](/previous-versions/azure/devops/2015/mar-27-team-services)">27 Mar 2015</a></td>
            <td>Application Insights: Save search page, pause export, and export on alert fail</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="7"><a href="/previous-versions/azure/devops/2015/mar-10-team-services" data-raw-source="[10 Mar 2015](/previous-versions/azure/devops/2015/mar-10-team-services)">10 Mar 2015</a></td>
            <td>Current iteration query token</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Reordering on the Kanban board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Kanban definition of done</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Responsive card sizes</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Bugs on the Taskboard</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Syntax highlight for XML, Sass, Objective-C, R</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>CodeLens for accounts in West Europe</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/azure/azure-monitor/app/java-get-started" data-raw-source="[9 Mar 2015](/azure/azure-monitor/app/java-get-started)">9 Mar 2015</a></td>
            <td>Application Insights support for Java</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2015/feb-18-team-services" data-raw-source="[18 Feb 2015](/previous-versions/azure/devops/2015/feb-18-team-services)">18 Feb 2015</a></td>
            <td>Adding and editing directly from the board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Split columns on the Kanban board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Assign multiple people to test suites</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Application Insights in the Azure portal (Preview)</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="https://devblogs.microsoft.com/devops/announcing-limited-preview-for-visual-studio-online-code-search/" data-raw-source="[13 Feb 2015](https://devblogs.microsoft.com/devops/announcing-limited-preview-for-visual-studio-online-code-search/)">13 Feb 2015</a></td>
            <td>Limited preview for Code Search</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="https://azure.microsoft.com/updates/application-insights-support-for-windows-phone-and-windows-store/" data-raw-source="[29 Jan 2015](https://azure.microsoft.com/updates/application-insights-support-for-windows-phone-and-windows-store/)">29 Jan 2015</a></td>
            <td>Application Insights support for Windows Phone and Windows Store Applications</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2015/jan-27-team-services" data-raw-source="[27 Jan 2015](/previous-versions/azure/devops/2015/jan-27-team-services)">27 Jan 2015</a></td>
            <td>Basic license upgraded</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Reordering on the Taskboard</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Unparented Tasks on the Taskboard</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Inline editing on the Kanban board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td><a href="https://blogs.msdn.com/b/bharry/archive//previous-versions/azure/devops/2015/01/15/visual-studio-online-iso-27001-certification-and-european-model-clauses.aspx" data-raw-source="[15 Jan 2015](https://blogs.msdn.com/b/bharry/archive//previous-versions/azure/devops/2015/01/15/visual-studio-online-iso-27001-certification-and-european-model-clauses.aspx)">15 Jan 2015</a></td>
            <td>VS Online ISO 27001 Certification</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="6"><a href="/previous-versions/azure/devops/2014/dec-17-team-services" data-raw-source="[17 Dec 2014](/previous-versions/azure/devops/2014/dec-17-team-services)">17 Dec 2014</a></td>
            <td>Quick code editing</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Filtering on backlogs and queries</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Sprint backlog and task board improvements</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>New integrations: Slack and Azuqua</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Preview APIs for adding and updating files in source control</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>CodeLens for Visual Studio Team Services</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="2">11 Dec 2014</td>
            <td><a href="https://azure.microsoft.com/updates/application-insights-status-monitor-and-sdk-updated/" data-raw-source="[Application Insights Status Monitor and SDK updates](https://azure.microsoft.com/updates/application-insights-status-monitor-and-sdk-updated/)">Application Insights Status Monitor and SDK updates</a></td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="https://azure.microsoft.com/updates/application-insights-adds-telemetry-export-and-segmentation-chart-editing/" data-raw-source="[Application Insights includes telemetry export and segmentation editing](https://azure.microsoft.com/updates/application-insights-adds-telemetry-export-and-segmentation-chart-editing/)">Application Insights includes telemetry export and segmentation editing</a></td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="5"><a href="/previous-versions/azure/devops/2014/dec-02-team-services" data-raw-source="[2 Dec 2014](/previous-versions/azure/devops/2014/dec-02-team-services)">2 Dec 2014</a></td>
            <td>Identity control and avatars</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Pull Request improvements</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Taskboard changes</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Kanban board persisted column headers</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Sharing personal queries</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>12 Nov 2014</td>
            <td>Release Management Preview as VSTS service</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="7"><a href="/previous-versions/azure/devops/2014/nov-04-team-services" data-raw-source="[4 Nov 2014](/previous-versions/azure/devops/2014/nov-04-team-services)">4 Nov 2014</a></td>
            <td>Bugs on the backlog</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Test execution charts</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Recent test results</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Preview Markdown and HTML files in Code Explorer</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Browse link dialog</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>REST batch support</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Third-party OAuth scopes</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2014/oct-28-team-services" data-raw-source="[28 Oct 2014](/previous-versions/azure/devops/2014/oct-28-team-services)">28 Oct 2014</a></td>
            <td>European Datacenter</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>VSTS REST API version 1.0 is here</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Service hooks is out of preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2014/oct-14-team-services" data-raw-source="[14 Oct 2014](/previous-versions/azure/devops/2014/oct-14-team-services)">14 Oct 2014</a></td>
            <td>Test artifacts as work items</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.3](https://www.microsoft.com/download/details.aspx?id=44911)">2013.3</a></td>
        </tr>
        <tr>
            <td>Copy and paste query results</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2014/sep-23-team-services" data-raw-source="[23 Sep 2014](/previous-versions/azure/devops/2014/sep-23-team-services)">23 Sep 2014</a></td>
            <td>Maximizing text area fields</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Navigating to links</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Work item performance improvements</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td rowspan="6"><a href="/previous-versions/azure/devops/2014/sep-04-team-services" data-raw-source="[4 Sep 2014](/previous-versions/azure/devops/2014/sep-04-team-services)">4 Sep 2014</a></td>
            <td>Work Item query improvements</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Quick search through tree controls</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Longer trend charts</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Test Cases related to Test Suites</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>WIT REST API v1.2</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Event and resource versioning within service hooks</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2014/aug-27-team-services" data-raw-source="[27 Aug 2014](/previous-versions/azure/devops/2014/aug-27-team-services)">27 Aug 2014</a></td>
            <td>A license for Stakeholders</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2014/aug-18-team-services" data-raw-source="[18 Aug 2014](/previous-versions/azure/devops/2014/aug-18-team-services)">18 Aug 2014</a></td>
            <td>Project Welcome pages</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=48260" data-raw-source="[2015](https://www.microsoft.com/download/details.aspx?id=48260)">2015</a></td>
        </tr>
        <tr>
            <td>Tagging support in the Test Hub</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td rowspan="5"><a href="/previous-versions/azure/devops/2014/jul-21-team-services" data-raw-source="[21 Jul 2014](/previous-versions/azure/devops/2014/jul-21-team-services)">21 Jul 2014</a></td>
            <td>Using corporate identities with existing accounts</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Viewing existing projects in the Azure portal (Preview)</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Trend charts + aggregation</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Test Hub added to the Advanced License</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Deleting your account</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2014/jul-01-team-services" data-raw-source="[1 Jul 2014](/previous-versions/azure/devops/2014/jul-01-team-services)">1 Jul 2014</a></td>
            <td>Hiding work in progress on the backlog</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.3](https://www.microsoft.com/download/details.aspx?id=44911)">2013.3</a></td>
        </tr>
        <tr>
            <td>Full Screen on the backlog and boards</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td>Move to position on the backlog</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2014/jun-10-team-services" data-raw-source="[10 Jun 2014](/previous-versions/azure/devops/2014/jun-10-team-services)">10 Jun 2014</a></td>
            <td>Pull Requests</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.4](https://www.microsoft.com/download/details.aspx?id=44911)">2013.4</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2014/may-20-team-services" data-raw-source="[20 May 2014](/previous-versions/azure/devops/2014/may-20-team-services)">20 May 2014</a></td>
            <td>Using corporate identities</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Copy/Paste shared parameter data between VS Online and Excel</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.3](https://www.microsoft.com/download/details.aspx?id=44911)">2013.3</a></td>
        </tr>
        <tr>
            <td>End of data export period</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2014/may-12-team-services" data-raw-source="[12 May 2014](/previous-versions/azure/devops/2014/may-12-team-services)">12 May 2014</a></td>
            <td>Integrate with Visual Studio Team Services</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Service Migration with OpsHub</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2014/apr-03-team-services" data-raw-source="[3 Apr 2014](/previous-versions/azure/devops/2014/apr-03-team-services)">3 Apr 2014</a></td>
            <td>General Availability of Visual Studio Team Services</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Application Insights Limited Preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Shared Parameters for Test Cases</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2014/mar-18-team-services" data-raw-source="[18 Mar 2014](/previous-versions/azure/devops/2014/mar-18-team-services)">18 Mar 2014</a></td>
            <td>Getting started with Application Insights</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Search across your application trace logs</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2014/feb-28-team-services" data-raw-source="[28 Feb 2014](/previous-versions/azure/devops/2014/feb-28-team-services)">28 Feb 2014</a></td>
            <td>Build support for Java code managed in Git</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td>Java JDK, Ant, and Maven libraries preinstalled in hosted build</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Maven support for TF version control projects</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2014/feb-10-team-services" data-raw-source="[10 Feb 2014](/previous-versions/azure/devops/2014/feb-10-team-services)">10 Feb 2014</a></td>
            <td>Exporting test artifacts</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td>New "create tags" permission</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2014/jan-22-team-services" data-raw-source="[22 Jan 2014](/previous-versions/azure/devops/2014/jan-22-team-services)">22 Jan 2014</a></td>
            <td>Querying tags</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td>Removing weekends from the Burndown</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td>Configurable CFD dates</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/dec-11-team-services" data-raw-source="[11 Dec 2013](/previous-versions/azure/devops/2013/dec-11-team-services)">11 Dec 2013</a></td>
            <td>Application Insights – Response Stacked Distribution</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Application Insights – Windows Store App support</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Asynchronous backlogs</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/nov-13-team-services" data-raw-source="[13 Nov 2013](/previous-versions/azure/devops/2013/nov-13-team-services)">13 Nov 2013</a></td>
            <td>Commercial preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Application Insights limited preview</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Live editing of Windows Azure sites</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2013/nov-08-team-services" data-raw-source="[8 Nov 2013](/previous-versions/azure/devops/2013/nov-08-team-services)">8 Nov 2013</a></td>
            <td>Work item chart pinning</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2013/oct-21-team-services" data-raw-source="[21 Oct 2013](/previous-versions/azure/devops/2013/oct-21-team-services)">21 Oct 2013</a></td>
            <td>New account and project pages</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2013/oct-17-team-services" data-raw-source="[17 Oct 2013](/previous-versions/azure/devops/2013/oct-17-team-services)">17 Oct 2013</a></td>
            <td>Build images updated to VS 2013</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/sep-30-team-services" data-raw-source="[30 Sep 2013](/previous-versions/azure/devops/2013/sep-30-team-services)">30 Sep 2013</a></td>
            <td>New languages supported for code syntax highlighting</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td>Color picking in charts</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td>Column options for the test case grid view</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=44911" data-raw-source="[2013.2](https://www.microsoft.com/download/details.aspx?id=44911)">2013.2</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2013/sep-09-team-services" data-raw-source="[9 Sep 2013](/previous-versions/azure/devops/2013/sep-09-team-services)">9 Sep 2013</a></td>
            <td>Work item charts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Bulk edit of test cases</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Delete a team project</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Work items from code discussion</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2013/aug-19-team-services" data-raw-source="[19 Aug 2013](/previous-versions/azure/devops/2013/aug-19-team-services)">19 Aug 2013</a></td>
            <td>Improved code commenting</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/jul-29-team-services" data-raw-source="[29 Jul 2013](/previous-versions/azure/devops/2013/jul-29-team-services)">29 Jul 2013</a></td>
            <td>Improved permission management for Git repos</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Team room Git push events</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Deleting team rooms</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2013/jul-10-team-services" data-raw-source="[10 Jul 2013](/previous-versions/azure/devops/2013/jul-10-team-services)">10 Jul 2013</a></td>
            <td>Backlog mapping</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Team permission changes</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/jun-26-team-services" data-raw-source="[26 Jun 2013](/previous-versions/azure/devops/2013/jun-26-team-services)">26 Jun 2013</a></td>
            <td>Windows 8.1 support in hosted build</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Paste images into work items in the web</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Open Microsoft Test Runner from web</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/jun-19-team-services" data-raw-source="[19 Jun 2013](/previous-versions/azure/devops/2013/jun-19-team-services)">19 Jun 2013</a></td>
            <td>Agile Portfolio Management updates – view filter and quick decompose</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Open MTM from web</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Admin panel color change</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="5"><a href="/previous-versions/azure/devops/2013/jun-03-team-services" data-raw-source="[3 Jun 2013](/previous-versions/azure/devops/2013/jun-03-team-services)">3 Jun 2013</a></td>
            <td>Agile Portfolio Management</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Lightweight code commenting</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Team Room</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Create/modify test plans through Web UI</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Cloud load testing</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/may-28-team-services" data-raw-source="[28 May 2013](/previous-versions/azure/devops/2013/may-28-team-services)">28 May 2013</a></td>
            <td>Build IaaS</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Git alerts</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Backlog updates – name changed to &quot;backlogs&quot; and now backlogs show all items until they reach the completed state</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2013/may-13-team-services" data-raw-source="[13 May 2013](/previous-versions/azure/devops/2013/may-13-team-services)">13 May 2013</a></td>
            <td>Work item colors based on process template settings</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Usability updates – icon updates and sentence casing</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Navigation updates in Web UI, including ability to view past iterations</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Git multi-repo support</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2013/mar-22-team-services" data-raw-source="[22 Mar 2013](/previous-versions/azure/devops/2013/mar-22-team-services)">22 Mar 2013</a></td>
            <td>Branches view for Git</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>TCM Improvements – bulk edit test step pass/fail, double click test step reorder, hover over inline images</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2013/mar-04-team-services" data-raw-source="[4 Mar 2013](/previous-versions/azure/devops/2013/mar-04-team-services)">4 Mar 2013</a></td>
            <td>Customizable Kanban columns</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>TCM improvements – edit test steps when running tests</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Annotate/Blame for version control</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Scheduled builds for Git-based projects</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2013/feb-11-team-services" data-raw-source="[11 Feb 2013](/previous-versions/azure/devops/2013/feb-11-team-services)">11 Feb 2013</a></td>
            <td>Continuous Integration for Git</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>TCM improvements – view test step attachments when running tests, add attachments when running tests, pause, and resume tests in Test Runner</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>WIT tagging cleanup for unused tags</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Download as Zip for version control</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2013/jan-30-team-services" data-raw-source="[30 Jan 2013](/previous-versions/azure/devops/2013/jan-30-team-services)">30 Jan 2013</a></td>
            <td>Work item tagging</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Git support</td>
            <td></td><td><a href="https://go.microsoft.com/fwlink/p/?LinkId=306566" data-raw-source="[2013](https://go.microsoft.com/fwlink/p/?LinkId=306566)">2013</a></td>
        </tr>
        <tr>
            <td>Test Hub in Web UI</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2013/jan-21-team-services" data-raw-source="[21 Jan 2013](/previous-versions/azure/devops/2013/jan-21-team-services)">21 Jan 2013</a></td>
            <td>Changeset context menu in Web UI</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2013/jan-09-team-services" data-raw-source="[9 Jan 2013](/previous-versions/azure/devops/2013/jan-09-team-services)">9 Jan 2013</a></td>
            <td>Account rename of Team Foundation Service account</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="5"><a href="/previous-versions/azure/devops/2013/jan-07-team-services" data-raw-source="[7 Jan 2013](/previous-versions/azure/devops/2013/jan-07-team-services)">7 Jan 2013</a></td>
            <td>Email work items from backlog</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Search for changesets by ID in Web UI</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Full screen mode for code viewing</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Inline diff of images in version control</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Collapsible left pane in all left panels in Web UI</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2012/dec-10-team-services" data-raw-source="[10 Dec 2012](/previous-versions/azure/devops/2012/dec-10-team-services)">10 Dec 2012</a></td>
            <td>Renamed Source to Code in Web UI hub</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Code Explorer updates in Web UI</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Hosted build updates for Azure SDK 1.8, TypeScript 0.8.1, and VS 2012 Update 1</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2012/nov-19-team-services" data-raw-source="[19 Nov 2012](/previous-versions/azure/devops/2012/nov-19-team-services)">19 Nov 2012</a></td>
            <td>Send work items in email from TFS web access</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td>Build file counts and sizes in summary reports</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.2](https://www.microsoft.com/download/details.aspx?id=36392)">2012.2</a></td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2012/oct-31-team-services" data-raw-source="[31 Oct 2012](/previous-versions/azure/devops/2012/oct-31-team-services)">31 Oct 2012</a></td>
            <td>General availability of Team Foundation Service</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2012/oct-29-team-services" data-raw-source="[29 Oct 2012](/previous-versions/azure/devops/2012/oct-29-team-services)">29 Oct 2012</a></td>
            <td>Build drops</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td><a href="/previous-versions/azure/devops/2012/oct-08-team-services" data-raw-source="[8 Oct 2012](/previous-versions/azure/devops/2012/oct-08-team-services)">8 Oct 2012</a></td>
            <td>400 character server paths for version control</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2012/sep-17-team-services" data-raw-source="[17 Sep 2012](/previous-versions/azure/devops/2012/sep-17-team-services)">17 Sep 2012</a></td>
            <td>Drag/drop in sprint planning to assign to person or activity</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td>Web usability improvements (tabs and UX modified, collapse left pane in work items)</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td>Process template updates to Agile 6.1 and Scrum 2.1</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td rowspan="4"><a href="/previous-versions/azure/devops/2012/aug-27-team-services" data-raw-source="[27 Aug 2012](/previous-versions/azure/devops/2012/aug-27-team-services)">27 Aug 2012</a></td>
            <td>Improved source browsing, viewing, and searching</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td>Improved source &quot;diff&quot;</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td>Hosted builds of SharePoint components</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td>Basic authentication support</td>
            <td></td><td>N/A</td>
        </tr>
        <tr>
            <td rowspan="3"><a href="/previous-versions/azure/devops/2012/aug-13-team-services" data-raw-source="[13 Aug 2012](/previous-versions/azure/devops/2012/aug-13-team-services)">13 Aug 2012</a></td>
            <td>Kanban board</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td>Cumulative Flow Diagram</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td>WIP Limits</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td rowspan="2"><a href="/previous-versions/azure/devops/2012/aug-06-team-services" data-raw-source="[6 Aug 2012](/previous-versions/azure/devops/2012/aug-06-team-services)">6 Aug 2012</a></td>
            <td>Drag/drop in task board to move tasks between people and stories</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
        <tr>
            <td>Azure continuous deployment summary report</td>
            <td></td><td><a href="https://www.microsoft.com/download/details.aspx?id=36392" data-raw-source="[2012.1](https://www.microsoft.com/download/details.aspx?id=36392)">2012.1</a></td>
        </tr>
    </tbody>
</table>

## Azure DevOps Server


## Azure DevOps Server Build Numbers


> [!NOTE]
> TFS 2015 RTM has multiple build numbers, due to the componentized nature of its build and packaging process. The number of the installer, which will show up in Add/Remove Programs, is 14.0.23129.01. The number of the majority of the assemblies, which will show up in the TFS Administration Console, is 14.0.23128.00.

<table>
<thead>
        <tr>
          <th>Release</th>
          <th>Date</th>
          <th>Build</th>
        </tr>
</thead>
<tbody>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2022?view=azure-devops&preserve-view=true" data-raw-source="[2022 RTW](/azure/devops/server/release-notes/azuredevops2022)">2022 RTW</a></td>
          <td>December 6, 2022</td>
          <td>19.205.33122.1</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2022?view=azure-devops&preserve-view=true" data-raw-source="[2022 RC2](azure/devops/server/release-notes/azuredevops2022?view=azure-devops&preserve-view=true#azure-devops-server-2022-rc2-release-date-october-25-2022)">2022 RC2</a></td>
          <td>October 25, 2022</td>
          <td>19.205.33011.1</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2022?view=azure-devops&preserve-view=true" data-raw-source="[2022 RC1](azure/devops/server/release-notes/azuredevops2022?view=azure-devops&preserve-view=true#azure-devops-server-2022-rc1-release-date-august-9-2022)">2022 RC1</a></td>
          <td>August 9, 2022</td>
          <td>19.205.32728.1</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2020u1?view=azure-devops#azure-devops-server-2020-update-12-release-date-may-17-2022&preserve-view=true" data-raw-source="[2020.1.2 RTW](/azure/devops/server/release-notes/azuredevops2020u1?view=azure-devops#azure-devops-server-2020-update-12-release-date-may-17-2022)">2020.1.2</a></td>
          <td>May 17, 2022</td>
          <td>18.181.32404.7</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2020?view=azure-devops#azure-devops-server-202002-release-date-may-17-2022&preserve-view=true" data-raw-source="[2020.0.2 RTW](/azure/devops/server/release-notes/azuredevops2020?view=azure-devops#azure-devops-server-202002-release-date-may-17-2022)">2020.0.2</a></td>
          <td>May 17, 2022</td>
          <td>18.170.32404.6</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2020u1?view=azure-devops-2020&preserve-view=true" data-raw-source="[2020.0.1 RTW](/azure/devops/server/release-notes/azuredevops2020u1?view=azure-devops-2020&preserve-view=true)">2020.1.1</a></td>
          <td>August 26, 2021</td>
          <td>18.181.31626.1</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2020u1?view=azure-devops&preserve-view=true" data-raw-source="[2020.0.1 RTW](/azure/devops/server/release-notes/azuredevops2020u1?view=azure-devops&preserve-view=true)">2020.1</a></td>
          <td>May 25, 2021</td>
          <td>18.181.31230.2</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2020?view=azure-devops&preserve-view=true" data-raw-source="[2020.0.1 RTW](/azure/devops/server/release-notes/azuredevops2020?view=azure-devops&preserve-view=true)">2020.0.1</a></td>
          <td>January 19, 2021</td>
          <td>18.170.30910.2</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2020?view=azure-devops-2020&preserve-view=true" data-raw-source="[2020 RTW](/azure/devops/server/release-notes/azuredevops2020?view=azure-devops-2020&preserve-view=true)">2020</a></td>
          <td>Oct. 6, 2020</td>
          <td>18.170.30525.1</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2019u1" data-raw-source="[2019.1](/azure/devops/server/release-notes/azuredevops2019u1)">2019.1.1</a></td>
          <td>Dec. 10, 2019</td>
          <td>17.153.29522.3</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2019u1" data-raw-source="[2019.1](/azure/devops/server/release-notes/azuredevops2019u1)">2019.1</a></td>
          <td>Aug. 20, 2019</td>
          <td>17.153.29207.5</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2019" data-raw-source="[2019.0.1](/azure/devops/server/release-notes/azuredevops2019)">2019.0.1</a></td>
          <td>May 21, 2019</td>
          <td>17.143.28912.1</td>
        </tr>
        <tr>
          <td><a href="/azure/devops/server/release-notes/azuredevops2019" data-raw-source="[2019 RTW](/azure/devops/server/release-notes/azuredevops2019)">2019 RTW</a></td>
          <td>Mar. 5, 2019</td>
          <td>17.143.28621.4</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update3" data-raw-source="[2018.3.2](/visualstudio/releasenotes/tfs2018-update3)">2018.3.2 Rerelease</a></td>
          <td>Feb. 6, 2019</td>
          <td>16.131.28601.4</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update3" data-raw-source="[2018.3.2](/visualstudio/releasenotes/tfs2018-update3)">2018.3.2</a></td>
          <td>Jan. 15, 2019</td>
          <td>16.131.28507.4</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update3" data-raw-source="[2018.3.1](/visualstudio/releasenotes/tfs2018-update3)">2018.3.1</a></td>
          <td>Nov 11, 2018</td>
          <td>16.131.28226.3</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update3" data-raw-source="[2018.3](/visualstudio/releasenotes/tfs2018-update3)">2018.3</a></td>
          <td>Sep. 12, 2018</td>
          <td>16.131.28106.2</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update2" data-raw-source="[2018.2](/visualstudio/releasenotes/tfs2018-update2)">2018.2</a></td>
          <td>May 7, 2018</td>
          <td>16.131.27701.1</td>
        </tr>
         <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update1" data-raw-source="[2018.1.2](/visualstudio/releasenotes/tfs2018-update1)">2018.1.2</a></td>
          <td>Nov. 27, 2018</td>
          <td>16.122.28313.3</td>
        </tr>
         <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update1" data-raw-source="[2018.1.1](/visualstudio/releasenotes/tfs2018-update1)">2018.1.1</a></td>
          <td>Sep. 12, 2018</td>
          <td>16.122.28028.4</td>
        </tr>
         <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-update1" data-raw-source="[2018.1](/visualstudio/releasenotes/tfs2018-update1)">2018.1</a></td>
          <td>Feb. 20, 2018</td>
          <td>16.122.27409.2</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2018-relnotes" data-raw-source="[2018 RTW](/visualstudio/releasenotes/tfs2018-relnotes)">2018 RTW</a></td>
          <td>Nov. 15, 2017</td>
          <td>16.122.27102.1</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2017-update3" data-raw-source="[2017.3.1](/visualstudio/releasenotes/tfs2017-update3)">2017.3.1</a></td>
          <td>Feb. 28, 2018</td>
          <td>15.117.27414.0</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2017-update3" data-raw-source="[2017.3](/visualstudio/releasenotes/tfs2017-update3)">2017.3</a></td>
          <td>Nov. 6, 2017</td>
          <td>15.117.27024.0</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2017-update2" data-raw-source="[2017.2](/visualstudio/releasenotes/tfs2017-update2)">2017.2</a></td>
          <td>Jul. 24, 2017</td>
          <td>15.117.26714.00</td>
        </tr>
        <tr>
          <td>2017.1</td>
          <td>Mar. 9, 2017 (Mar. 7, 2017)</td>
          <td><a href="/visualstudio/releasenotes/tfs2017-update1#build-doesnt-work-when-upgrading-to-tfs-2017-update-1-build-15112263010-from-tfs-2013-or-earlier" data-raw-source="[15.112.26307.00
          (15.112.26301.0)](/visualstudio/releasenotes/tfs2017-update1#build-doesnt-work-when-upgrading-to-tfs-2017-update-1-build-15112263010-from-tfs-2013-or-earlier)">15.112.26307.00
          (15.112.26301.0)<em></a></td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2017-relnotes" data-raw-source="[2017.0.1](/visualstudio/releasenotes/tfs2017-relnotes)">2017.0.1</a></td>
          <td>Feb. 28, 2018</td>
          <td>15.105.27412.0</td>
        </tr><br/>        <tr>
          <td>2017 RTM</td>
          <td>Nov. 16, 2016</td>
          <td>15.105.25910.00</td>
        </tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2015-update4-vs" data-raw-source="[2015.4.2](/visualstudio/releasenotes/tfs2015-update4-vs)">2015.4.2</a></td>
          <td>Apr. 9, 2019</td>
          <td>14.114.28805.0</td>
        </tr>
        <tr>
        <tr>
          <td><a href="/visualstudio/releasenotes/tfs2015-update4-vs" data-raw-source="[2015.4.1](/visualstudio/releasenotes/tfs2015-update4-vs)">2015.4.1</a></td>
          <td>Feb. 28, 2018</td>
          <td>14.114.26412.0</td>
        </tr>
        <tr>
          <td>2015.4</td>
          <td>Apr. 11, 2017</td>
          <td>14.114.26403.0</td>
        </tr>
        <tr>
          <td>2015.3</td>
          <td>Jun. 27, 2016</td>
          <td>14.102.25423.00</td>
        </tr>
        <tr>
          <td>2015.2</td>
          <td>May 5, 2016</td>
          <td>14.95.25122.00</td>
        </tr>
        <tr />
        <tr>
          <td>2015.1</td>
          <td>Nov. 30, 2015</td>
          <td>14.0.24720.00</td>
        </tr>
        <tr>
          <td>2015 RTM</td>
          <td>Aug. 6, 2015</td>
          <td>14.0.23128.00</em></td>
        </tr>
        <tr>
          <td>2013.5</td>
          <td>Jul. 19, 2015</td>
          <td>12.0.40629.0</td>
        </tr>
        <tr>
          <td>2013.4</td>
          <td>Nov. 11, 2014</td>
          <td>12.0.31101.00</td>
        </tr>
        <tr>
          <td>2013.3</td>
          <td>Aug. 4, 2014</td>
          <td>12.0.30723.00</td>
        </tr>
        <tr>
          <td>2013.2</td>
          <td>Apr. 2, 2014</td>
          <td>12.0.30324.00</td>
        </tr>
        <tr>
          <td>2013 RTM</td>
          <td>Nov. 18, 2013</td>
          <td>12.0.21005.01</td>
        </tr>
        <tr>
          <td>2012.4</td>
          <td>Nov. 12, 2013</td>
          <td>11.0.61030.0</td>
        </tr>
        <tr>
          <td>2012.3</td>
          <td>Jun. 26, 2013</td>
          <td>11.0.60610.01</td>
        </tr>
        <tr>
          <td>2012.2</td>
          <td>Apr. 4, 2013</td>
          <td>11.0.60315.01</td>
        </tr>
        <tr>
          <td>2012.1</td>
          <td>Dec. 12, 2012</td>
          <td>11.0.51106.01</td>
        </tr>
        <tr>
          <td>2012 RTM</td>
          <td>Aug. 15, 2012</td>
          <td>11.0.50727.01</td>
        </tr>
      </tbody>
    </table>


## How to provide feedback

We would love to hear what you think about these features. Report any problems or suggest a feature through [Developer Community](https://developercommunity.visualstudio.com/spaces/21/index.html).

> [!div class="mx-imgBorder"] 
> ![Make a suggestion](media/help-make-a-suggestion.png)

You can also get advice and your questions answered by the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/azure-devops).
