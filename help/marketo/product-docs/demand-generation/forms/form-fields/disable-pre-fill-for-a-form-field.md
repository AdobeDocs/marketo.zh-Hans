---
unique-page-id: 2359675
description: 禁用表单字段的预填写 — Marketo文档 — 产品文档
title: 禁用表单字段的预填
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 禁用表单字段的预填 {#disable-pre-fill-for-a-form-field}

当Web访客已知(Cookie)时，Marketo表单将默认预填充字段及其信息。 如果你想关闭这个，请看这个。

>[!NOTE]
>
>**表单预填充** 默认情况下处于启用状态。 登陆页面级别的预填充设置和管理员级别的预填充设置，而不是表单级别设置：
>
>表单>登陆页面>管理员

## 如何禁用预填充 {#how-to-disable-pre-fill}

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-7.png)

1. 选择您的表单并单击 **编辑表单**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >在您自己的页面上嵌入表单时，表单预填充不起作用。 它仅适用于Marketo登陆页。

1. 选择一个字段并设置 **表单预填充** to **已禁用**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >您还可以在登陆页面级别或管理员级别禁用表单预填。

1. 单击 **完成**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. 单击 **批准并关闭**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## 敏感字段 {#sensitive-fields}

当您 [将字段标记为敏感](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md)，以阻止其值在表单中预填充，您将在“预填充”选项中看到此内容。

![](assets/disable-pre-fill.png)