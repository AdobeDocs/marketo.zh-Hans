---
unique-page-id: 2359467
description: 电子邮件性能报告- Marketo Docs —— 产品文档
title: 电子邮件性能报告
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# 电子邮件性能报告 {#email-performance-report}

要了解您的电子邮件对已发送、打开、点击等统计信息的效果，请创建电子邮件性能报告。

1. [在项目中创建报告](../../../../product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) ，然后选择 **电子邮件**[性能报告类型](../../../../product-docs/reporting/basic-reporting/report-types/report-type-overview.md)。
1. [更改报告时间范围](../../../../product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) ，然后单 **击报** 告选项卡。
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
   >
   >电子邮件绩效报告包含所有人员的活动，包括自电子邮件发送后已删除的人员。 有时，您只希望看到活跃人员的活动。 在这种情况下，您需要从报表中筛选已删除的人员。 使用 **智能列表** 选项 [卡为报表](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 创建智能列表。 如果您未对任何特定字段进行过滤，请将“电子邮件地址”过滤器设置为： **不是空的**。

   [为“电子邮件](../../../../product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) ”性能报告选择报告列包括：

   | 列 | 说明 |
   |---|---|
   | 硬退回 | 电子邮件被拒绝，因为存在永久条件，如不存在的电子邮件地址。 |
   | 软退回 | 由于临时情况（如服务器关闭或收件箱已满），电子邮件被拒绝。 |
   | 待定 | 此数字通过从“已发送”总数中减去“已传送”、“退回”和“软退回”电子邮件数来计算。 |
   | 已点击链接 | 单击电子邮件中链接的电子邮件收件人数。 |
   | 取消订阅 | 单击电子邮件中的“取消订 **阅** ”链接并填写表单的电子邮件收件人数。 |

   >[!NOTE]
   >
   >取消订阅电子邮件中被点击的链接和电子邮件地址将不会在报告的“已点击链接”下注册。

一般来说，我们试图用常识来记录这些统计数据。 例如，如果某人单击了电子邮件中的链接，则显然他们首先打开了电子邮件。 我们遵循电子邮件性能报告的以下特定规则：

* **规则1**:每个电子邮件活动记录均设置为以下一项，且仅设置为一项： *已交付**、*&#x200B;硬退回 *、*&#x200B;软退回 *或*&#x200B;待定。

* **规则2**:如果电子邮件记录显 *示已*&#x200B;打开，则计为已 *送达*。

* **规则3**:如果电子邮件记录显 *示“已点击* ”或“ *未订阅*”，则计为“已 *送达* ”和“已 **&#x200B;打开”。

* **规则4**:如果电子邮件已打 *开*，则会忽略弹回。 如果电子邮件尚未打开，则“硬 *退回* ”优先于“软退 *回”和“已* 送达” **。

>[!NOTE]
>
>从同一活动向同一人发送的多个消息只计数一次。

>[!NOTE]
>
>**相关文章**
>
>* [筛选活动电子邮件报告中的资产](../../../../product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [电子邮件链接性能报告](email-link-performance-report.md)

>



>[!NOTE]
>
>**深潜**
>
>在基本报告 [中了解更多](http://docs.marketo.com/display/docs/basic+reporting)。

