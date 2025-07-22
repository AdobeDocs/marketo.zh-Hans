---
unique-page-id: 37355569
description: 项目群成员自定义字段 — Marketo文档 — 产品文档
title: 项目群成员自定义字段
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 1%

---

# 项目群成员自定义字段 {#program-member-custom-fields}

程序成员自定义字段允许您收集每个成员的特定于程序的数据。 它们可用于：Marketo表单、智能列表过滤器和触发器，以及智能营销活动流操作。 可在项目群的“成员”选项卡中查看数据。

## 创建项目群成员自定义字段 {#create-a-program-member-custom-field}

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/one.png)

1. 单击 **[!UICONTROL Field Management]**。

   ![](assets/two.png)

1. 单击 **[!UICONTROL New Custom Field]**。

   ![](assets/three.png)

1. 单击&#x200B;**[!UICONTROL Object]**&#x200B;下拉列表并选择所需的对象。

   ![](assets/four.png)

   >[!NOTE]
   >
   >[!UICONTROL Person]和[!UICONTROL Program Member]自定义字段不能共享相同的名称。

1. 填写其余字段，然后单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/five.png)

   >[!NOTE]
   >
   >[!UICONTROL Program Member]自定义字段支持的类型为：布尔值、日期、日期时间、浮点数、整数、字符串、URL。 [了解有关字段类型的更多信息](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}。

## 对象说明 {#object-descriptions}

| 对象 | 描述 |
|---|---|
| 公司 | 与人员关联的公司的名称。 |
| 机会 | 商机可以与个人或帐户关联，作为潜在的未来销售。 他们通常通过CRM或API进入Marketo。 |
| 人员 | 通过营销活动与之接触的Marketo数据库中的个人。 |
| 计划成员 | 同时还是项目群成员的人员 |

## 触发器和过滤器 {#triggers-and-filters}

您可以通过[触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}和/或[筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}，在智能列表中利用此程序特定的数据。

![](assets/six.png)

## 注意事项 {#things-to-know}

* 项目群成员自定义字段仅在本地资产中可用。 Design Studio不支持这些功能，因为无法将它绑定到特定程序。
* 不能将包含程序成员自定义字段的表单（或带有表单的登陆页面）克隆/移动到Design Studio。
* [您可以将](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}项目群成员自定义字段与促销活动成员自定义字段同步。
* 程序成员对象最多可以有20个自定义字段。 这些字段适用于任何项目。
* 当您删除某个项目的成员时，如果他们的项目群成员自定义字段中包含任何数据，则将从该字段中清除该数据。
* 要查看数据，请单击程序中的成员选项卡，然后创建包含这些字段的自定义视图。
* 支持通过[list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}和[API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/home){target="_blank"}导入和导出。 导出仅对项目群成员列表有效，对静态列表无效。
* 合并两个人员时，将使用入选者的项目群成员自定义字段数据。 但是，如果获胜方没有赢家，将使用失败方的价值。
* 项目群成员信息字段不允许更改类型。
* 程序成员自定义字段不支持“包含”智能列表约束。

>[!MORELIKETHIS]
>
>* [在Marketo中创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [程序成员自定义字段同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
