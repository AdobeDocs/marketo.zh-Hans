---
unique-page-id: 11378814
description: 帐户列表 — Marketo文档 — 产品文档
title: 帐户列表
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 帐户列表 {#account-lists}

帐户列表是指可一起定位的已命名帐户集合。 帐户列表允许您按公司的行业、位置或大小定位已命名帐户。

除了帐户列表之外，您还可以创建通过公共CRM帐户视图生成的动态帐户列表。 “CRM帐户视图”是一组规则，在显示帐户时充当过滤器。 例如，您可以使用它查找行业即医疗保健的帐户 *和* 营收超过1亿美元。

![](assets/one.png)

>[!NOTE]
>
>在中构建智能列表和Web营销活动时，在Marketo Target帐户管理中创建的帐户列表会自动可用 [Web个性化](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## 创建新帐户列表 {#create-a-new-account-list}

1. 单击 **新建** 下拉框并选择 **创建新帐户列表**.

   ![](assets/1a.png)

1. 为您的列表提供一个名称并单击 **创建**.

   ![](assets/three-0.png)

1. 创建帐户列表后，开始使用 [向其添加指定帐户](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo将只显示指定帐户数量在2,000个或更少的帐户列表的分析。

## 创建新的动态帐户列表 {#create-a-new-dynamic-account-list}

1. 单击 **新建** 下拉框并选择 **新建动态列表**.

   ![](assets/1.png)

1. 在对话框中，选择 **CRM帐户视图** ，或键入名称以搜索。

   ![](assets/image2017-7-18-9-48-23.png)

1. 单击&#x200B;**创建**。

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >在Salesforce中，确保向同步用户提供列表视图对象权限。

## 重命名帐户列表 {#rename-an-account-list}

>[!NOTE]
>
>这些步骤仅适用于帐户列表。 _动态_ 帐户列表使用其关联的CRM帐户视图的名称。

1. 选择要重命名的帐户，单击 **帐户列表操作** 下拉框并选择 **重命名帐户列表**.

   ![](assets/three.png)

1. 输入新名称，然后单击 **重命名**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >CRM帐户视图每8小时同步一次到动态帐户列表。 如果它们尚未同步，Marketo将在下一个周期中同步它们。

## 删除帐户列表 {#delete-an-account-list}

>[!NOTE]
>
>对于帐户列表和动态帐户列表，这些步骤是相同的。

1. 选择要删除的帐户，单击 **帐户列表操作** 下拉框并选择 **删除帐户列表**.

   ![](assets/five.png)

1. 单击 **删除**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [将现有命名帐户添加到帐户列表](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [帐户列表分析](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)

