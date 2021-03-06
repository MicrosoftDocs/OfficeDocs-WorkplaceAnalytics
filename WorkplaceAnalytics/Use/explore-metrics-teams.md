---
# Metadata Sample
# required metadata

title: Explore Teams metrics in Workplace Analytics
description: Overview of Teams collaboration metrics in Workplace Analytics
author: madehmer
ms.author: v-midehm
ms.date: 06/20/2019
ms.topic: article
localization_priority: normal 
ms.prod: wpa

---

# Teams collaboration

**Teams collaboration** in **Explore** shows communication trends about and insights into how your organization's employees use Teams for communication and collaboration. You can select what collaboration data to analyze on this page, either Teams' calls, instant messages, or both.

![Teams collaboration](../images/wpa/use/teams-explore.png)

To open **Teams collaboration**:

1. Open the [Workplace Analytics](https://workplaceanalytics.office.com) Home page. If prompted, sign in with your work account.
2. In the left navigation pane, select **Analyze** and then select **Explore**.
3. In **Explore**, select **Teams collaboration**.

## Call hours

The **Call hours** graph shows the average and total number of hours each group spent in calls as initiators or participants, through Teams, including scheduled and unscheduled calls during and outside of working hours (as set in Outlook).

![Teams call hours](../images/wpa/use/teams-explore-calls.png)

## Instant messaging hours

The **Instant messaging hours** graph shows average and total number of hours each group spent sending or receiving instant messages (IMs) through Teams, including IMs during and outside of working hours (as set in Outlook).

![Teams IMs](../images/wpa/use/teams-explore-ims.png)

## Filters for Teams

You can use the **Call hours** and **IM hours** filters in the Charts and in Page Settings to filter and view Teams data in Explore.

![Teams filters](../images/wpa/use/teams-filters.png)

## Data sources includes Teams

As part of Office 365 data, the **Data sources** page also provides a summary of Teams data that you can use to evaluate collaboration data levels over a given time period. It provides a view of average weekly call hours and instant messaging hours over time. The **Last refreshed** date shows when data was most recently processed.

Analysts can use these views to evaluate communication and collaboration trends and patterns for your organization.

![Teams summary in Data sources](../images/wpa/Use/teams-data-source.png)

## Teams data in queries

You can also include and analyze data about Teams calls and instant messages in Person queries and data for Teams calls in Meeting queries. For example, you can customize a person or meeting query to show internal as compared to external number of calls.

For Meeting queries, meeting hours and related meeting metrics will include data about scheduled and unscheduled calls in Teams.

The following table provides details about Teams metrics in Person queries.

### Teams metrics in Person queries

|Metric|Description|Query type|Data type|Customizable|
|------|-----------|----------|---------|------------|
|Calls| Total number of calls the person spent time in as initiator or participant, through Teams, during and outside of working hours.| Person| Count| Yes |
|IMs | Total number of instant messages (IMs) or chats sent by the person as the initiator, through Teams, during and outside of working hours. Note: Time in IM compose estimated to 22 seconds, Time in IM read estimated to 8 seconds| Person| Count| Yes|
|Time in calls after hours | Number of hours the person spent in calls, through Teams, outside of working hours. For calls that started during working hours, this number only includes the part of the call that occurred outside of that person’s work schedule (as set in Outlook).| Person| Hour| Yes|
|Time in IMs after hours| Number of hours the person spent in reading/sending Instant Messages in  Teams, outside of that person’s working hours. Note: Time in IM compose estimated to 22 seconds, Time in IM read estimated to 8 seconds| Person| Hour| Yes|
|Total call hours | Total number of hours the person spent in calls as initiator or participant, through Teams, including scheduled and impromptu calls during and outside of working hours (as set in Outlook). | Person| Hour| Yes|
|Total IM hours | Total number of hours the person spent in IMs as initiator or participant, through Teams, including scheduled and impromptu IMs during and outside of working hours (as set in Outlook).  Note: Time in IM compose estimated to 22 seconds, Time in IM read estimated to 8 seconds.| Person| Hour| Yes|
|Working hours in calls| Total number of hours a person spent time in scheduled and unscheduled calls with Teams, during working hours. | Person| Hour| Yes|

## Related topics

* [Explore page settings](../use/explore-page-settings.md)
* [Person queries](../tutorials/Person-queries.md)
* [Meeting queries](../tutorials/Meeting-queries.md)
* [Workplace Analytics Charts](../use/chart-types.md)
* [Metric descriptions](../use/metric-definitions.md)
