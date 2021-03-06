---
title: "Analytics for sources in Market Insights | Microsoft Docs"
description: "Learn how to focus your analysis on the various data sources in Market Insights."
keywords: "sources, analytics, twitter, reddit, facebook, news, blogs, youtube, forums, rss"
ms.date: 10/31/2018
ms.service: dynamics-365-ai
ms.topic: article
ms.assetid: cafd302e-97bc-4e0c-81db-fa032a5b3b90
author: m-hartmann
ms.author: mhart
manager: shellyha
ms.custom: dyn365-ai-marketinsights
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365SE
---

# Analyze sources of posts in your data set

(This topic is pre-release documentation and is subject to change.)

Understand which social media sources are found most often in your search topics and analyze sources, such as top languages and user sentiment.  
  
In [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], go to **Analytics** > **Sources** to see details about the sources of posts in your data set.  

![screenshot of the sources page in the analytics area of market insights](media/analytics-sources.png "Screenshot of the sources page in the Analytics area of Market Insights")
    
## Activities

Shows the post type (post, reply, share, retweet) based on volume.

## Authors

The normal view of this widget shows the top five authors and sources, based on the volume of posts and trend indicator. Select the **Full view** button ![full view button](media/open-full-view-icon.png "Full view button") to expand the widget and see more details such as reach, source, and location for the 100 most-active authors and their posts.    
To add a filter for multiple authors at once, select the check boxes on the left side of the list for all authors that you want to include. Then select **INCLUDE** in the list header. To remove an author from the authors filter, select the check boxes on the left side of the list for all authors that you want to remove from the filter. Then select **EXCLUDE** in the list header.
> [!NOTE]
> Full view also has a **Delete** button ![delete button](media/trashbin-icon.png "Delete button") you can use to [delete a selected author](manage-authors.md) and the author’s posts. You must have a **Power Analyst** or **Administrator** user role to delete an author.
>  When you delete an author, none of the author’s previous posts will be available; they are permanently deleted. No new posts from this author will be acquired in the future.  
  
## Authors by source

Authors by source shows the most active sources and summarizes how many authors posted in other sources.

## Languages

Lists the five most-used languages based on the volume of posts and trend indicator.

## Location insights

Displays the posts with location information on a map to show where posts are coming from. You can also [define an activity map](activity-maps.md) to see new posts in real time, with additional functionality. 

Dynamic widget. Shows only if posts contain location information in the selected data set.

## Phrases by sources

Lists top phrases for the top five sources based on volume.

## Sources

Shows the number of posts from the most active sources and summarizes how many posts were found in other sources.    
Click the **Full view** button ![full view button](media/open-full-view-icon.png "Full view button") to expand the widget for additional details.  
  
## Sources by sentiment

Lists the top five sources along with sentiment index and trend indicator.  

## Sources history

Displays the volume of posts from different sources in a selected time frame. 

## Volume change by source

Shows the change in post volume for the top five sources compared to previous periods and trend indicator.

### See Also  

[Analyze social data using widgets](analyze-social-data-using-widgets.md)   
[Get to know your filters](use-filters.md)    
[Explore more options with your data set](more-options-with-data-set.md)    
