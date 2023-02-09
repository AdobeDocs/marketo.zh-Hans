---
unique-page-id: 11378814
description: 帐户智能列表 — Marketo文档 — 产品文档
title: 帐户智能列表
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
source-git-commit: adff42d54d7953c9ec72e4d736ce0153502be960
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 帐户智能列表 {#account-smart-lists}

下面介绍如何快速准确地识别您的高价值客户。

>[!NOTE]
>
>此功能仅适用于同时具有Target帐户管理加载项和已颁发TAM许可的用户。

## 创建帐户智能列表 {#create-an-account-smart-list}

1. 在Marketo，转到 **营销活动**.

   ![](assets/account-smart-lists-1.png)

1. 查找并选择所需的程序。

   ![](assets/account-smart-lists-2.png)

1. 单击 **新建** 下拉框并选择 **新建本地资产**.

   ![](assets/account-smart-lists-3.png)

1. 单击 **帐户智能列表**.

   ![](assets/account-smart-lists-4.png)

1. 输入名称并单击 **创建** （描述和标签是可选的）。

   ![](assets/account-smart-lists-5.png)

您的帐户智能列表已创建！ 有关定义其规则的步骤，请参阅下文。

## 帐户智能列表规则 {#account-smart-list-rules}

帐户智能列表的工作方式与标准智能列表类似，但有一个显着例外：容器。

1. 要定义帐户智能列表，请单击 **帐户智能列表规则** 选项卡。

   ![](assets/account-smart-lists-6.png)

1. 选择所需的帐户过滤器。 在本例中，我们选择 _行业是医疗保健_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >在 [帐户分析排名和调整](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) 将显示为自定义帐户属性，以供在帐户智能列表中使用。 此自定义属性数据基于创建/更新帐户配置文件模型的时间。

1. 选择匹配的人员筛选器。 在本例中，我们选择 _加利福尼亚州_.

   ![](assets/account-smart-lists-9.png)

**可选步骤**:这是集装箱的入口。 如果您选择其他匹配的人员过滤器，则可以将其放在第一个过滤器下方，或 _in_ 创建容器。 在本例中，我们通过添加 _职位是首席财务官_.

![](assets/account-smart-lists-10.png)

容器的外观如下。

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>创建过滤器容器会创建“和”规则，这意味着它将只返回所有合并的结果。 在本例中，客户是医疗保健行业的客户，并位于加利福尼亚州 _和_ 被列为首席财务官的人。 如果您不想使用容器，只需将过滤器放在现有容器的下方/上方。

就这样！ 请查看下面的部分，了解如何利用您的帐户智能列表。

>[!TIP]
>
>与使用标准智能列表一样，您可以使用高级逻辑进一步优化结果。 为此，您至少需要三个过滤器，而在帐户智能列表中，一个容器（不管其本身包含多少个过滤器）等于一个过滤器。

## 帐户智能列表操作 {#account-smart-list-actions}

在帐户智能列表的概述选项卡中，您会注意到一些操作选项。

**导出**:这会将帐户智能列表的结果导出为CSV。

**克隆**:制作帐户智能列表的副本。

**发送到广告网络**:将列表作为新的匹配受众发送到LinkedIn。

您还可以在标准智能营销活动/列表中使用 _帐户智能列表的人员成员_ 过滤器。

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>智能帐户列表的人员成员结果将显示已识别帐户中的每个人，而不只是显示通过智能帐户列表中的匹配人员过滤器找到的人员。

>[!NOTE]
>
>**条件**
>
>**帐户智能列表的人员成员**:在本例中，“会员”一词是指账户本身，因此“人员”是指这些账户中的实际人员(Marketo记录)。
