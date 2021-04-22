---
unique-page-id: 37355569
description: 项目成员自定义字段 — Marketo文档 — 产品文档
title: 项目成员自定义字段
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 项目成员自定义字段{#program-member-custom-fields}

项目成员自定义字段允许您为每个成员收集特定于项目的数据。 它们可用于：Marketo表单、智能列表过滤器和触发器以及智能活动流动操作。 可在项目的“成员”选项卡中查看数据。

>[!NOTE]
>
>项目成员自定义字段目前未与Salesforce活动成员字段集成。

## 创建项目成员自定义字段{#create-a-program-member-custom-field}

1. 在Marketo中，单击&#x200B;**Admin**。

   ![](assets/one.png)

1. 单击&#x200B;**字段管理**。

   ![](assets/two.png)

1. 单击&#x200B;**新建自定义字段**。

   ![](assets/three.png)

1. 单击“对象”(Object)下拉框并选择所需的对象。

   ![](assets/four.png)

   >[!NOTE]
   >
   >“人员”和“项目成员”自定义字段不能共享同一名称。

1. 填写其余字段，然后单击&#x200B;**创建**。

   ![](assets/five.png)

   >[!NOTE]
   >
   >支持项目成员自定义字段的类型有：boolean、date、datetime、float、integer、string、URL。 [了解有关字段类型的更多信息](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)。

## 对象描述{#object-descriptions}

| 对象 | 说明 |
|---|---|
| 公司 | 与人员关联的公司的名称。 |
| 机会 | 一个机会可以与某个人或帐户关联，作为潜在的未来销售。 他们通常通过CRM或API进入Marketo。 |
| 人 | 您通过营销活动参与的Marketo数据库中的个人。 |
| 项目成员 | 也是项目成员的人 |

## 触发器和过滤器{#triggers-and-filters}

您可以通过[触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)和/或[过滤器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)在智能列表中利用此项目特定数据。

![](assets/six.png)

## {#things-to-know}

* 项目成员自定义字段仅在本地资产中可用。 Design Studio中不支持这些组件，因为无法将其绑定到特定项目。
* 不能将包含项目成员自定义字段的表单(或包含表单的登陆页)克隆/移动到Design Studio。
* “项目成员”对象最多可包含20个自定义字段。 这些字段可用于任何项目。
* 当您删除项目的成员时，如果他们的项目成员自定义字段中有任何数据，则将从该字段中删除数据。
* 要视图数据，请单击项目中的成员选项卡，并创建包含这些字段的自定义视图。
* 支持通过[列表](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)和[API](https://developers.marketo.com/)导入和导出。
* 合并两个人时，将使用入选方的项目成员自定义字段数据。 但如果胜者没有，那么输家的价值就会被利用。

>[!MORELIKETHIS]
>
>[在Marketo中创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
