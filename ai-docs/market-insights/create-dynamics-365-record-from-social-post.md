---
title: "Create a record from a post in Market Insights | Microsoft Docs"
description: "Learn how to send posts found in Market Insights to Dynamics 365 to create new lead or case records."
keywords: "Link to Dynamics 365, Link to CRM, link post, record details, social activity, entity, entities"
ms.date: 10/31/2018
ms.service: dynamics-365-ai
ms.topic: article
ms.assetid: b1341b83-efc9-4ed3-b5c3-b26e814f3f72
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

# Create a Dynamics 365 record from a social post

(This topic is pre-release documentation and is subject to change.)

Send a post found with [!INCLUDE[Dynamics 365 Market Insights](../includes/pn-market-insights-long.md)] to your [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] instance to create a record. For example, you can automatically convert posts to cases for customer service, or to leads for your sales team. When you create a social activity, if the author of the post doesn’t have a social profile in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)], the system creates a social profile and contact record, and then links the social profile with the contact record. When a record is created in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)], you can see the details about this record in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  
Learn about the [prerequisites to establish a connection with Dynamics 365](connect-dynamics-365-record-creation.md#prerequisites-to-establish-a-connection-with-dynamics-365) on how to configure your online and on-premises [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] instance to connect with [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].

## Specify record details

You can define the information to show in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record details when a record in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] is created from a social post. Depending on your selection, [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] fields shows the information about the connected instance and selected entity. To familiarize yourself with the social activity record type or the [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record creation and update rules feature, see [MSDN: SocialActivity entity messages and methods](https://msdn.microsoft.com/library/dn689062.aspx), [CRM Help & Training: Set up rules to automatically create or update records in CRM](https://go.microsoft.com/fwlink/p/?LinkID=624394).  

Define the fields of a [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] entity that you want to display in **Dynamics 365 Record Details** in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] when a record of the same entity is created from a post. Add the fields you want to see in the **Dynamics 365 Record Details** when you define the entity details in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].    
[!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] lets you select the record type to create when linking a new post to [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)]. Depending on the settings in **Entity Details**, you can see the current values of the [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] when you load the record details for a post that was linked before.   

> [!NOTE]
> Only the custom entities in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] which are in relationship with the Social Activity entity are visible in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. For more information, see [TechNet: Create and edit entity relationships](https://technet.microsoft.com/library/dn531171.aspx).

### Define or edit fields for record details

1. In [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], go to **Settings** > **Connections** > **Microsoft Dynamics 365**.  

2. In the **Microsoft Dynamics 365 Connections** pane, select the [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] instance that you want to define entity details for.  

3. In the **Dynamics 365 Instance** pane, select the record type under **Record details**.  

4. In the **Entity Details** pane, select the [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] fields to show in the **Dynamics 365 Record Details** form for the selected entity. Or click **Add** ![add button](media/add-icon.png "Add button") to add more fields.  

5. Reorder the fields using the up arrow ![reorder dynamics 365 entity attributes up](media/arrow-up-icon.png "Reorder Dynamics 365 entity attributes up") or down arrow ![reorder dynamics 365 entity attributes down](media/arrow-down-icon.png "Reorder Dynamics 365 entity attributes down") or remove fields using the **Remove** button ![delete button](media/delete-icon.png "Delete button").  

   ![entity details](media/arrange-entity-details-for-linked-records.png "Entity details")  

   > [!IMPORTANT]
   >  You can't remove an entity if there are active automation rules using that entity. You will first need to deactivate or delete all automation rules using that entity. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Route posts using automation rules](automation-rules.md)  

6. To apply your changes, in the **Dynamics 365 Instance** pane, click **Save** ![save button](media/save-icon.png "Save button").  

## Convert a [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] post to a social activity

1. In [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], click **Posts** on any Analytics page to see the posts list.  

    --OR--  

    Go to **[!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]** > **Social Center** to see your streams.  

2. Go to the post you want to convert to a social activity record in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)], and then click **Link to Dynamics 365** ![link to dynamics 365 button in market insights](media/link-to-record-icon.png "Link to Dynamics 365 button in Market Insights").  

