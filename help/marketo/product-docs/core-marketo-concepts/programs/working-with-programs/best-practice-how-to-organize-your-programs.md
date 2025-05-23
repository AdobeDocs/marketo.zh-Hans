---
unique-page-id: 6848705
description: 最佳实践 — 如何整理程序 — Marketo文档 — 产品文档
title: 最佳实践 — 如何组织程序
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# 最佳实践：如何组织项目 {#best-practice-how-to-organize-your-programs}

可通过多种方式在营销活动中组织树以及单个项目的内容。 但是，某些方法更好，并且将有助于营销部门的人员。

>[!TIP]
>
>有一天（晋升后！），其他人会试图理解您的计划。 良好的组织将有助于他们快速提高工作效率。

## 文件夹 {#folders}

在营销活动中，您应使用文件夹来组织项目。 我们建议的结构如下例所示：

>[!NOTE]
>
>**示例**
>
>* 有效的营销计划
>   * 电子邮件
>   * 事件
>      * 现场活动/路演
>      * 贸易展
>      * 网络研讨会
>   * 快讯
>   * 客户培养
>   * Web内容
>   * Web窗体
>* 学习
>* 可操作
>   * 生命周期
>   * 评分
>   * 数据管理
>* 销售分析
>   * 有趣的时刻
>   * 销售电子邮件
>   * 销售请求的营销活动
>* **存档**
>   * 存档事件
>      * 存档2012
>      * 存档2013

本示例中提到的每个内容都是一个文件夹。 请注意它们是如何唯一命名的。 可以在INSIDE程序中有重复（更简单的）文件夹名称，但不能在树的根目录下使用。

>[!TIP]
>
>“存档”文件夹是一种特殊类型的文件夹，旨在从选定列表以及报表中删除项目。 这将帮助您的系统更快地运行。 了解[有关文件夹](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md){target="_blank"}的更多信息。

您当然可以按照自己的需要添加更多文件夹。 请记住，贵公司中未来的营销人员将服从您关于如何命名/组织产品的决策。

## 命名方案 {#naming-schemes}

命名至关重要，因为Marketo的功能都使用通用语言进行通信。 对于项目，您应该为其命名一些唯一的名称。 **任何两个程序不能具有相同的名称**。 最佳实践为使用以下格式：

[程序类型]的缩写[YYYY]-[MM]-[可选DD] [简要说明]

>[!NOTE]
>
>**示例**
>
>示例程序名称：
>
>1. ES 2015-09-21构件简介
>1. NL 2015-06新闻稿
>1. WBN 2015-12-01网络研讨会主题

您的订阅中的程序名称必须是唯一的，即使是在不同的[工作区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md){target="_blank"}中。  对于程序内的本地资产，规则是&#x200B;**保持名称简单**。 只需将邀请命名为“邀请”，而不是“2015年6月网络研讨会邀请”。 由于这些程序位于程序中，因此当从其他位置选择父程序时，父程序会自动成为名称的一部分。 换言之，本地资产只需在项目中是唯一的。 你可以拥有数百个名为“邀请”的资产，每个资产都位于不同的程序中，这不会让你一团糟。

## 令牌 {#tokens}

令牌使用文件夹和程序作为工具，来设置要由登陆页面、电子邮件和其他资产使用的变量。

通过上述组织，可将令牌放入事件文件夹中，以便级联到所有事件中。

>[!NOTE]
>
>**示例**
>
>**您的公司地址**。 使用令牌，而不是每次都写入令牌。 这样，您就可以在一个位置更新它，而无需创建大量草稿。 然后根据需要覆盖较低级别文件夹中的令牌。

## 事件 {#events}

事件通常包含许多移动部分，包括：邀请、登陆页面、表单、社交小部件和智能营销活动。 为了便于使用，最佳实践是按照事件的阶段来整理它们。 以下是您的文件夹树应如何查找事件的示例。

![](assets/capture.png)

## 参与计划 {#engagement-programs}

了解[所有参与计划](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md){target="_blank"}。 组织参与计划的最佳方法是使用文件夹。 为每个流创建一个文件夹，然后将电子邮件或程序放入该文件夹。 当内容过期并且您想要删除它时，请在每个流中包含一个存档文件夹。

## 运行程序 {#operational-programs}

它们用于数据清理目的。 具有运行程序的日期的文件夹，然后存档这些文件夹。 通过使该程序可运行，您将其从报表中省略，这有利于此类活动。

## 嵌套电子邮件程序 {#nesting-email-programs}

“电子邮件程序”旨在成为您进行邮件爆破的工具。 您可以将其放入活动或其他促销活动、邀请和提醒项目中。 它们附带一个很酷的仪表板和其他A/B测试功能。 此外，它们还可在项目计划视图中轻松操作。

您还可以将电子邮件程序作为独立程序来创建。 不允许将电子邮件程序嵌入其他电子邮件程序。 那太疯狂了！

## 正在克隆 {#cloning}

Marketo中最酷的功能之一是克隆程序。 这意味着您可以设置项目“模板”，其中包含您想要的所有智能营销活动和电子邮件。 提前设置它，然后克隆它以用于您的下一个营销计划。

>[!TIP]
>
>请注意顶部示例中的事件模板。 将不同类型的事件放在其中以方便克隆。

有些人甚至将电子邮件和登陆页面中的大部分文本抽象为令牌。 这允许您克隆并编辑令牌。 最后，转到项目计划视图，调整日期并且您结束。 看！

## 摘要 {#summary}

如你所见，Marketo权力很大。 我们在此介绍了基本知识，但请考虑由[Marketo Engage专家](https://business.adobe.com/products/marketo/services-support.html){target="_blank"}提供的其他服务以进行微调并为获得成功做好准备。
