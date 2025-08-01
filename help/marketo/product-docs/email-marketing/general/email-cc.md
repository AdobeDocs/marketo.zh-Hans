---
unique-page-id: 17727995
description: 电子邮件抄送 — Marketo文档 — 产品文档
title: 电子邮件抄送
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 电子邮件抄送 {#email-cc}

电子邮件抄送允许通过Marketo发送的指定电子邮件包含抄送收件人。

此功能在所有Marketo电子邮件资源中均可用，无论电子邮件的发送方式（批量或触发营销活动）如何。 抄送收件人将收到发送给所选Marketo人员的电子邮件的精确副本。 因此，任何参与活动（打开、点击等）都将记录到电子邮件的“收件人”行中Marketo人员的活动日志中。 但是，“软退回”_以外的投放活动（已发送、已投放、硬退回等）将_&#x200B;不会&#x200B;**注册，因为Marketo无法区分Marketo人员的投放事件和抄送收件人。** Marketo一次最多只能抄送10万人。 如果您的智能列表超过100,000，并且其中的每个人都必须获得抄送，我们建议将您的列表分类。

>[!NOTE]
>
>电子邮件CC不能用于A/B测试。 如果您愿意，也可以使用，但是，由于技术上不支持，Marketo支持将无法协助进行任何故障排除。

## 设置电子邮件抄送 {#set-up-email-cc}

1. 在“我的Marketo”中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/one.png)

1. 在树中选择&#x200B;**[!UICONTROL Email]**。

   ![](assets/two.png)

1. 单击 **[!UICONTROL Edit Email CC Settings]**。

   ![](assets/three.png)

1. 选择最多25个Marketo潜在客户或公司字段（类型为“电子邮件”），以用作电子邮件中的抄送地址。 完成后单击&#x200B;**保存**。

   ![](assets/four.png)

## 使用电子邮件抄送 {#using-email-cc}

1. 选择您的电子邮件并单击&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/five.png)

1. 单击 **[!UICONTROL Email Settings]**。

   ![](assets/six.png)

1. 选择要用于抄送人员的字段。 _每封电子邮件不能超过5封_。 在本例中，我们只需要Lead Owner CC&#39;d。完成后单击&#x200B;**保存**。

   ![](assets/seven.png)

   就这么简单！ 在上例中，当您发送电子邮件时，所选收件人的Lead Owner将被抄送。

   >[!NOTE]
   >
   >如果“抄送”字段中包含无效的电子邮件地址，则将跳过该字段。

   为了快速识别，“电子邮件摘要”视图显示是否/选择了哪些电子邮件抄送字段。

   ![](assets/eight.png)

   如果电子邮件获得批准，但Marketo管理员在发送电子邮件之前禁用了一个或多个“抄送”字段，则&#x200B;**这些用户将不会收到电子邮件**。 在这种情况下，“电子邮件摘要”视图将清除所有在审批后但在发送前被禁用的字段：

   ![](assets/removal.png)

   >[!NOTE]
   >
   >您还会在电子邮件草稿的电子邮件设置部分中看到上述错误。

## 发送后 {#after-the-send}

* 如果抄送收件人单击电子邮件中的跟踪链接，则点击活动（与所有其他参与活动一样）将与电子邮件的主收件人关联。 此外，他们可以单击进入具有Marketo Web跟踪代码(munchkin.js)的页面，从而导致他们被作为主收件人进行编码。

>[!TIP]
>
>您可以选择[禁用电子邮件中的部分或全部跟踪链接](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md)。

* 执行电子邮件营销活动后，“发送电子邮件”活动将包括邮件每个收件人所包含的所有CC地址的列表。 如果由于取消订阅而跳过了任何CC地址，则活动中也会记录该地址。
* 取消订阅链接和页面在抄送电子邮件中正常工作。 这样，抄送收件人就可以根据需要成功取消订阅（遵守反垃圾邮件法规），并且此操作的记录将存储在Marketo数据库中。
* 在Marketo数据库中被列为已取消订阅的人将&#x200B;**不**&#x200B;通过CC接收电子邮件。
