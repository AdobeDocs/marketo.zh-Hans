---
unique-page-id: 8159286
description: 机会过滤器和触发器- Marketo Docs —— 产品文档
title: 机会过滤器和触发器
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# 机会过滤器和触发器{#opportunity-filters-and-triggers}

业务机会过滤器和触发器允许您从Salesforce跟踪业务机会事件。 与其他过滤器和触发器相比，它们有些不同。

## 机会过滤器{#opportunity-filters}

业务机会过滤器允许您深入了解拥有业务机会的Salesforce潜在客户。 编辑智能列表时，您可以在Palette的Opportunity文件夹中找到它们。 它们有几种味道。

* Optys数
* 产品总数
* 预计总业务收入
* 有机会
* 已添加机会
* 已删除机会
* 已更新业务机会

如果要查找Opportunity字段（自定义或标准），请使用&#x200B;**Has Opportunity**&#x200B;过滤器或&#x200B;**Opportunity是`[Added/Removed/Updated]`**&#x200B;过滤器或触发器。

**Optys数量、 Opty Amount 、 Opty Preset Revenue**

通过这些过滤器，您可以根据潜在客户的所有机会的总数、金额或预期收入来查找潜在客户。

![](assets/image2015-6-11-12-3a29-3a34.png)

**Has Opportunity（已添加到Opportunity）已从Opportunity中删除**

如果您正在寻找基于条件组合而拥有机会的潜在客户，请使用&#x200B;**Has Opportunity**、**Was Added to Opportunity**&#x200B;或&#x200B;**Was Removed from Opportunity**&#x200B;过滤器。 他们告诉你：

* **有机会**:如果此潜在客户当前具有任何匹配的机会
* **已添加到Opportunity**:如果此潜在客户曾被添加到匹配的机会中
* **已从Opportunity中删除**:如果此潜在客户从匹配的机会中删除

在筛选器上将搜索条件添加为&#x200B;**Constraints**。 约束包括您的机会标准和自定义字段：

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

例如，假设您要查找具有至少5,000美元的潜在客户。 在&#x200B;**Has Opportunity**&#x200B;过滤器中拖动并使用&#x200B;**Is Closed**&#x200B;和&#x200B;**Amount**&#x200B;约束：

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>当您使用多个Opportunity过滤器时，您可能会得到错误的答案。 如果您使用两个Opportunity过滤器构建上述示例，您将得到一列表潜在客户，他们拥有至少5,000美元的机会和任何已关闭的机会，即使这些机会是单独的机会。

**已更新业务机会**

**Opportunity was Updated**&#x200B;过滤器在更新特定机会字段时查找任何机会。 选取要检查的“触发器属性”(Trigger Attribute)下拉框，然后使用约束来缩小更改集。

例如，此过滤器将向您显示过去30天内完成结束日期更改的所有潜在客户：

![](assets/image2015-6-11-12-3a33-3a7.png)

## Opportunity Triggers {#opportunity-triggers}

可以使用以下机会触发器。 它们的工作方式与其相应过滤器（如前所述）相同，只是当事件发生时，它们可以直接触发活动:

* 已更新业务机会
* 添加到Opportunity
* 从Opportunity中删除

例如，您可以使用此智能列表在将任何潜在客户添加到任何业务机会时触发。 在流程中，您可以将其添加到“营销暂停”列表或向其发送目标电子邮件。

![](assets/image2015-6-11-12-3a33-3a48.png)

要触发业务机会自定义字段，请使用&#x200B;**Opportunity is Updated**&#x200B;触发器，并在下拉列表中选择字段：

![](assets/image2015-6-11-12-3a33-3a34.png)

