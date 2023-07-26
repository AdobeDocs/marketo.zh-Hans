---
unique-page-id: 2359467
description: 电子邮件性能报表 — Marketo文档 — 产品文档
title: 电子邮件性能报表
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# 电子邮件性能报表 {#email-performance-report}

要查看电子邮件使用已投放、已打开、已单击等统计信息时的性能，请创建电子邮件性能报表。

1. [在项目群中创建报告](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) 并选择 **电子邮件性能** [报告类型](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [更改报表时间范围](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) 然后单击 **报表** 选项卡。
1. 你在那儿！ 现在，浏览报表以查看电子邮件的执行情况。

   >[!NOTE]
   >
   >“发送日期”过滤器基于电子邮件的第一个发送日期。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >单击电子邮件的名称，以在电子邮件预览器中将其打开。

   >[!NOTE]
   >
   >电子邮件性能报表包含适用于所有人员的活动，包括自发送电子邮件以来已删除的活动。 有时候，您只想查看活跃人士的活动。 在这种情况下，您需要从报表中过滤删除的人员。 使用 **智能列表** 按Tab键至 [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 作为报告。 如果您未对任何特定字段进行筛选，请将电子邮件地址筛选器设置为： **不为空**.

   [选择报表列](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) 对于电子邮件性能报表，包括：

   | 列 | 描述 |
   |---|---|
   | 硬退回 | 由于永久条件（如不存在电子邮件地址），电子邮件被拒绝。 |
   | 软退回 | 由于临时情况（如服务器关闭或收件箱已满），电子邮件被拒绝。 |
   | 待处理 | 此数字可通过从发送的总数中减去已发送、已退回和已软退回的电子邮件数来计算。 |
   | 已单击的链接 | 单击电子邮件中链接的电子邮件收件人数量。 |
   | 退订 | 单击“ ”的电子邮件收件人数 **取消订阅** 电子邮件中的链接并填写表单。 |

   >[!NOTE]
   >
   >取消订阅电子邮件中单击的链接和电子邮件地址将不会在报表中的已单击链接下注册。

一般来说，我们尝试用常识来记录这些统计数据。 例如，如果某人单击了电子邮件中的链接，则他们显然会先打开该电子邮件。 我们遵循电子邮件性能报表的以下特定规则：

* **规则1**：每个电子邮件活动记录均设置为以下项之一，且仅设置一个： _已投放_， _硬退回_， _软退回_，或 _待处理_.

* **规则2**：如果电子邮件记录显示 *已打开*，则计为 *已投放*.

* **规则3**：如果电子邮件记录显示 _已点击电子邮件_ 或 _已取消订阅_，则计为 _已投放_ 和 _已打开_.

* **规则4**：如果电子邮件为 _已打开_，会忽略退回。 如果电子邮件尚未打开， _硬退回_ 优先于 _软退回_ 和 _已投放_.

>[!NOTE]
>
>从同一营销活动向同一人员发送的多次发送仅计数一次。

>[!MORELIKETHIS]
>
>* [在Campaign电子邮件报表中筛选资源](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [电子邮件链接性能报表](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)
