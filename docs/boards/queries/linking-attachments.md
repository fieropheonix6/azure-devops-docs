---
title: Query work items by link or attachment count in Azure Boards  
titleSuffix: Azure Boards
description: Learn how to query work items based on link type, link count, link restrictions, and attached file count in Azure Boards.
ms.custom: boards-queries, engagement-fy23
ms.service: azure-devops-boards
ms.assetid: 219717a0-de6e-4f70-8558-54f813f82507
ms.author: chcomley
author: chcomley
ms.topic: example-scenario
monikerRange: '<= azure-devops'
ms.date: 09/06/2024
---

# Query work items by link or attachment count  

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]

You can [link work items to track related work and dependencies](../backlogs/add-link.md) and attach files to share information with your team. You can then list work items based on one or more of the following fields:

::: moniker range="azure-devops"  
Attached File Count | (Discussion) Comment Count | External Link count| Hyperlink Count| Link Comment| Related Link Count|Remote Link Count
::: moniker-end 

::: moniker range="< azure-devops" 
- Attached File Count
- (Discussion) Comment Count 
- External Link count
- Hyperlink Count
- Link Comment
- Related Link Count
::: moniker-end 

For more information about these fields, see the [table provided later in this article](#table-field). 

## Prerequisites

[!INCLUDE [prerequisites-queries](../includes/prerequisites-queries.md)]

## Supported operators and macros 

Clauses that specify an integer field can use the following operators.

`= , <> , > , < , >= , <= ,`  
`=[Field], <>[Field], >[Field], <[Field], >=[Field], <=[Field],`   
`In, Not In,`   
`Was Ever`  

<a id="tree"></a>

## List hierarchical items in a tree view  

Add a query and select **Tree of work items** to begin your query. You should see something similar to the following examples: 

#### [Browser](#tab/browser/)

:::image type="content" source="media/query-link-attach-all-items-tree-query.png" alt-text="Screenshot of Query Editor, Tree Query, web portal.":::

#### [Visual Studio 2015](#tab/visual-studio/)

:::image type="content" source="media/link-attachments/tree-query-te.png" alt-text="Screenshot of Query Editor, Tree Query, Team Explorer.":::

***
> [!NOTE]
> You can't construct a query that shows a hierarchical view of Test Plans, Test Suites, and Test Cases. These items aren't linked together using parent-child link types. But, you can create a direct links query that lists test-related work items. Also, you can [view the hierarchy through the Test Plans page](../../test/create-a-test-plan.md). 

## Options for filters and query clauses

Change the filter options for linked work items and add query clauses via the following options. 

:::row:::
   :::column span="":::
     **Filter for**
   :::column-end:::
   :::column span="":::
      **Include these query clauses**
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
     Only child items of work item 645
   :::column-end:::
   :::column span="":::
      **Add to Filters for top-level work items:**  
      `ID  =  645`
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
     Tasks or bugs
   :::column-end:::
   :::column span="":::
      **Add to Filters for linked work items:**  
      `Work Item Type  In  Task,Bug`
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
     Items assigned to my team (Web)
   :::column-end:::
   :::column span="":::
      **Add to both top and bottom filters:**  
      `Assigned to  In Group  [Fabrikam Fiber]\Web`  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
     Parent items of tasks assigned to me
   :::column-end:::
   :::column span="":::
      Change Filter options to **Match linked work items first**  
      **Add to Filters for linked work items:**  
      `Assigned To = @Me`
   :::column-end:::
:::row-end:::

<a id="dependents"></a>

## List items based on linked dependents  

The following example shows a dependent linked query that returns items with dependencies on work managed by other teams and projects. 

#### [Browser](#tab/browser/)

The following query finds work items in all projects that are linked to work items under the **Fabrikam** area path and project using Predecessor and Successor link types.

:::image type="content" source="media/link-attachments/direct-links-query-web-portal.png" alt-text="Screenshot of Query Editor, Work items, and direct links, Web portal.":::

- Check the **Query across projects** checkbox to enable all dependent linked work items that match the filter criteria to be listed, no matter which project they belong to.
- Specify the **Area Path Under Fabrikam** clause to find only work items that are linked to work items defined under the Fabrikam project.   
- Specify **Only return items that have matching links**, and **Return selected link types** to return only work items that are linked based on the **Predecessor** and **Successor** link types.  


#### [Visual Studio 2015](#tab/visual-studio/)

Use this type of query to list all dependent work items that link to active Product Backlog Items or Bugs that aren't removed, closed, or completed. Only those dependent work items that are under a product area other than the **Phone Save\Phone Customers** are returned.

![Work Items and Dependent Links Query](media/example-work-item-queries/IC588290.png)   

- Remove the **Team Project = @Project** to enable all dependent linked work items that match the filter criteria to be listed, no matter which project they belong to in the collection.
- Group each of two clauses to return all **Product Backlog Item**s on the backlog or in progress, and the second grouped clause returns all **Bug**s on the backlog or in progress.
- Group the two clauses with the **OR** operator at the start of the second clause to return work items that match either of the two filter criteria.
- Choose the **Only return items that have the specified links** to return only top-level work items that have dependencies.
- Choose **Return links of any type** to return all linked work items that match the filter criteria for linked work items, in this case, returning all work items that aren't under the **Phone Saver\\Phone Customers** area path, and aren't completed or removed.

The following image shows the query results.

![Screenshot of Direct links query results.](media/example-work-item-queries/IC588291.png)  

***
<a id="orphan-stories"></a>

## List orphan user stories 

If you typically organize your user stories under features, you can quickly find them by doing the following steps.

1. Open the product backlog and turn on the **Parents On** view option. 
2. Scroll down to the section that lists **Unparented Stories** (Agile) or **Unparented Backlog items** (Scrum).

:::image type="content" source="media/link-attachments/list-orphan-stories.png" alt-text="Screenshot of List orphan stories or backlog items.":::

Or, you can find unparented backlog items using a **Work items and direct links** query. For example, the following query lists active user stories for the Azure DevOps team that don't have a Parent link. 

:::image type="content" source="media/link-attachments/unparented-work-items.png" alt-text="Screenshot of Query Editor, Work items, and direct links, Web portal, unparented user stories.":::
<a id="table-field"></a>
<a id="fields"></a>

## Fields associated with links and attachments

The following table describes fields associated with links and attachments. Most of these fields don't appear within the work item form, but get tracked for all work item types. 

:::row:::
   :::column span="1":::
   **Attached File Count**
   :::column-end:::
   :::column span="3":::
   The number of files attached to the work item and stored in the work item tracking database.  
   Reference Name=System.AttachedFileCount, Data type=Integer  
   > [!NOTE]
   > For Azure Boards (cloud service), you can add up to 100 attachments to a work item. Attempts to add more result in an error message upon saving the work item.  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   **Comment Count**
   :::column-end:::
   :::column span="3":::
   The number of comments added to the **Discussion** section of the work item.  
   Reference Name=System.CommentCount, Data type=Integer  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="external-link-count"></a>

   **External Link Count**

   :::column-end:::
   :::column span="3":::
   The number of links from the work item to artifacts that aren't work items, such as pull requests, commits, changesets, or other link types.  
   Reference Name=System.ExternalLinkCount, Data type=Integer
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="hyper-link-count"></a>

   **Hyperlink Count**

   :::column-end:::
   :::column span="3":::
   The number of hyperlinks that are defined for the work item.

   Reference Name=System.HyperLinkCount, Data type=Integer
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   **Link Comment**
   :::column-end:::
   :::column span="3":::
   Contains comments from the team member who created the link. You can configure this field to appear as a column in a list of links on a work item form. (Not supported in query editor.)  

   Reference Name=System.Links.Comment, Data type=PlainText
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::

   **Link Description**

   :::column-end:::
   :::column span="3":::
   Contains the work item type, ID, and title of the work item that is the target of the link. You can configure this field to appear as a column in a list of links on a work item form. (Not supported in query editor.) 

   Reference Name=System.Links.Description, Data type=PlainText
   :::column-end:::
:::row-end:::
::: moniker range=">= azure-devops-2022" 
:::row:::
   :::column span="1":::
   <a id="parent"></a>

   **Parent**

   :::column-end:::
   :::column span="3":::
   When included as a column option in a backlog or query results list, the **Title** of the parent work item is displayed. Internally, the system stores the **ID** of the work item within an Integer field. 
   > [!NOTE]
   > You can add the **Parent** field as a column or specify it within a query clause by specifying the parent work item ID.   
   Reference Name=System.Parent, Data type=Integer
   :::column-end:::
   :::column span="1":::
   All
   :::column-end:::
:::row-end:::
::: moniker-end 
::: moniker range="azure-devops-2020" 
:::row:::
   :::column span="1":::
   <a id="parent"></a>

   **Parent**

   :::column-end:::
   :::column span="3":::
   When included as a column option in a backlog or query results list, the **Title** of the parent work item is displayed. Internally, the system stores the **ID** of the work item within an Integer field. 
   > [!NOTE]
   > The **Parent** field is available from Azure DevOps Server 2020 and later versions. You can't specify this field within a query clause.   
   Reference Name=System.Parent, Data type=Integer
   :::column-end:::
:::row-end:::
::: moniker-end 
:::row:::
   :::column span="1":::
   <a id="related-link-count"></a>

   **Related Link Count**

   :::column-end:::
   :::column span="3":::
   The number of links defined for a work item that use a work link type, such as Parent-Child, Predecessor-Successor, and Related. For a full list, see  [Link type reference](link-type-reference.md).  
   Reference Name=System.RelatedLinkCount, Data type=Integer
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
   <a id="remote-link-count"></a>

   **Remote Link Count**

   :::column-end:::
   :::column span="3":::
   Available for Azure DevOps Services only. The number of links from a work item to work items defined in another organization. The same Microsoft Entra ID must manage the organizations. Supported link types include Consumes From, Produced For, and Remote Related. For more information, see [Add link to work items, Link to a remote work item](../backlogs/add-link.md).  
   Reference Name=System.RemoteLinkCount, Data type=Integer
   :::column-end:::
:::row-end:::

## Related content

- [Add a link to multiple work items](../backlogs/add-link.md) 
- [Link work items to other objects](../backlogs/add-link.md) 
- [Query quick reference](query-index-quick-ref.md)
- [Query editor](using-queries.md)   
- [Query fields, operators, and macros](query-operators-variables.md)   
- [Work item field index](../work-items/guidance/work-item-field.md) 

::: moniker range="< azure-devops" 

### Visualize related work and other objects 

You can view related work items and objects within a work item with the [Work item visualization extension](https://marketplace.visualstudio.com/items?itemName=ms-devlabs.WorkItemVisualization) available from the Visual Studio Marketplace, Azure DevOps tab.

### Add custom link types or customize the links controls 

To add link types, see [Manage link types [witadmin]](/previous-versions/azure/devops/reference/witadmin/manage-link-types). 

All tabs that support creating links between work items are implemented by using the **LinksControl** element on the work item form. This element controls filtering and restricting the types of work items to which you can link. It also controls the types of links that you can create and whether you can link work items in another project. To customize the link controls and restrictions, you modify the definition of the `LinksControlOptions` for a work item type, see [LinksControlOptions XML elements](/previous-versions/azure/devops/reference/xml/linkscontroloptions-xml-elements?view=tfs-2017&preserve-view=true).  

### Default data fields in lists of links

You can add or remove columns from the list of links, and you can customize the default columns and the column order. For more information, see [LinksControlOptions XML elements](/previous-versions/azure/devops/reference/xml/linkscontroloptions-xml-elements?view=tfs-2017&preserve-view=true).

::: moniker-end 
