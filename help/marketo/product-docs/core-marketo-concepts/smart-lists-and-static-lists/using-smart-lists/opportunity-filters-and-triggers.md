---
unique-page-id: 8159286
description: Opportunity Filters and Triggers - Marketo文档 — 产品文档
title: 机会过滤器和触发器
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# 机会过滤器和触发器 {#opportunity-filters-and-triggers}

机会过滤器和触发器允许您跟踪来自[!DNL Salesforce]的机会事件。 它们与其他过滤器和触发器有些不同。

## 机会过滤器 {#opportunity-filters}

机会筛选器允许您深入查看具有机会的Salesforce潜在客户。 编辑智能列表时，可以在“组件面板”的“业务机会”文件夹中找到它们。 它们有几种味道。

* 选件数
* 总商机金额
* 预计总商机收入
* 具有机会
* 机会已添加
* 机会已删除
* 机会已更新

如果您正在查找Opportunity字段（自定义或标准），请使用&#x200B;**Has Opportunity**&#x200B;筛选器或&#x200B;**Opportunity是`[Added/Removed/Updated]`**&#x200B;个筛选器或触发器。

**商机数，总商机金额，总商机预期收入**

通过这些过滤器，您可以根据销售机会的总数、金额或预期收入来查找销售线索。

![](assets/opportunity-filters-and-triggers-1.png)

**Has Opportunity Added To Opportunity Was Removed From Opportunity**

如果您要查找根据条件组合而拥有机会的潜在客户，请使用&#x200B;**Has Opportunity**、**Was Added To Opportunity**&#x200B;或&#x200B;**Was Removed from Opportunity**&#x200B;筛选器。 他们会告诉你：

* **具有机会**：如果此潜在客户当前具有任何匹配的机会
* **已添加到Opportunity**：如果此潜在客户已添加到匹配机会
* **已从商机中删除**：如果此商机已从匹配商机中删除

将搜索条件添加为筛选器上的&#x200B;**约束**。 这些限制包括您的机会标准字段和自定义字段：

![](assets/opportunity-filters-and-triggers-2.png)

![](assets/opportunity-filters-and-triggers-3.png)

例如，假设您要查找具有至少$5,000的未完成销售机会的潜在客户。 拖入&#x200B;**Has Opportunity**&#x200B;筛选器并使用&#x200B;**Is Closed**&#x200B;和&#x200B;**Amount**&#x200B;约束：

![](assets/opportunity-filters-and-triggers-4.png)

>[!NOTE]
>
>当您使用多个Opportunity筛选器时，您可能会得到不正确的答案。 如果您使用两个Opportunity筛选器构建了以上示例，您会得到一个销售线索列表，这些销售线索中至少有5,000美元的销售机会，并且有已结束的销售机会，即使这些是单独的业务机会。

**机会已更新**

**Opportunity已更新**&#x200B;筛选器在更新特定的opportunity字段时查找任何opportunity。 选取要与“触发器属性”下拉菜单一起检查的字段，然后使用约束来缩小更改集。

例如，此过滤器将显示其关闭日期在过去30天内发生更改的所有潜在客户：

![](assets/opportunity-filters-and-triggers-5.png)

## 机会触发器 {#opportunity-triggers}

以下机会触发器可供使用。 它们的作用与它们对应的过滤器（前面已介绍）相同，不同之处在于，它们可以在事件发生时触发营销活动：

* 机会已更新
* 已添加到机会
* 已从机会中移除

例如，您可以使用此智能列表在任意商机中添加任何商机时触发。 在流中，您可以将用户添加到“营销已挂起”列表，或向他们发送定向电子邮件。

![](assets/opportunity-filters-and-triggers-6.png)

要触发您的Opportunity自定义字段，请使用&#x200B;**Opportunity is Updated**&#x200B;触发器并选取下拉列表中的字段：

![](assets/opportunity-filters-and-triggers-7.png)
