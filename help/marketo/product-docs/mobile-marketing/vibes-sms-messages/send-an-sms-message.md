---
description: 发送短信消息 — Marketo文档 — 产品文档
title: 发送短信消息
feature: Mobile Marketing
exl-id: 2c863ded-f441-4217-9541-6dcc442d9831
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 发送短信消息 {#send-a-vibes-sms-message}

您已[创建短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}，现在可以发送该消息了。 您可以通过批量或触发营销活动来发送营销活动。

>[!NOTE]
>
>发送短信消息时：
>
>* 按电话号码Marketo Engage重复数据消除。 因此，如果多人拥有相同的电话号码，则只有一人会收到消息，前提是他们仅属于一个Vibes订阅列表。 重复数据消除是在Vibes Subscription列表级别，而不是Marketo项目级别完成的。
>* Marketo不会发送给被列入阻止列表或营销暂停的人员。
>* 如果任何未订阅的用户不在Vibes移动数据库列表中，则不会向其发送短信消息。

## 发送批量短信 {#send-a-batch-sms}

1. 在“我的Marketo”中，单击&#x200B;**营销活动**。

   ![](assets/send-an-sms-message-1.png)

1. 查找并选择所需的Smart Campaign。

   ![](assets/send-an-sms-message-2.png)

1. 单击&#x200B;**智能列表**&#x200B;选项卡并定义短信的受众。 在本例中，我们将向数据库中将“Adobe”列为其公司的每个人发送。

   ![](assets/send-an-sms-message-3.png)

1. 在&#x200B;**流**&#x200B;选项卡中，拖到&#x200B;**发送短信消息**&#x200B;上。 从下拉列表中选择所需的短信消息和访客列表。

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >“访客列表”选择器充当在智能列表中已标识的受众的附加过滤器，仅定向属于该访客列表的人员。

1. 单击&#x200B;**计划**&#x200B;选项卡并计划您的短信。

   ![](assets/send-an-sms-message-5.png)

## 发送触发短信 {#send-a-trigger-sms}

1. 在“我的Marketo”中，单击&#x200B;**营销活动**。

   ![](assets/send-an-sms-message-6.png)

1. 查找并选择所需的Smart Campaign。

   ![](assets/send-an-sms-message-7.png)

1. 单击&#x200B;**智能列表**&#x200B;选项卡，选择所需的触发器并定义其值。 在此示例中，我们使用&#x200B;**填写表单**。

   ![](assets/send-an-sms-message-8.png)

1. 在&#x200B;**流**&#x200B;选项卡中，拖到&#x200B;**发送短信消息**&#x200B;上。 从下拉列表中选择所需的短信消息和访客列表。

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >“访客列表”选择器充当在智能列表中已标识的受众的附加过滤器，仅定向属于该访客列表的人员。

1. 单击&#x200B;**计划**&#x200B;选项卡，然后单击&#x200B;**激活**。

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [创建Vibes消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}
>* [在智能营销活动中使用短信选项](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
