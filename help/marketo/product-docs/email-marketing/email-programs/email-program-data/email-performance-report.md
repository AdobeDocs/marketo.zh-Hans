---
unique-page-id: 2359467
description: 电子邮件性能报表 — Marketo文档 — 产品文档
title: 电子邮件性能报表
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# 电子邮件性能报表 {#email-performance-report}

要了解您的电子邮件使用已提交、打开、点击等统计资料的表现如何，请创建电子邮件效果报表。

1. [在项目中创建报表](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) ，然后选择 **电子邮件性能** [报表类型](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [更改报表时间范围](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) ，然后单击 **报表** 选项卡。
1. 你在那！ 现在浏览该报表，了解电子邮件的执行情况。

   >[!NOTE]
   >
   >“发送日期”过滤器基于电子邮件的首次发送日期。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >单击电子邮件的名称，以在电子邮件预览器中将其打开。

   >[!NOTE]
   >
   >电子邮件性能报表包含所有人员的活动，包括自电子邮件发送以来已删除的活动。 有时，您只想查看活跃人员的活动。 在这种情况下，您需要从报表中过滤已删除的人员。 使用 **智能列表** 选项卡 [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 中。 如果未对任何特定字段进行过滤，请将“电子邮件地址”过滤器设置为： **不为空**.

   [选择报表列](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) 对于“电子邮件性能”报表，其中包括：

   | 列 | 描述 |
   |---|---|
   | 硬退回 | 电子邮件因永久性条件（如不存在的电子邮件地址）而被拒绝。 |
   | 软退回 | 电子邮件因临时情况（如服务器关闭或收件箱已满）而被拒绝。 |
   | 待定 | 此数字的计算方式是从总发送数量中减去已送达、已退回和软退回的电子邮件数量。 |
   | 点击的链接 | 单击电子邮件中链接的电子邮件收件人数量。 |
   | 退订 | 点击了 **取消订阅** 链接并填写表单。 |

   >[!NOTE]
   >
   >取消订阅电子邮件中点击的链接和电子邮件地址不会在报表的已点击链接下注册。

一般来说，我们尝试用常识来记录这些统计数据。 例如，如果某人单击了电子邮件中的链接，则显然是先打开了电子邮件。 我们在电子邮件性能报表中遵循以下特定规则：

* **规则1**:每个电子邮件活动记录均设置为以下一项，且仅设置为一项： _已交付_, _硬退回_, _软退回_&#x200B;或 _待定_.

* **规则2**:如果电子邮件记录显示 *已打开*，则计为 *已交付*.

* **规则3**:如果电子邮件记录显示 _已点击电子邮件_ 或 _已取消订阅_，则计为 _已交付_ 和 _已打开_.

* **规则4**:如果电子邮件为 _已打开_，则会忽略跳出。 如果尚未打开电子邮件， _硬退回_ 优先于 _软退回_ 和 _已交付_.

>[!NOTE]
>
>从同一营销活动向同一人发送的多个消息只会被计数一次。

>[!MORELIKETHIS]
>
>* [在营销活动电子邮件报表中过滤资产](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [电子邮件链接性能报表](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

