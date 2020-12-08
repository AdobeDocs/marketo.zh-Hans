---
unique-page-id: 11379045
description: 添加SMS - Marketo Docs —— 产品文档的流程步骤
title: 为SMS添加流程步骤
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 为SMS添加流程步骤 {#add-a-flow-step-for-sms}

Marketo有三个流程步骤，您可以在SMS智能活动中使用：

* **发送SMS消息** -此流操作向订阅用户选择的Vibes订阅列表的Marketto智能列表用户发送消息。 它不启动订阅过程。
* **订阅Vibes列表** -此流操作通过用户选择的Vibes客户获取活动启动SMS订阅流程。 然后，Vibes发送确认消息；收件人必须回复它才能完成订阅过程。
* **取消订阅Vibes列表** -此流操作取消每个人对用户选择的Vibes订阅列表的订阅。

>[!NOTE]
>
>发送SMS消息时：
>
>* Marketo通过电话号码消除重复。 因此，如果多个人具有相同的电话号码，则只有一个人会收到该消息。
>* Marketo不会发送给被或市场列入阻止列表暂停的人员。

>



有关设置流步骤的一般信息，请 [参阅将流步骤添加到智能活动](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)。

下面是使用SMS的基础知识。

1. 在“我的营销人员”中，单 **击营销活动**。

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. 查找要添加SMS流的智能活动。 单击“流 **”** (Flow)选项卡。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. 拖动到流上，例如， **发送SMS消息**。 从下拉菜单中选择SMS消息和Vibes列表。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Vibes列表选择器充当对智能列表中已识别的受众的进一步过滤器，以仅目标属于该Vibes列表的那些潜在客户。
   >
   >
   >“订 **阅Vibes列表** ”和“ **取消订阅Vibes列表流** ”有不同的要求。 对于 **订阅**，您必须选择Vibes列表和Vibes客户获取活动。 对于 **取消订**&#x200B;阅，只需使用Vibes列表。

