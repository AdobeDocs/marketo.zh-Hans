---
unique-page-id: 2359467
description: 电子邮件性能报告 - Marketo 文档 - 产品文档
title: 电子邮件性能报告
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '489'
ht-degree: 100%

---

# 电子邮件性能报告 {#email-performance-report}

要查看电子邮件的投递、打开、点击等性能量度，请创建一份电子邮件性能报告。

1. 请按照[在项目中创建报告](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md)的步骤操作，并选择&#x200B;**[!UICONTROL Email Performance]** [报告类型](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md)。
1. [更改报告时间范围](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md)，然后点击 **[!UICONTROL Report]** 选项卡。
1. 完成了！现在您可以查看报告，了解电子邮件的发送效果。

   >[!NOTE]
   >
   >“发送日期”筛选条件基于电子邮件首次发送的日期。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >点击电子邮件名称，即可在电子邮件预览器中打开。

   >[!NOTE]
   >
   >电子邮件性能报告包含所有人员的活动记录，包括在电子邮件发送后已删除的人员。有时您可能只希望查看活跃人员的活动。在这种情况下，需要在报告中过滤掉已删除的人员。请使用 **[!UICONTROL Smart List]** 选项卡，为报告[创建一个智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)。如果未基于任何特定字段进行筛选，请将“电子邮件地址”筛选条件设置为 **[!UICONTROL is not empty]**。

   电子邮件性能报告的[选择报告列](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md)包括：

   <table><thead>

<tr>
    <th>列</th>
    <th>描述</th>
  </tr></thead>
<tbody>
  <tr>
    <td>硬退信</td>
    <td>由于永久性原因（例如电子邮件地址不存在），电子邮件遭到拒收。</td>
  </tr>
  <tr>
    <td>软退信</td>
    <td>由于临时性原因（例如服务器不可用或收件箱已满），拒收电子邮件。</td>
  </tr>
  <tr>
    <td>待处理</td>
    <td>该数值通过从发送总数中减去已投递、硬退信和软退信的电子邮件数量计算得出。</td>
  </tr>
  <tr>
    <td>点击链接</td>
    <td>点击电子邮件中任意链接的收件人数量。</td>
  </tr>
  <tr>
    <td>取消订阅</td>
    <td>点击电子邮件中的取消订阅链接并填写表单的收件人数量。</td>
  </tr>
  <tr>
    <td>已中止</td>
    <td>未能成功投递且未收到退信事件的电子邮件数量。如果电子邮件发送后三天内未收到任何响应，该电子邮件将会自动标记为“中止”。</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>在报告中，点击取消订阅链接或电子邮件地址的行为不会计入“点击链接”。

通常情况下，我们会以符合直觉的方式来记录这些统计数据。例如，如果某人点击了电子邮件中的链接，则必然已先打开该电子邮件。电子邮件性能报告遵循以下具体规则：

* **规则 1**：每条电子邮件活动记录只会被标记为以下状态之一：_已投递_、_硬退信_、_软退信_&#x200B;或&#x200B;_待处理_。

* **规则 2**：如果电子邮件记录显示为 _[!UICONTROL Opened]_，则计为_&#x200B;已投递&#x200B;_。

* **规则 3**：如果电子邮件记录显示为 _[!UICONTROL Clicked Email]_或_[!UICONTROL Unsubscribed]_，则同时计为&#x200B;_已投递_&#x200B;和&#x200B;_已打开_。

* **规则 4**：如果电子邮件状态为 _[!UICONTROL Opened]_，则忽略退信。如果电子邮件尚未打开，则_&#x200B;硬退信&#x200B;_的优先级高于_&#x200B;软退信&#x200B;_和_&#x200B;已投递&#x200B;_。

* **规则 5**：如果电子邮件发送后三天内未收到任何活动记录，则视为&#x200B;_中止_。

>[!NOTE]
>
>* 同一营销活动向同一人员多次发送的电子邮件，仅计数一次。
>
>* 不同营销活动向同一人员发送的电子邮件，将分别计数。

>[!MORELIKETHIS]
>
>* [在营销活动电子邮件报告中过滤资源](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [在电子邮件性能报告中过滤已删除/已合并的记录](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [电子邮件链接性能报告](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
