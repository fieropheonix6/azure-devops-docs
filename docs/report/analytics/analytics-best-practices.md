---
title: Analytics best practices
titleSuffix: Azure DevOps  
description: Learn about the best practices to use when you query Analytics for Azure DevOps.
ms.subservice: azure-devops-analytics
ms.author: chcomley
author: chcomley
ms.topic: overview
monikerRange: "<=azure-devops"
ms.date: 11/02/2023
ms.custom:
  - analytics
  - sfi-image-nochange
---

# Analytics best practices 

[!INCLUDE [version-gt-eq-2019](../../includes/version-gt-eq-2019.md)] 

Analytics is the reporting platform for Azure DevOps, which allows you to gain insights from your data and make data-driven decisions. Analytics is optimized for fast read-access and server-based aggregations, and it provides various tools to visualize and analyze your data. In this article, we share some best practices for using Analytics in Azure DevOps.

[!INCLUDE [prerequisites-simple](../includes/analytics-prerequisites-simple.md)]
- If you're an extension developer, make sure to review [OData Analytics query guidelines](../extend-analytics/odata-query-guidelines.md).

## Get familiar with the Analytics metadata 

Query the Analytics metadata to gain familiarity with the entity types, entity sets, properties, and enumerated lists. For more information, see [Query the Analytics service](analytics-query-parts.md), [Analytics OData metadata](../extend-analytics/analytics-metadata.md), and [Entities and properties reference for Azure Boards](entity-reference-boards.md). 

## Structure your query to return the data you need 

To query the minimum data set you need to create your report, follow these practices:   

- [Choose the entity set that supports the report your want to create](#entityset)
- [Specify query parts in the order they're executed](#order)
- [Limit the columns you request in your query](#limit-columns)
- [Create preview queries](#preview)
- [Limit queries to projects you have access to](#limit-projects)

<a id="entityset"></a>

### Choose the entity set to support your report

While there are several `EntitySets` supported in the Analytics data model, only a few are used to generate reports.`EntitySets` used to build reports fall into three categories: 

- **Current**: Contains information about the current configuration of the `EntityTypes` contained within the `EntitySet`. 
- **Snapshot**: Composite entities that combine historical and date-related data. Snapshot entities are intended to be used to support aggregation reports.  
- **Revision**: Contains historical information. For example, `WorkItemRevision` maintains data about the history of work items. 

Here's a quick reference for the EntityTypes to specify to support reports. For a description of each of these EntityTypes, see [Data model for Analytics](../extend-analytics/data-model-analytics-service.md). 

|Azure DevOps data | Current        | Snapshot                  | Revision       | 
|------------------|----------------|---------------------------|----------------|   
|Azure Boards | `WorkItems`  | `WorkItemSnapshot`<br/>`WorkItemBoardSnapshot` | `WorkItemRevisions` | 
|Azure Pipelines | `Pipelines`<br/>`PipelineTasks`  | `ParallelPipelineJobsSnapshot`<br/>`PipelineRuns`, `PipelineRunActivityResults` |  | 
|Azure Pipelines and Tests | `TestResultsDaily` |  `TestRuns`        | 
|Azure Test Plans | `Tests`<br/>`TestConfiguration`<br/>`TestPoints`<br/>`WorkItems` | `TestResultsDaily`<br/>`TestPointHistorySnapshot` |  | 

<a id="order"></a>

### Specify query parts in the order they're executed 

The recommended order for the various query parts is to specify them in the following order, which is the order in which they're evaluated. For a description of each query part, see [Query the Analytics service, Query options](analytics-query-parts.md#query-options).
 
1. `$apply`
1. `$filter`
1. `$orderby`
1. `$expand`
1. `$select`
1. `$skip`
1. `$top`

All queries must contain an `$apply` or `$select` clause, otherwise you might receive a warning message. 

<a id="limit-columns"></a>

### Limit the columns you request in your query 

You specify columns of data to return using the `$select` clause. With customization, work items can have numerous fields associated with them. The more properties or fields that a query references, the more expensive it's to process. Consider the report you want to generate and make sure you're only requesting the fields you need.  

For example, to return the ID, Work Item Type, Title, and State fields for a filtered set of work items, specify the following `$select` clause: `$select=WorkItemId, WorkItemType, Title, State`.  

To look up the list of properties and their corresponding field names, see [Entities and properties reference for Azure Boards](../analytics/entity-reference-boards.md). 

<!--- General info 
Analytics is built on top of a Columnstore Index technology. That means that data is both storage and query processing is column-based. So, the more properties that a query references, the more expensive it's to process. 
-->

<a id="preview"></a>

### Create preview queries

Preview queries are queries that return a single record or small subset of records. By creating a preview query, you can refine your query to ensure that you're requesting the data that you need. By starting with a minimal query, you can build up your query to ensure that you're specifying the records you want and the column data you need. 

By using the `apply=aggregate($count as Count)`, you can identify the number of records you're requesting. For example, the following syntax queries the number of work items for the *Fabrikam Fiber* project. 

> [!div class="tabbedCodeSnippets"]
```OData
https://analytics.dev.azure.com/content-learn/Content/_odata/v4.0-preview/WorkItems? $apply=aggregate($count as Count)
```

The response returns a total of 1415 work items. 

> [!div class="tabbedCodeSnippets"]
```OData
{
  "@odata.context": "https://analytics.dev.azure.com/fabrikam/Fabrikam Fbier/_odata/v4.0-preview/$metadata#WorkItems(Count)",
   "value": [
  {
     "@odata.id": null,
   "Count": 1415
  }
  ]
}
```

<a id="limit-projects"></a>

### Limit queries to projects you have access to 

Project-scope queries return information about a single project, whereas organization-scope queries are designed to return information that cross project boundaries. Organization scoped queries require broader user permissions or careful scoping restrictions to ensure that your query isn't blocked due to a lack of project permissions. 

If you have access to one or more projects, but not all projects, and you submit an organization-scoped query, you receive an error message.

`"VS403496: The query results include data in one or more projects for which you do not have access. Add one or more projects filters to specify the project(s) you have access to in 'WorkItems' entity. If you're using $expand or navigation properties, project filter is required for those entities. More information can be found here: https://go.microsoft.com/fwlink/?LinkId=786441."`

For more information, see [Project and organization-scoped queries](../extend-analytics/account-scoped-queries.md).

## Review warning and error messages  

Analytics reviews each query it receives for violations to its rules. It returns warning messages when it detects a violation. We recommend that you review these messages to correct or improve the query structure. 

::: moniker range="azure-devops" 

## Rate limits and throttling 

Queries made to Analytics for Azure DevOps Services are subject to rate limits. If too  many queries are sent that request the return of large amounts of data within a short time frame, the service might be subject to throttling. For more information, see [Rate and usage limits](../../integrate/concepts/rate-limits.md).

You can review usage for the service and for individuals by going to **Organization Settings>Usage** and exercising the filters. For example, the following image shows the usage by *Jamal Hartnett* to the Analytics service. 

:::image type="content" source="media/best-practices/usage-analytics.png" alt-text="Screenshot of Usage page for a single user and Analytics.":::

::: moniker-end
 
## Related articles

- [What is the Analytics service?](../powerbi/what-is-analytics.md)
- [Construct OData queries for Analytics](analytics-query-parts.md)
- [Analytics OData metadata](../extend-analytics/analytics-metadata.md) 
- [OData Analytics query guidelines](../extend-analytics/odata-query-guidelines.md)
