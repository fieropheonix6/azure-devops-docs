---
title: Allowed address lists and network connections
titleSuffix: Azure DevOps
description: Add IP addresses and domain URLs to the allowlist for Azure DevOps and troubleshoot network connections.
ms.topic: reference
ms.subservice: azure-devops-security
ms.reviewer: jominana
ms.author: chcomley
author: chcomley
monikerRange: '<= azure-devops'
ms.date: 07/02/2025
---

# Allowed IP addresses and domain URLs

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]

If your organization is secured with a firewall or proxy server, you must add certain internet protocol (IP) addresses and domain uniform resource locators (URLs) to the **allowlist**. Adding these IPs and URLs to the allowlist helps to ensure that you have the best experience with Azure DevOps. You know that you need to update your allowlist if you can't access Azure DevOps on your network.

**Required ports:**
- **Port 443 (HTTPS)**: Required for all Azure DevOps web access, REST API calls, and most service connections
- **Port 22 (SSH)**: Required only for Git operations using SSH protocol

See the following sections in this article:

- [Allowed domain URLs](#allowed-domain-urls)
- [IP addresses and range restrictions](#ip-addresses-and-range-restrictions)

> [!TIP]
> So that Visual Studio and Azure Services work well with no network issues, open select ports and protocols. For more information, see [Install and use Visual Studio behind a firewall or proxy server, Use Visual Studio and Azure Services](/visualstudio/install/install-and-use-visual-studio-behind-a-firewall-or-proxy-server#use-visual-studio-and-azure-services).

<a id="range-restrictions"></a>

## IP addresses and range restrictions

::: moniker range="azure-devops"

### Outbound connections

_Outbound connections_ target other dependent sites. Examples of such connections include:

- Browsers connecting to Azure DevOps website as users go to and use features of Azure DevOps
- Azure Pipelines agents installed on your organization's network connecting to Azure DevOps to poll for pending jobs
- CI events sent from a source code repository hosted within your organization's network to Azure DevOps

Ensure the following IP addresses are allowed for outbound connections on **port 443 (HTTPS)**, so your organization works with any existing firewall or IP restrictions. The endpoint data in the following chart lists requirements for connectivity from a machine in your organization to Azure DevOps Services.

#### [IP V4 ranges](#tab/IP-V4)

```IP V4 ranges

13.107.6.0/24
13.107.9.0/24
13.107.42.0/24
13.107.43.0/24
150.171.22.0/24 
150.171.23.0/24 
150.171.73.0/24 
150.171.74.0/24 
150.171.75.0/24 
150.171.76.0/24
```

#### [IP V6 ranges](#tab/IP-V6)

```IP V6 ranges

2620:1ec:4::/48
2620:1ec:a92::/48
2620:1ec:21::/48
2620:1ec:22::/48
2620:1ec:50::/48 
2620:1ec:51::/48 
2603:1061:10::/48
```

---

If you're currently allowing the `13.107.6.183` and `13.107.9.183` IP addresses, leave them in place, as you don't need to remove them.

> [!NOTE]
> [Azure Service Tags](/azure/virtual-network/service-tags-overview) aren't supported for *outbound* connections.

::: moniker-end

### Inbound connections

_Inbound connections_ originate from Azure DevOps and target resources within your organization's network. Examples of such connections include:

- Azure DevOps Services connecting to endpoints for [Service Hooks](../../service-hooks/overview.md)  
- Azure DevOps Services connecting to customer-controlled SQL Azure VMs for [Data Import](../../migrate/migration-overview.md)  
- Azure Pipelines connecting to on-premises source code repositories such as [GitHub Enterprise](../../pipelines/repos/github-enterprise.md) or [Bitbucket Server](../../pipelines/repos/on-premises-bitbucket.md)  
- Azure DevOps Services [Audit Streaming](../audit/auditing-streaming.md) connecting to on-premises or cloud-based Splunk

Ensure the following IP addresses are allowed for inbound connections on **port 443 (HTTPS)**, so your organization works with any existing firewall or IP restrictions. The endpoint data in the following chart lists requirements for connectivity from Azure DevOps Services to your on-premises or other cloud services.

> [!div class="mx-tdCol2BreakAll"]  
> |  Geography | Region  | IP V4 ranges |  
> |------|------|---------|  
> | Australia | Australia East | 20.37.194.0/24 |  
> |  | Australia South East | 20.42.226.0/24 |  
> | Brazil | Brazil South | 191.235.226.0/24 |  
> | Canada | Central Canada | 52.228.82.0/24 |
> | Asia Pacific | Southeast Asia (Singapore) | 20.195.68.0/24 |
> | India | South India | 20.41.194.0/24 |
> |  | Central India | 20.204.197.192/26 |  
> | United States | Central United States | 20.37.158.0/23 |  
> |  | West Central United States | 52.150.138.0/24 |
> |  | East United States   | 20.42.5.0/24 |  
> |  | East 2 United States  | 20.41.6.0/23 |
> |  | North United States  | 40.80.187.0/24 |  
> |  | South United States   | 40.119.10.0/24 |
> |  | West United States  | 40.82.252.0/24 |  
> |  | West 2 United States | 20.42.134.0/23 |
> |  | West 3 United States | 20.125.155.0/24 |  
> | Europe | Western Europe | 40.74.28.0/23 |
> |  | North Europe | 20.166.41.0/24 |
> | United Kingdom | United Kingdom South | 51.104.26.0/24 |  

Azure Service Tags are supported only for *inbound* connections. Instead of allowing the previously listed IP ranges, you may use the **AzureDevOps** service tag for Azure Firewall and Network Security Group (NSG) or on-premises firewall via a JSON file download.  

> [!NOTE]
> The Service Tag or previously mentioned inbound IP addresses don't apply to Microsoft Hosted agents. Customers are still required to allow the [entire geography for the Microsoft Hosted agents](../../pipelines/agents/hosted.md#agent-ip-ranges). If allowing the entire geography is a concern, we recommend using the [Microsoft Managed DevOps Pools](../../managed-devops-pools/overview.md). Alternatively, you can also use [Azure Virtual Machine Scale Set agents](../../pipelines/agents/scale-set-agents.md). Managed DevOps Pools and Scale Set agents are a form of self-hosted agents that can be auto-scaled to meet your demands.  
Hosted macOS agents are hosted in GitHub's macOS cloud. IP ranges can be retrieved using the [GitHub metadata API](https://docs.github.com/en/rest/reference/meta#get-github-meta-information) using the instructions provided [here](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#ip-addresses).

### Other IP addresses

Most of the following IP addresses pertain to Microsoft 365 Common and Office Online.

```Microsoft365Common&OfficeIPs

40.82.190.38
52.108.0.0/14
52.237.19.6
52.238.106.116/32
52.244.37.168/32
52.244.203.72/32
52.244.207.172/32
52.244.223.198/32
52.247.150.191/32
```

For more information, see [Worldwide endpoints](/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide&preserve-view=true#microsoft-365-common-and-office-online) and [Adding IP address rules](/azure/app-service/app-service-ip-restrictions#adding-ip-address-rules).

### Azure DevOps ExpressRoute connections

If your organization uses ExpressRoute, ensure the following IP addresses are allowed for both outbound and inbound connections on **port 443 (HTTPS)**.

#### [IP V4 ranges](#tab/IP-V4)

```IP V4 ranges
13.107.6.175/32
13.107.6.176/32
13.107.6.183/32
13.107.9.175/32
13.107.9.176/32
13.107.9.183/32
13.107.42.18/32
13.107.42.19/32
13.107.42.20/32
13.107.43.18/32
13.107.43.19/32
13.107.43.20/32
150.171.73.14/32
150.171.73.15/32
150.171.73.16/32
150.171.74.14/32
150.171.74.15/32
150.171.74.16/32
150.171.75.14/32
150.171.75.15/32
150.171.75.16/32
150.171.76.14/32
150.171.76.15/32
150.171.76.16/32
150.171.22.17/32
150.171.22.18/32
150.171.22.19/32
150.171.23.17/32
150.171.23.18/32
150.171.23.19/32
```

#### [IP V6 ranges](#tab/IP-V6)

```IP V6 ranges
2620:1ec:a92::175/128
2620:1ec:a92::176/128
2620:1ec:a92::183/128
2620:1ec:4::175/128
2620:1ec:4::176/128
2620:1ec:4::183/128
2620:1ec:21::18/128
2620:1ec:21::19/128
2620:1ec:21::20/128
2620:1ec:22::18/128
2620:1ec:22::19/128
2620:1ec:22::20/128
2603:1061:10::14/128
2603:1061:10::15/128
2603:1061:10::16/128
2603:1061:10:1::14/128
2603:1061:10:1::15/128
2603:1061:10:1::16/128
2603:1061:10:2::14/128
2603:1061:10:2::15/128
2603:1061:10:2::16/128
2603:1061:10:3::14/128
2603:1061:10:3::15/128
2603:1061:10:3::16/128
2620:1ec:50::17/128
2620:1ec:50::18/128
2620:1ec:50::19/128
2620:1ec:51::17/128
2620:1ec:51::18/128
2620:1ec:51::19/128
```

---

For more information about Azure DevOps and ExpressRoute, see [ExpressRoute for Azure DevOps](https://devblogs.microsoft.com/devops/expressroute-for-azure-devops/).

## Allowed Domain URLs

Network connection issues could occur because of your security appliances, which might be blocking connections - Visual Studio uses TLS 1.2 and above. When you're using [NuGet](#nuget-connections) or connecting from Visual Studio 2015 and later, update the security appliances to support TLS 1.2 and above for the following connections.

**Port requirements for domain URLs:**
- **Port 443 (HTTPS)**: Required for all domain URLs listed in this article
- **Port 22 (SSH)**: Required only for SSH Git connections (see [SSH connections](#ssh-connections) section)

To ensure your organization works with any existing firewall or IP restrictions, ensure that `dev.azure.com` and `*.dev.azure.com` are open on **port 443**.

The following section includes the most common domain URLs to support sign in and licensing connections.

```CommonDomainURLs

https://dev.azure.com
https://*.dev.azure.com
https://aex.dev.azure.com
https://aexprodea1.vsaex.visualstudio.com
https://*.vstmrblob.vsassets.io
https://amp.azure.net
https://app.vssps.dev.azure.com
https://app.vssps.visualstudio.com
https://*.vsblob.visualstudio.com
https://*.vssps.visualstudio.com
https://*.vstmr.visualstudio.com
https://azure.microsoft.com
https://go.microsoft.com
https://graph.microsoft.com
https://login.microsoftonline.com
https://management.azure.com
https://management.core.windows.net
https://microsoft.com
https://microsoftonline.com
https://static2.sharepointonline.com
https://visualstudio.com
https://vsrm.dev.azure.com
https://*.windows.net
https://{organization_name}.visualstudio.com
https://{organization_name}.vsrm.visualstudio.com
https://{organization_name}.vstmr.visualstudio.com
https://{organization_name}.pkgs.visualstudio.com
https://{organization_name}.vssps.visualstudio.com

Azure DevOps uses the following URL to provide the agent software for download for self-hosted agents.
https://download.agent.dev.azure.com

Azure DevOps uses content delivery network (CDN) to serve static content. The following URLs are part of that. 
https://cdn.vsassets.io
https://*.vsassets.io
https://*.gallerycdn.vsassets.io
https://aadcdn.msauth.net
https://aadcdn.msftauth.net
https://amcdn.msftauth.net
https://azurecomcdn.azureedge.net
```

The following endpoints are used to authenticate Azure DevOps organizations using a Microsoft Account (MSA). 
These endpoints are only needed for Azure DevOps organizations backed by Microsoft Accounts (MSA). 
Azure DevOps organizations backed a Microsoft Entra tenant doesn't need the following URLs.

```
https://live.com 
https://login.live.com 
```

The following URL is required if you're migrating from Azure DevOps Server to the cloud service using our data migration tool.
```
https://dataimport.dev.azure.com
```

> [!NOTE]
> Azure DevOps uses Content Delivery Networks (CDNs) to serve static content. Users in **China** should also add the following domain URLs to an allowlist:
>
> ``` NuGetDomainURLs
> https://*.vsassetscdn.azure.cn
> https://*.gallerycdn.azure.cn
> ```

We recommend you open port `443` to all traffic on the following IP addresses and domains. We also recommend you open port `22` to a smaller subset of targeted IP addresses.

**Port configuration summary:**
- **Port 443 (HTTPS)**: Open to ALL domain URLs and IP addresses listed in this article
- **Port 22 (SSH)**: Open only to SSH-specific hosts listed in the [SSH connections](#ssh-connections) section

|More domain URLs |Descriptions |Required Port |
|---------|---------|---------|
|https://login.microsoftonline.com |Authentication and sign-in related |443 |
|https://*.vssps.visualstudio.com   |Authentication and sign-in related |443 |
|https://*.gallerycdn.vsassets.io   |Hosts Azure DevOps extensions |443 |
|https://*.vstmrblob.vsassets.io | Hosts Azure DevOps TCM log data |443 |
|https://cdn.vsassets.io    | Hosts Azure DevOps Content Delivery Networks (CDNs) content |443 |
|https://static2.sharepointonline.com    | Hosts some resources that Azure DevOps uses in "office fabric" UI kit for fonts, and so on |443 |
|https://vsrm.dev.azure.com   | Hosts releases |443 |
|https://download.agent.dev.azure.com      |  Required to set up self-hosted agent in machines within your network |443 |
|https://amp.azure.net   | Needed for deploying to Azure app service |443 |
|https://go.microsoft.com  | Accesses go links |443 |

### Azure Artifacts

Ensure the following domain URLs are allowed for Azure Artifacts:

```AzureArtifactsDomainURLs
https://*.blob.core.windows.net
https://*.visualstudio.com
https://*.dedup.microsoft.com
```

Also allow all IP addresses in the "name": "Storage.{region}" section of the following file (updated weekly): [Azure IP ranges and Service Tags - Public Cloud](https://aka.ms/aax7d4q). {region} is the same Azure Geography as your organization.

### NuGet connections

Ensure the following domain URLs are allowed for NuGet connections:

``` NuGetDomainURLs
https://*.azurewebsites.net
https://*.nuget.org
```

> [!NOTE]
> Privately owned NuGet server URLs might not be included in the previous list. You can check the NuGet servers you're using by opening `%APPData%\Nuget\NuGet.Config`.

### SSH connections

If you need to connect to Git repositories on Azure DevOps with SSH, allow requests to **port 22** for the following hosts:

```SSHDomainHosts

ssh.dev.azure.com
vs-ssh.visualstudio.com
```

Also allow **port 22** for IP addresses in the "name": "AzureDevOps" section of [this downloadable file](https://aka.ms/aax7d4q) (updated weekly) named: **Azure IP ranges and Service Tags - Public Cloud**

### Azure Pipelines Microsoft-hosted agents

If you use Microsoft-hosted agent to run your jobs and you need the information about what IP addresses are used, see [Microsoft-hosted agents IP ranges](../../pipelines/agents/hosted.md#agent-ip-ranges). See all [Microsoft Managed DevOps Pools](../../managed-devops-pools/overview.md) and [Azure Virtual Machine Scale Set agents](../../pipelines/agents/scale-set-agents.md?preserve-view=true&view=azure-devops).

For more information about hosted Windows, Linux, and macOS agents, see [Microsoft-hosted agent IP ranges](../../pipelines/agents/hosted.md#agent-ip-ranges).

### Azure Pipelines self-hosted agents

If you're running a firewall and your code is in Azure Repos, see [Self-hosted Linux agents FAQs](../../pipelines/agents/linux-agent.md#im-running-a-firewall-and-my-code-is-in-azure-repos-what-urls-does-the-agent-need-to-communicate-with), [Self-hosted macOS agents FAQs](../../pipelines/agents/osx-agent.md#im-running-a-firewall-and-my-code-is-in-azure-repos-what-urls-does-the-agent-need-to-communicate-with) or [Self-hosted Windows agents FAQs](../../pipelines/agents/windows-agent.md#im-running-a-firewall-and-my-code-is-in-azure-repos-what-urls-does-the-agent-need-to-communicate-with). This article has information about which domain URLs and IP addresses your private agent needs to communicate with.

> [!IMPORTANT]
> [Edgio CDN for Azure DevOps was retired](https://devblogs.microsoft.com/devops/important-switching-cdn-providers/), which required a new domain URL to be allow-listed in firewall rules for agent software download.
> The new domain to allowlist for agent download is `https://*.dev.azure.com`. If your firewall rules don't allow wildcards, use `https://download.agent.dev.azure.com`.
> 
> The Azure DevOps team recommended making this change by the following date:
> - May 1, 2025 for Azure DevOps Services
> - May 15, 2025 for Azure DevOps Server
>
> For more information, see [CDN Domain URL change for Agents in Pipelines](https://devblogs.microsoft.com/devops/cdn-domain-url-change-for-agents-in-pipelines/).

## Azure DevOps import service

During the import process, we highly recommend that you restrict access to your virtual machine (VM) to only IP addresses from Azure DevOps. To restrict access, allow only connections from the set of Azure DevOps IP addresses,  which were involved in the collection database import process. For information about identifying the correct IP addresses, see [(Optional) Restrict access to Azure DevOps Services IPs only](../../migrate/migration-import-large-collections.md#ips).

> [!NOTE]
> Azure DevOps doesn't natively support allowlisting directly within its settings. However, you can manage allowlisting at the network level using your organization's firewall or proxy settings. 

## Related content

- [Available service tags](/azure/virtual-network/service-tags-overview)
- [Microsoft-hosted agents IP address ranges](../../pipelines/agents/hosted.md#agent-ip-ranges)
- [Self-hosted Windows agents FAQs](../../pipelines/agents/windows-agent.md)
- [Configure Azure Storage firewalls and virtual networks](/azure/storage/common/storage-network-security?toc=%2Fazure%2Fvirtual-network%2Ftoc.json&tabs=azure-portal)
- [Install and use Visual Studio behind a firewall or proxy server](/visualstudio/install/install-and-use-visual-studio-behind-a-firewall-or-proxy-server#use-visual-studio-and-azure-services)
