---
unique-page-id: 7515133
description: 了解Salesforce和Marketo中合并潜在客户、联系人和人员的工作方式。 了解分数、字段值和活动日志的合并规则。
title: SFDC同步 — 合并潜在客户/联系人/人员
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 25bbf4409df3db38b849d936e2a90b48f859d089
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 2%

---

# SFDC 同步：合并潜在客户/联系人/人员 {#sfdc-sync-merging-a-lead-contact-person}

有时最好只是列出规则。 接下来是：

* 当您在&#x200B;**[!DNL Salesforce]**&#x200B;中合并两个潜在客户时，普通同步会告知Marketo，并且这些潜在客户会自动作为Marketo中的人员合并。
* 在&#x200B;**Marketo**&#x200B;中合并两个人实际上会调用与在[!DNL Salesforce]中合并潜在客户相同的进程。 它仍然自动工作。
* 将&#x200B;**潜在客户（人员）合并到联系人**&#x200B;的工作方式相同。 最终两边只有一个接触点。
* 合并时，将汇总默认得分。

>[!NOTE]
>
>如果将3个各自得分为10分的潜在客户（人员）合并，则将得到1个潜在客户（人员）的结果，得分为30。

* 从“入选记录”中获取冲突的字段值。 （记录=产生的潜在客户或联系人）
* 如果“失败记录”（正在消失的记录）具有值，并且获胜记录没有（或为空），我们将保留失败记录。 换句话说，“有价值总比没有价值好。”
* 所有活动日志项都会被合并。

>[!NOTE]
>
>在2026年3月版中，API合并中的布尔字段行为发生了更改。 现在，False值会正确被视为具有该字段的值。 在评估冲突字段时，只有null值被视为“空”。 查看[此社区帖子](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219){target="_blank"}的更多详细信息。

>[!MORELIKETHIS]
>
>深入了解Marketo[&#128279;](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)中有关合并人员的详细信息。
