---
unique-page-id: 2949716
description: 使用适用于Outlook的电子邮件加载项 — Marketo文档 — 产品文档，发送和跟踪电子邮件
title: 使用Outlook的电子邮件加载项发送和跟踪电子邮件
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 使用Outlook的电子邮件加载项发送和跟踪电子邮件 {#send-and-track-an-email-with-the-email-add-in-for-outlook}

您可以直接从Outlook通过Marketo发送和跟踪电子邮件。

>[!PREREQUISITES]
>
>如果尚未安装，请安装 [适用于Outlook的Marketo电子邮件加载项](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

1. 打开Microsoft Outlook并创建新电子邮件。

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >如果电子邮件中包含多个收件人，则会在第一个收件人下跟踪所有活动。

1. 按常规方式撰写电子邮件，然后单击 **发送和跟踪**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >如果您向Marketo实例中不存在的人员发送电子邮件，则将自动为他们创建人员记录。 他们的姓氏将始终为“mktUnknown”，以便您轻松找到他们。

   >[!TIP]
   >
   >如果要使用Marketo模板，请参阅 [使用模板从Outlook发送和跟踪](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. 查看预览并单击 **发送**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >反垃圾邮件技术通常拒绝在发送电子邮件后20秒内打开和发生的点击，因此，请至少等待那么长时间，以在测试时打开/单击。

   为了查看谁收到了您通过Outlook发送的电子邮件，请使用“已发送销售电子邮件”过滤器创建智能列表。

   ![](assets/was-sent-sales-email.png)

这太简单了！ 即使此电子邮件是由销售人员的Outlook发送的，仍会在Marketo中对其进行跟踪。

>[!MORELIKETHIS]
>
>[在Marketo中记录来自您潜在客户的入站邮件](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
