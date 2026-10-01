---
unique-page-id: 2360188
description: 了解按智能营销活动对电子邮件统计信息分组的Campaign电子邮件性能报表。 跟踪打开、点击、退回和取消订阅以衡量促销活动有效性。
title: 营销活动电子邮件性能报告
exl-id: 524222c6-7cf6-4e6d-a1a5-20a771cd9da5
feature: Reporting
TQID: https://experienceleague.adobe.com/pMoHSEmaDbjOVpoVaUi1lvUHBYkyzOwkuF1n7mxpmY0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
source-git-commit: fd61a23992a0698425987c9c1c307c148c51041e
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 26%
---
# 营销活动电子邮件性能报告 {#campaign-email-performance-report}

要查看按[Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/understanding-batch-and-trigger-smart-campaigns.md)分组的电子邮件性能统计信息，请运行营销活动电子邮件性能报告。

>[!NOTE]
>
>营销活动电子邮件效果报表只能在营销活动程序中创建为本地资产。 在Analytics部分中不可用。

1. 在程序中，单击&#x200B;**新建**&#x200B;并选择&#x200B;**新建本地资产**。

   ![](assets/campaign-email-performance-report-1.png)

1. 选择&#x200B;**报告**。

   ![](assets/campaign-email-performance-report-2.png)

1. 在&#x200B;_类型_&#x200B;下拉列表中，选择&#x200B;**促销活动电子邮件性能**。 为您的报告提供一个名称，然后单击&#x200B;**创建**。

   ![](assets/campaign-email-performance-report-3.png)

1. 定义报表的参数。

   ![](assets/campaign-email-performance-report-4.png)

1. 完成后，单击&#x200B;**报告**&#x200B;选项卡以查看报告。

您可以为营销活动电子邮件性能报告选择[列](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md)，这些列包括：

| 列 | 描述 |
|---|---|
| [!UICONTROL Hard Bounced] | 由于永久性原因（例如电子邮件地址不存在），电子邮件遭到拒收。 |
| [!UICONTROL Soft Bounced] | 由于临时性原因（例如服务器不可用或收件箱已满），拒收电子邮件。 |
| [!UICONTROL Pending] | 电子邮件仍在投放过程中。 |
| [!UICONTROL Clicked Link] | 点击电子邮件中任意链接的收件人数量。 |
| [!UICONTROL Unsubscribed] | 单击电子邮件中的&#x200B;**[!UICONTROL Unsubscribe]**&#x200B;链接并填写表单的电子邮件收件人数。 |

>[!NOTE]
>
>通常情况下，我们会以符合直觉的方式来记录这些统计数据。 例如，如果某人单击了电子邮件中的链接，则他们显然会先打开该链接。 有关我们遵循的特定规则，请参阅[电子邮件性能报表](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md)。

>[!MORELIKETHIS]
>
>* [在营销活动电子邮件报告中筛选Assets](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [电子邮件性能报告](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md)
