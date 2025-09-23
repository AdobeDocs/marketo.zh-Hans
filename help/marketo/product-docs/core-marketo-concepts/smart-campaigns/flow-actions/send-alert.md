---
unique-page-id: 1146958
description: 发送警报 — Marketo文档 — 产品文档
title: 发送警报
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 2%

---

# 发送警报 {#send-alert}

Marketo Engage可以向任何人（销售负责人、合作伙伴或其他人）发送包含人员信息的电子邮件警报。 使用“[!UICONTROL Send Alert]”流程步骤。

![](assets/send-alert-1.png)

1. 查找并选择您要发送的电子邮件。

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >您的电子邮件警报必须包含所有标题信息并处于&#x200B;**[!UICONTROL Approved]**&#x200B;状态。

1. 您可以单击预览图标，以确保您选择了正确的电子邮件。

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >请确保在电子邮件中使用“[!UICONTROL Send Alert Info]”令牌。

1. 选择警报收件人。 您可以选择[!UICONTROL Sales Owner]或[!UICONTROL Account Owner]。

   ![](assets/send-alert-4.png)

1. （可选）添加您想要的任何其他电子邮件地址（用逗号或分号分隔）。

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >在触发营销活动中，您可以使用&#x200B;**[!UICONTROL To Other Emails]**&#x200B;中的令牌，如`{{lead.Territory Owner}}`或`{{my.Alert Recipient}}`，只要这些值是有效的电子邮件地址即可。 **[!UICONTROL To Other Emails]**&#x200B;中的令牌在批处理营销活动中不起作用。

>[!MORELIKETHIS]
>
>[创建电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
