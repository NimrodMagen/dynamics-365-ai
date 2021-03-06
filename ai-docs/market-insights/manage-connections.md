---
title: "Manage connections in Market Insights | Microsoft Docs"
description: "Learn how to get started with connections to other services."
keywords: "connect, connections, integration, dynamics 365"
ms.date: 10/31/2018
ms.service: dynamics-365-ai
ms.topic: get-started-article
ms.assetid: 79184579-61c0-425c-b7fd-28cc663dfa58
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

# Manage connections in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]

(This topic is pre-release documentation and is subject to change.)

[!INCLUDE[Dynamics 365 Market Insights](../includes/pn-market-insights-long.md)] lets admins connect to and share social data with other applications. To work with social data in other applications, you can connect them on the **Connections** page in the [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] Settings area. The type of connection you create depends on the application you want to connect to.  
  
 ![connections page in the Microsoft Dynamics 365 Market Insights settings area](media/settings-on-connections-page.png "Connections page in the Microsoft Dynamics 365 Market Insights Settings area")  
  
- Connect to [!INCLUDE[pn_microsoft_azure_event_hubs](../includes/pn-microsoft-azure-event-hubs.md)] and stream posts that match a data set as events from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] to an event hub. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Stream data from Market Insights to Microsoft Azure Event Hubs](stream-data-to-event-hubs.md)  
  
- Connect to [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] to create new [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] records from posts found in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Link posts from Market Insights to Dynamics 365](link-posts-to-dynamics-365.md)  
  
- Manage a list of domains that allow applications to connect with and request data from your [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] solution. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Connect Market Insights to other domains](connect-other-domains.md)  
  
  - To display [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] widgets in [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)], you need to connect [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] to [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  For [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] to be able to connect to [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], its domain must be allowed in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Integrate Market Insights with Dynamics 365](integrate-widgets-dynamics-365.md)  

  - If you want to import [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] data to [!include[](../includes/pn-customer-insights-full.md)], you can add [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] as a data source. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Add Market Insights as a data source](https://docs.microsoft.com/dynamics365/customer-engagement/customer-insights/deploy/datasourcemse)
  
### See also  
 [Administer Market Insights](settings-administration.md)
