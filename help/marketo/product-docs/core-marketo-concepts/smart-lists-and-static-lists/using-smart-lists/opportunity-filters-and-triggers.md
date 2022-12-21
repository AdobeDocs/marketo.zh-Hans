---
unique-page-id: 8159286
description: Opportunity Filter和触发器 — Marketo文档 — 产品文档
title: Opportunity Filters和Triggers
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Opportunity Filters和Triggers {#opportunity-filters-and-triggers}

Opportunity过滤器和触发器允许您从Salesforce中跟踪商机事件。 与其他过滤器和触发器相比，它们有些不同。

## 机会过滤器 {#opportunity-filters}

Opportunity Filter允许您深入了解有机会的Salesforce潜在客户。 编辑智能列表时，您可以在Paltete的Opportunities文件夹中找到它们。 它们有几种味道。

* 选项数
* 产品总额
* 预计总运营收入
* 有机会
* 已添加机会
* 机会已删除
* 机会已更新

如果您正在查找Opportunity字段（自定义或标准），请使用 **有机会** 过滤器或 **机会是`[Added/Removed/Updated]`** 过滤器或触发器。

**产品数量、产品总额、预计产品总收入**

通过这些过滤器，您可以根据所有商机的总数、金额或预期收入来查找潜在客户。

![](assets/image2015-6-11-12-3a29-3a34.png)

**Has Opportunity（已添加到Opportunity）已从Opportunity中删除**

如果您要查找基于一系列标准而具有商机的潜在客户，请使用 **有机会**, **已添加到Opportunity**&#x200B;或 **已从Opportunity中删除** 过滤器。 他们告诉你：

* **有机会**:如果此潜在客户当前具有任何匹配机会
* **已添加到Opportunity**:如果此潜在客户被添加到匹配机会
* **已从Opportunity中删除**:如果此潜在客户从匹配机会中删除

将搜索条件添加为 **约束** 中。 这些限制包括您的机会标准和自定义字段：

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

例如，假设您希望找到机会至少为5,000美元的潜在客户。 拖入 **有机会** 筛选和使用 **已关闭** 和 **金额** 约束：

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>当您使用多个Opportunity过滤器时，您可能会收到错误的答案。 如果您使用两个Opportunity筛选器构建了上面的示例，您将获得一个潜在客户列表，这些潜在客户拥有至少5,000美元的机会和任何已关闭的机会，即使这些机会是单独的机会。

**机会已更新**

的 **机会已更新** 筛选器会在特定机会字段更新后查找任何机会。 选取要与“触发器属性”(Trigger Attribute)下拉列表一起检查的字段，然后使用约束来缩小更改集。

例如，此过滤器将向您显示过去30天内完成其关闭日期更改的所有潜在客户：

![](assets/image2015-6-11-12-3a33-3a7.png)

## Opportunity Triggers {#opportunity-triggers}

以下机会触发器可用。 它们的工作方式与相应的过滤器（如前所述）相同，不同之处在于它们能够在事件发生时立即触发营销活动：

* 机会已更新
* 已添加到Opportunity
* 从Opportunity中删除

例如，您可以使用此智能列表在将任何潜在客户添加到任何商机时触发。 在流程中，您可以将它们添加到营销暂停列表，或向它们发送定向电子邮件。

![](assets/image2015-6-11-12-3a33-3a48.png)

要触发您的机会自定义字段，请使用 **机会已更新** 触发器并选择下拉菜单中的字段：

![](assets/image2015-6-11-12-3a33-3a34.png)
