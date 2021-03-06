---
# Metadata Sample
# required metadata

title: Use the auto-refresh option for queries in Workplace Analytics 
description: Describes the auto-refresh option for queries in Workplace Analytics.     
author: paul9955
ms.author: v-pascha
ms.date: 08/12/2019
ms.topic: article
localization_priority: normal 
ms.prod: wpa
---

# Auto-refresh option for queries

## One-time queries show you a snapshot

As an analyst, you can run different kinds of queries in Workplace Analytics, including person, meeting, group-to-group, and person-to-group queries to get a snapshot of workplace behavior. 

You can run a query as a one-time event where you set it up, run it one time, and get the results. To visualize workplace patterns uncovered by this query, you can load the results into a data analysis tool, such as Power BI or Excel.

## Auto-refresh shows you trends over time

Query results, especially when viewed in a data analysis tool, can uncover dynamic patterns. These patterns evolve over time because the workplace behavior of employees evolves over time. To isolate one instance of evolving workplace behavior over time, you can use the applicable query multiple times, on a regular schedule. To do this, you can use the auto-refresh feature for Workplace Analytics queries.

## Create a query with the auto-refresh option

> [!Note] 
> Generally, an organization can have a maximum of 20 auto-refresh queries. For more information, see [Maximum number of auto-refresh queries](#maximum-number-of-auto-refresh-queries).

[!INCLUDE [To create an auto-refresh query](../Includes/to-create-auto-refresh-query.md)]

## Stop the auto-refresh option

Follow these steps only for a query that has already run and for which auto-refresh is currently in effect. 

1. In Workplace Analytics, open the **Queries > Results** page.
2. In the row of the query, select the ellipsis.
3. In the option menu, select **Turn off auto-refresh**: 

   ![Turn off auto-refresh](../images/wpa/tutorials/auto-refresh-options-on-48.png)

## Start/re-start the auto-refresh option

Follow these steps only for a query that has already run and for which auto-refresh is not currently in effect.  

1. In Workplace Analytics, open the **Queries > Results** page.
2. In the row of the query, select the ellipsis.
3. In the option menu, select **Turn on auto-refresh**: 

   ![Turn on auto-refresh](../images/wpa/tutorials/auto-refresh-options-off-48.png)

Alternatively, you can renew an auto-refresh query in the [notifications panel](../use/wpa-notifications.md) on the Workplace Analytics Home page.    

## Auto-refresh details

### Basic behavior

 * When you create the query, you run it for the first time. As it runs, it uses data from the exact date range that you defined.

 * The query automatically runs again, once for every time period that you selected (such as week or month). Each run coincides with the date on which Workplace Analytics refreshes mail and calendar data from Microsoft Exchange.

 * Each time the query runs automatically, its date range advances by one unit of the time period that you selected (such as week or month). That is,both its start date and its end date shift shift to a later date by the same amount of time.  

### Auto-refresh stop, restart, and expiration

 * You can start or stop auto-refresh for a query at any time. See [Stop the auto-refresh option](#stop-the-auto-refresh-option) and [Start/re-start the auto-refresh option](#startre-start-the-auto-refresh-option). 

 * The auto-refresh option of a query expires after two months. This expiration period applies after your _initial_ setting of the auto-refresh option and also after each _renewal_ of the auto-refresh option.
 
 The **Is Recurring** column on the **Queries > Results** page shows whether auto-refresh is currently turned on for the query represented by that row:

   ![Turn off auto-refresh status](../images/wpa/tutorials/auto-status-48.png) 

 * After auto-refresh expires for a query, you can renew it. See [Start/re-start the auto-refresh option](#startre-start-the-auto-refresh-option).  

 * Deleting a query for which auto-refresh is turned on stops all future auto-refresh runs of that query. 

### Maximum number of auto-refresh queries

Generally, an organization can have a maximum of 20 auto-refresh queries. If your organization has already reached this limit and you need a new auto-refresh query, you have the following options: 
 * Delete an existing auto-refresh query or turn auto-refresh off for a query (on the **Queries > Results** page). Then, create your new auto-refresh query.
 * Contact Workplace Analytics to request additional auto-refresh queries. To do this, follow the instructions in the "Workplace Analytics Support" row under [Get support](../overview/getting-support.md).

<!-- [AUGUST 14 2019] COMMENT THIS NOTE OUT UNTIL PARTITIONS ARE RELEASED. PER NITHIN, THAT COULD BE MONTHS FROM NOW. 
> [!Note] 
> Auto-refresh queries respect partitions. (A partition is a data workspace for an analyst.) This means that if other analysts&mdash;who work within their own partitions&mdash;have created a total of fifteen auto-refresh queries, five auto-refresh queries remain for you to use. 
-->

## View query results with the auto-refresh option

On the **Analyze** > **Queries** > **Results** page, find your query in the results table, which includes the following:

* The results (a .csv file) of the _latest_ weekly run. You can select **Download** to download an archived file of these results.
* The date on which the query last ran.
* An icon that indicates it as a query with the auto-refresh option.

## Auto-refresh query results in Power BI

On the **Results** page, you can copy a link to the query results and then use it in Power BI.

1. To the right of the query's row, select **Copy link**:

   ![Copy a query's results link](../images/wpa/tutorials/Get-results-link.png)

2. Select **Copy**. The Get results link dialog box displays the word "Copied."
3. In Power BI, on the Home tab, select **Get Data**, and then select **OData feed**.
4. In the **OData feed** dialog box, paste the link that you copied into the URL field:

   ![OData feed in Power BI](../images/wpa/tutorials/OData-feed.png)

5. Select **OK**.
6. Enter your client credentials, and then select **Connect**.

After you do this, Power BI maintains a connection to this query in Workplace Analytics. In the future, to visualize the query's current results, open the Workplace Analytics project in Power BI and select **Refresh**.

### Related topics

[View, download, and export query results](../use/view-download-and-export-query-results.md)