> [!NOTE]
> The **Link to Dynamics 365** feature doesn't support [!INCLUDE[pn_crm_2016](../includes/pn-crm-2016.md)] (on-premises) in combination with the [!include[](../includes/pn-internet-explorer.md)] or [!include[](../includes/pn-microsoft-edge.md)] browsers.

   ![link to dynamics 365 button in market insights](media/link-post-to-dynamics-365.png "Link to Dynamics 365 button in Market Insights")  

3. Select from the available instances, and then select the record type you want to create from the **Entity** drop-down list. The **Entity** drop-down list shows only those entities that are configured in the **Dynamics 365 Instance** panel in the **Dynamics 365 Record Details** section. If a single entity is configured with an instance, it will be selected by default.  

   ![select instance and entity](media/create-record-in-dynamics-365.png "Select instance and entity")  

4. Add any additional information, up to 250 characters, related to the record in **Notes**, and then click **Create**.  

    The post now displays a **Linked** button ![link to dynamics 365 button in market insights](media/link-to-record-icon.png "Link to Dynamics 365 button in Market Insights") along with the name of the [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] instance it is linked to.  

   ![linked button by a post in market insights](media/post-linked-to-dynamics-365.png "Linked button by a post in Market Insights")  

> [!TIP]
> - To automatically create records in [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] from social posts that match a specific data set, you can create automation rules. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Route posts using automation rules](automation-rules.md)  
> - If the linked [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] instance has [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] system settings set to disabled, the link creation fails and shows this error message: "Dynamics 365 can’t receive social data from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]". Contact your [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] administrator to review the Disable [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] system settings. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [TechNet: Control social data](https://go.microsoft.com/fwlink/p/?LinkId=723352)  
> - If [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] allows incoming social activities, but no rules are configured to create [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] entities out of them, the linking operation does succeed. However, opening link details in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] will provide details about the social activiy only. Contact your [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] administrator if this happens. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [CRM Help & Training: Set up rules to automatically create or update records in CRM](https://go.microsoft.com/fwlink/p/?LinkID=624394)  

## Configure Dynamics 365 to automatically create records from linked posts

By default, [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] creates a Social Activity entity when a post is linked from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. In [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)], you can convert this entity to a different record type. To automate the process, you can set up Automatic Record Creation Rules in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] to automatically create records from incoming social activities.  

