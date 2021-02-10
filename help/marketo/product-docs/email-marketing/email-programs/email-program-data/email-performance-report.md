---
unique-page-id: 2359467
description: 电子邮件性能报告- Marketo Docs —— 产品文档
title: 电子邮件性能报告
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---


# 电子邮件性能报告{#email-performance-report}

要了解您的电子邮件对已发送、打开、点击等统计信息的效果，请创建电子邮件性能报告。

1. [在程序中创建报](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) 告，然后选择 **电子邮件** [性能报告类型](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md)。
1. [更改报告时间](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) 框架，然后单击报 **** 告选项卡。
1. 你在那！ 现在浏览报告，了解电子邮件的执行方式。

   >[!NOTE]
   >
   >“发送日期”过滤器基于电子邮件的第一个发送日期。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >单击电子邮件的名称以在电子邮件预览器中将其打开。

   >[!NOTE]
   >
   >电子邮件绩效报告包含所有人员的活动，包括自电子邮件发送后已删除的人员。 有时，您只希望看到活跃人员的活动。 在这种情况下，您需要从报表中筛选已删除的人员。 使用&#x200B;**智能列表**&#x200B;选项卡[为报告创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)。 如果您未对任何特定字段进行过滤，请将“电子邮件地址”过滤器设置为：**不为空**。

   [为电子邮件](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) 性能报告选择报告列包括：

   | 列 | 说明 |
   |---|---|
   | 硬退回 | 电子邮件被拒绝，因为存在永久条件，如不存在的电子邮件地址。 |
   | 软退回 | 由于临时情况（如服务器关闭或收件箱已满），电子邮件被拒绝。 |
   | 待定 | 此数字通过从“已发送”总数中减去“已传送”、“退回”和“软退回”电子邮件数来计算。 |
   | 已点击链接 | 单击电子邮件中链接的电子邮件收件人数。 |
   | 取消订阅 | 单击电子邮件中的&#x200B;**取消订阅**&#x200B;链接并填写表单的电子邮件收件人数。 |

   >[!NOTE]
   >
   >取消订阅电子邮件中被点击的链接和电子邮件地址将不会在报告的“已点击链接”下注册。

一般来说，我们试图用常识来记录这些统计数据。 例如，如果某人单击了电子邮件中的链接，则显然他们首先打开了电子邮件。 我们遵循电子邮件性能报告的以下特定规则：

* **规则1**:每个电子邮件活动记录均设置为以下一项，且仅设置为一项： _已交付_ _、_&#x200B;硬退回 _、_&#x200B;软退回 _或_&#x200B;待定。

* **规则2**:如果电子邮件记录显 *示已*&#x200B;打开，则计为已 *送达*。

* **规则3**:如果电子邮件记录显 _示“_ 已点击 _电子邮_&#x200B;件”或“未订 __ 阅 _”，则计为“已_&#x200B;交付和已打开”。

* **规则4**:如果电子邮件已打 _开_，则会忽略弹回。如果电子邮件尚未打开，则&#x200B;_硬退回_&#x200B;优先于&#x200B;_软退回_&#x200B;和&#x200B;_已送达_。

>[!NOTE]
>
>从同一活动向同一人发送的多个消息只计数一次。

>[!MORELIKETHIS]
>
>* [筛选活动电子邮件报告中的资产](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [电子邮件链接性能报告](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

