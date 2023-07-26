---
unique-page-id: 2359675
description: 禁用表单字段预填充 — Marketo文档 — 产品文档
title: 禁用表单字段的预填充
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 禁用表单字段的预填充 {#disable-pre-fill-for-a-form-field}

未知(cookie)Web访客时，默认情况下，Marketo表单会使用他们的信息预填充字段。 如果您想关闭此功能，请按照以下步骤操作。

>[!NOTE]
>
>**表单预填** 默认处于启用状态。 登陆页面级别预填充设置和管理级别预填充设置优先于表单级别设置：
>
>表单>登陆页面>管理员

## 如何禁用预填充 {#how-to-disable-pre-fill}

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-7.png)

1. 选择您的表单并单击 **编辑表单**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >在将表单嵌入到您自己的页面时，表单预填充不起作用。 它仅适用于Marketo登陆页面。

1. 选择一个字段并设置 **表单预填** 到 **已禁用**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >您还可以在登陆页面级别或管理员级别禁用表单预填充。

1. 单击 **完成**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. 单击 **批准并关闭**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## 敏感字段 {#sensitive-fields}

当您 [将字段标记为敏感](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md)，阻止在表单中预填其值，您将在预填选项中看到此信息。

![](assets/disable-pre-fill.png)