---
unique-page-id: 2949716
description: 使用Outlook的Email Add-In发送和跟踪电子邮件 — Marketo文档 — 产品文档
title: 使用Outlook的Email Add-In发送和跟踪电子邮件
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
source-git-commit: 8b9b2b83f5dc8908f9794d1ee387299edaae31b3
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 使用Outlook的Email Add-In发送和跟踪电子邮件 {#send-and-track-an-email-with-the-email-add-in-for-outlook}

您可以使用Marketo直接从Outlook发送和跟踪电子邮件。

>[!PREREQUISITES]
>
>如果尚未安装，请安装 [适用于Outlook的Marketo电子邮件加载项](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

>[!NOTE]
>
>Sales Insight Actions功能（包括“发送销售电子邮件”、“添加到Sales Campaign”和“任务”）在Gmail和Outlook的Sales Insight电子邮件插件中不可用。 目前，在使用Sales Insight电子邮件插件时，用户只能从其电子邮件客户端发送可跟踪电子邮件，无论是否包含Marketo电子邮件模板。

1. 打开Microsoft Outlook并创建新电子邮件。

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >如果电子邮件中包含多个收件人，则所有活动都将被跟踪到第一个收件人下。

1. 按常规方式撰写电子邮件，然后单击 **Send and Track**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >如果您将电子邮件发送给不在Marketo实例中的人员，则将自动为其创建人员记录。 他们的姓氏将始终为“mktUnknown”，以便您可以轻松找到他们。

   >[!TIP]
   >
   >如果要使用Marketo模板，请参阅 [使用模板从Outlook发送和跟踪](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. 查看预览并单击 **发送**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >反垃圾邮件技术通常会拒绝在发送电子邮件后20秒内发生的打开和点击，因此请在测试时至少等待这么长时间以打开/点击。

   要查看谁收到了通过Outlook发送的电子邮件，请使用“已发送销售电子邮件”过滤器创建一个智能列表。

   ![](assets/was-sent-sales-email.png)

就这么简单！ 即使此电子邮件是由销售人员的Outlook发送的，但将在Marketo中对其进行跟踪。

>[!MORELIKETHIS]
>
>[在Marketo中记录潜在客户的入站邮件](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
