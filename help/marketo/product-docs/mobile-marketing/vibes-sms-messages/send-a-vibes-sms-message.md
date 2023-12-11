---
description: 发送访客短信消息 — Marketo文档 — 产品文档
title: 发送访客短信消息
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: d4bd94b22b4f9da993150a94d2757014cbf87d80
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# 发送访客短信消息 {#send-a-vibes-sms-message}

您已 [已创建Vibes SMS消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)，现在该发送它了。 您可以通过批量或触发营销活动来发送营销活动。

>[!NOTE]
>
>发送短信消息时：
>
>* 按电话号码Marketo Engage重复数据消除。 因此，如果多人拥有相同的电话号码，则只有一人会收到消息，前提是他们仅属于一个Vibes订阅列表。 重复数据消除是在Vibes Subscription列表级别，而不是Marketo项目级别完成的。
>* Marketo不会发送给被列入阻止列表或营销暂停的人员。

## 发送批量短信 {#send-a-batch-sms}

1. 在“我的Marketo”中，单击 **营销活动**.

   ![](assets/send-a-vibes-sms-message-1.png)

1. 查找并选择所需的Smart Campaign。

   ![](assets/send-a-vibes-sms-message-2.png)

1. 单击 **智能列表** 制表符并定义短信的受众。 在本例中，我们将向数据库中将“Adobe”列为其公司的每个人发送。

   ![](assets/send-a-vibes-sms-message-3.png)

1. 在 **流量** 制表符，拖动到 **发送短信消息**. 从下拉列表中选择所需的短信消息和访客列表。

   ![](assets/send-a-vibes-sms-message-4.png)

   >[!NOTE]
   >
   >“访客列表”选择器充当在智能列表中已标识的受众的附加过滤器，仅定向属于该访客列表的人员。

1. 单击 **计划** 制表符并计划您的短信。

   ![](assets/send-a-vibes-sms-message-5.png)

## 发送触发短信 {#send-a-trigger-sms}

1. 在“我的Marketo”中，单击 **营销活动**.

   ![](assets/send-a-vibes-sms-message-6.png)

1. 查找并选择所需的Smart Campaign。

   ![](assets/send-a-vibes-sms-message-7.png)

1. 单击 **智能列表** 选项卡，选择所需的触发器并定义其值。 在本例中，我们使用 **填写表单**.

   ![](assets/send-a-vibes-sms-message-8.png)

1. 在 **流量** 制表符，拖动到 **发送短信消息**. 从下拉列表中选择所需的短信消息和访客列表。

   ![](assets/send-a-vibes-sms-message-9.png)

   >[!NOTE]
   >
   >“访客列表”选择器充当在智能列表中已标识的受众的附加过滤器，仅定向属于该访客列表的人员。

1. 单击 **计划** 选项卡，然后 **激活**.

   ![](assets/send-a-vibes-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [创建Vibes消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)
>* Vibes流步骤