To learn more about the social activity record type or the [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record creation and update rules feature, see [MSDN: SocialActivity entity messages and methods](https://msdn.microsoft.com/library/dn689062.aspx), [CRM Help & Training: Set up rules to automatically create or update records in CRM](https://go.microsoft.com/fwlink/p/?LinkID=624394).  

## Understand the data sent to Dynamics 365 when you create a social activity

When you create a social activity, [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] sends the social payload as a JSON object to the **Additional Parameters** field of a social activity. The payload can be used as channel properties that define conditions for rules, and for setting properties of the record you're creating or updating. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [CRM Help & Training: Set up rules to automatically create or update records in CRM](https://go.microsoft.com/fwlink/p/?LinkID=624394) The payload contains the most important fields required by [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] to consume tweets and [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] posts. These fields contain information about the post that was sent: author, content, URI to the original post, URI to the post in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], and some additional post metadata. Based on the post’s source, the content of the payload may change.  

Social Activity in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] has an **Additional Parameters** field that receives the social payload as JSON from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

To learn more about how to set up channel properties in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] to work with Additional Parameters from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], see [CRM Help & Training: Set up rules to automatically create or update records in CRM](https://go.microsoft.com/fwlink/p/?LinkID=624394).  

The JSON payload of this feature is described in the following table.  


|         Property          |  ActivityAdditionalParams   |                                                                                                                                                                                             Description                                                                                                                                                                                             |                                                   Source restrictions                                                   |
|---------------------------|-----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
|     `postmessagetype`     |             N/A             |                                                                                                                                                                 Type of post <br /><br />0: Public post<br /><br /> 1: Private post                                                                                                                                                                 |                                                           N/A                                                           |
|        `community`        |             N/A             |                                                                                                             Type of community <br /><br />1: [!INCLUDE[tn_facebook](../includes/tn-facebook.md)]<br /><br /> 2: [!INCLUDE[tn_twitter](../includes/tn-twitter.md)]<br /><br /> 0: Other                                                                                                              |                                                           N/A                                                           |
|     `sentimentvalue`      |             N/A             |                                                                                                                  Sentiment value of the post<br /><br />1: positive sentiment<br /><br />0: neutral sentiment<br /><br />-1: negative sentiment<br /><br />null: unknown sentiment                                                                                                                  |                                                           N/A                                                           |
|         `posturl`         |             N/A             |                                                                                                                                                                                         The URL of the post                                                                                                                                                                                         |                                                           N/A                                                           |
|       `description`       |             N/A             |                                                                                                                                                            Content of the post<br /><br />Up to 2000 characters of the written content.                                                                                                                                                             |                                                           N/A                                                           |
|         `subject`         |             N/A             |                                                                                                                                                       Post title if available. Otherwise, it's the first 200 characters of the post content.                                                                                                                                                        |                                                           N/A                                                           |
|        `postedon`         |             N/A             |                                                                                                                                                                           Date when the post was published by the author                                                                                                                                                                            |                                                           N/A                                                           |
| `activityaddtionalparams` |                             |                                                                                                                                                                             Additional parameters of the social activity                                                                                                                                                                             |                                                           N/A                                                           |
|            N/A            |     `targetEntityName`      |                                                                                  Name of the entity that gets created in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)].  When linking a post to [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)], this is always set to `socialactivity`.                                                                                  |                                                           N/A                                                           |
|            N/A            | `userPreferredTargetEntity` | Preferred entity as defined by the user in the Entity drop-down list  of a linked post's Record Details in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. This doesn’t necessarily match the type of record created in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] due to rules defined in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)]. |                                                           N/A                                                           |
|            N/A            |       `socialHandle`        |                                                                                                                                                                           Alias or user name of the author on the source.                                                                                                                                                                           |                                                           N/A                                                           |
|            N/A            |        `profileName`        |                                                                                                                                                                           Alias or user name of the author on the source.                                                                                                                                                                           |                                                           N/A                                                           |
|            N/A            |        `profilelink`        |                                                                                                                                                                                    URL to the author’s profile.                                                                                                                                                                                     | Available for [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] and [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] |
|            N/A            |         `fullName`          |                                                                                                                                                                                         The author’s name.                                                                                                                                                                                          |                                                           N/A                                                           |
|            N/A            |         `community`         |                                                                                                                            1: [!INCLUDE[tn_facebook](../includes/tn-facebook.md)]<br /><br /> 2: [!INCLUDE[tn_twitter](../includes/tn-twitter.md)]<br /><br /> 0: Other                                                                                                                             |                                                           N/A                                                           |
|            N/A            |      `influencescore`       |                                                                                                                                              Reach score of the author in a range from 0-99.  The higher the number, the more influential the author.                                                                                                                                               |                                                           N/A                                                           |
|            N/A            |  `retweetedBy_displayName`  |                                                                                                                                                                             Name of the author who retweeted the post.                                                                                                                                                                              |                                         Available only if the post is a retweet                                         |
|            N/A            |  `retweetedBy_externalId`   |                                                                                                                                                                          External ID of the author who retweeted the post.                                                                                                                                                                          |                                         Available only if the post is a retweet                                         |
|            N/A            |  `retweetedBy_screenName`   |                                                                                                                                                                             Name of the author who retweeted the post.                                                                                                                                                                              |                                         Available only if the post is a retweet                                         |
|            N/A            |         `isretweet`         |                                                                                                                                             Determines whether the post is a retweet or not.<br /><br /> true: retweet<br /><br /> false: not a retweet                                                                                                                                             |                                         Available only if the post is a retweet                                         |
|            N/A            |      `MSEbacklinkPost`      |                                                                                                                                                URI to access the post in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].                                                                                                                                                 |                                                           N/A                                                           |
|            N/A            |           `Notes`           |                                                                                                                 Additional information added by the creator of the social activity as free form text in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].                                                                                                                  |                                                           N/A                                                           |

## Sample payload

A typical JSON payload sent to [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] is given here.  

