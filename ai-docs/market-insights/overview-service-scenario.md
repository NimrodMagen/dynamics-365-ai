---
title: "Customer service scenarios for Market Insights | Microsoft Docs"
description: "Review service scenarios to get inspiration for how to efficiently leverage Market Insights in your organization."
keywords: "service scenario, overview, customer service, social customer service"
ms.date: 04/01/2019
ms.service: dynamics-365-ai
ms.topic: article
ms.assetid: ba7e7205-7c76-49ee-abfe-bffdd1365209
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

# Address customer service scenarios on social media with [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]

(This topic is pre-release documentation and is subject to change.)

Do you want to offer fast, powerful support to your customers on social channels? This overview suggests ways you and your team can use [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] to address your customers' service requests on social media. [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] lets you keep track of requests and adds intelligence on top of this tracking. You can answer customers directly in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] or link them to [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] for further tracking.

## Prerequisites

- [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] is [set up](settings-administration.md).

- [Search topics are configured](set-up-searches.md) and data acquisition is up and running.

- You have the required [user roles and permissions](user-roles.md) assigned in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].

## Social customer care scenario overview

The following steps describe an end-to-end configuration for social customer care. Review the steps and decide which are relevant for your customer care scenario.

1. [Enable service reps to engage with customers via social media](#manage-social-profiles-to-participate-in-conversations) by adding and sharing social profiles and streams.

2. Before you start engaging with customers, you need to [create a search topic](set-up-searches.md) with rules that gather all posts that address your organization's social profiles. For example, if you added a Twitter or Facebook page profile, make sure you [allow the acquisition of private messages](manage-access-tokens.md#tokens-for-interactions-with-posts) and [create search rules](add-rules-search-topic.md) that gather private messages and all post types for the profile.

3. [Add tags, automatically and manually](#use-intelligence-to-boost-productivity), and learn how automated intention analysis can help triage incoming posts. Let [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] do some of your work for you.

4. [Collaborate with your team](#establish-workflows-and-collaborate-with-other-users) and make sure they address the right customer issue with the intended priority.

> [!NOTE]
> Some of these capabilities can be automated. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Route posts using automation rules](automation-rules.md)

## Manage social profiles to participate in conversations

 Learn how to add and share social profiles and streams in Social Center, how to keep them up and running, and how to enable users to post on behalf of your organization.

1. [Add a new social profile](manage-social-profiles.md).

2. [Share a social profile](manage-social-profiles.md#share-a-social-profile-with-other-users).

3. [Create](social-center.md#configure-a-stream) and [share a stream](social-center.md#share-a-stream).

4. [Keep social profiles up and running](social-profiles-health-state.md).

## Use intelligence to boost productivity

Let [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] work for you. Find out how you can add tags to important posts, automatically or manually, and learn how intention analysis can help triage incoming posts and how to automate this process.

- [Define a new tag](tags.md#add-custom-tags) so you can add it to posts.

- Let the system learn from the tags you added and [automate the tagging of posts](tags.md#promote-custom-tags-to-auto-tags).

- Get [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] to [find the intentions in posts](tags.md#how-intention-analysis-works) to enable quick triage of large number of posts. For example, you can route support requests to your service reps.  
  To further increase efficiency, you can automate the routing of posts by using [automation rules](automation-rules.md).

## Create support cases in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] from social posts

Save time and minimize repetitive activities. [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] lets you create new records in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] directly from a post within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. For example, you can create a case and assign it so the right service rep in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] so they review and solve the case efficiently.

1. Get an [overview](link-posts-to-dynamics-365.md) of the [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] integration.

2. [Set up the connection](connect-dynamics-365-record-creation.md) to [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)].

3. [Set up record details](create-dynamics-365-record-from-social-post.md) for cases.

4. [Create a case from a post](create-dynamics-365-record-from-social-post.md) in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].

## Establish workflows and collaborate with other users

Collaborate with your team and make sure they prioritize the right issues.

1. [Assign posts](work-with-posts.md#assign-a-post-to-other-users) to other users to distribute work across the team.

2. [Share streams](social-center.md#share-a-stream) with other users so they can work on posts in near&ndash;real time.

3. [Add labels](work-with-posts.md#add-a-label-to-a-post) to posts to route them to specific streams.

> [!NOTE]
> [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] leverages Office 365 Groups to enable collaboration with groups of people. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Work with Office 365 Groups in Market Insights](office-365-groups.md)

## Customer stories

- [UK banking disrupted: Metro Bank reinvents customer service with Microsoft](https://customers.microsoft.com/story/uk-banking-disrupted-metro-bank-reinvents-customer-ser)

- [5 tips to help your business weather changes in the financial services industry](https://customers.microsoft.com/story/5-tips-to-help-your-business-weather-changes-in-the-fi)

### See also

[Connect Dynamics 365 and Market Insights](connect-dynamics-365-record-creation.md)   
[Link posts from Market Insights to Dynamics 365](link-posts-to-dynamics-365.md)   
[Work with posts](work-with-posts.md)