```json  
{
  "postmessagetype": 0,
  "community": 2,
  "sentimentvalue": 1,
  "posturl": "https://www.twitter.com/contoso/stauts/123412341234",
  "description": "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididu...", 
  "subject": "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididu...",
  "postedon": "2016-12-30T08:15:30-05:00",
  "activityadditionalparams": 
  {  
    "targetEntityName": "socialactivity",  
    "userPreferredTargetEntity": "incident",  
    "socialHandle": "Contoso",  
    "profileName": "Contoso",  
    "profilelink": "http://www.twitter.com/Contoso",  
    "fullName": "Contoso",  
    "community": 2,  
    "influencescore": 41.0,  
    "notes": "The customer requested a technician to call back as quickly as possible.",  
    "isRetweet": false,  
    "MSEbacklinkPost": "https://mi.ai.dynamics.com/app/23534544/#postid=45663"  
  }
}  
```  

## View record details for a linked post in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]

If a post is linked to a social activity in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)], you can open its associated record in **Dynamics 365 Record Details**.  

> [!NOTE]
> Only the custom entities in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] which are in relationship with the Social Activity entity are visible in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. For more information, see [TechNet: Create and edit entity relationships](https://technet.microsoft.com/library/dn531171.aspx).

### Open a Dynamics 365 record from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]

1. In [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], click **Posts** on the right side of any Analytics page to see the posts list.  

    --OR--  

    Go to **[!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]** > **Social Center** to see your streams.  

2. Select the post, and then click **Link to Dynamics 365** ![link to dynamics 365 button in market insights](media/link-to-record-icon.png "Link to Dynamics 365 button in Market Insights"). The **Dynamics 365 Record Details** dialog box shows all details for the associated Dynamics 365 record.  

   ![dynamics 365 record details](media/view-dynamics-365-record-details.png "Dynamics 365 record details")  

## Open a linked record in Dynamics 365

1. In [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], click **Posts** on any Analytics page to see the posts list.  

    --OR--  

    Go to **[!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]** > **Social Center** to see your streams.  

2. Select the post you want to open the associated record for, and then click **Link to Dynamics 365** ![link to dynamics 365 button in market insights](media/link-to-record-icon.png "Link to Dynamics 365 button in Market Insights").  

3. In the **Dynamics 365 Record Details**, click **Open Record** ![open record](media/open-record-icon.png "Open record") to see the record in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)].  

   [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] entities that are enabled for interactive experience open in the interactive service hub when you open a record on a social post that is linked to [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)]. [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] entities not enabled for interactive experience will continue open in the web client. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [CRM Help & Training: User's guide for the new interactive service hub](https://go.microsoft.com/fwlink/p/?LinkID=690167)  

   ![open record in dynamics 365 from market insights](media/open-record-details-in-dynamics-365.png "Open record in Dynamics 365 from Market Insights")  

> [!NOTE]
>  If there are no rules, or no active rules, or the social activity doesn't meet the defined conditions, no target [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record is created and the **Open Record** option  opens the social activity in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)]. When the target [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record is created, the **Open Record** option  opens the target record.

## Remove a linked Dynamics 365 record from a post

You can remove a linked [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record from a post. Note that removing a linked [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record from a post also removes any attached notes. Consider removing a linked [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record from a post when the link is no longer valid, is incorrect, or when you are considering creating a new entity record from the same post.  

> [!NOTE]
>  Removing a link does not affect the linked record in [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)], but only breaks the link between the [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] post and [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record. Once removed there is no way to re-establish the link between the same [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] post and same [!INCLUDE[pn_crm_shortest](../includes/pn-crm-shortest.md)] record.  

1. In [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)], click **Posts** on the right side of any Analytics page to see the posts list.  

    --OR--  

    Go to **[!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]** > **Social Center** to see your streams.  

2. Select the post you want to open the associated record for, and then click **Link to Dynamics 365** ![link to dynamics 365 button in market insights](media/link-to-record-icon.png "Link to Dynamics 365 button in Market Insights").  

3. In the **Dynamics 365 Record Details**, click **Remove**.  

![remove link between social post and dynamics 365](media/remove-link-to-dynamics-365-record.png "Remove link between social post and Dynamics 365")  

## Privacy Notice

 [!INCLUDE[cc_privacy_mse_post_and_automation_rules](../includes/cc-privacy-market-insights-post-and-automation-rules.md)] 

### See Also

 [Set up the connection between Dynamics 365 and Market Insights](connect-dynamics-365-record-creation.md)   
 [Link posts from Market Insights to Dynamics 365](link-posts-to-dynamics-365.md)   
 [Administer Market Insights](settings-administration.md)
