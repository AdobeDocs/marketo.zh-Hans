---
unique-page-id: 12981050
description: 锁定销售模板 — Marketo文档 — 产品文档
title: 锁定销售模板
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 锁定销售模板 {#lock-sales-template}

为防止CRM用户编辑销售模板，管理员可以启用锁定模板的功能，然后允许用户从电子邮件编辑器中单独锁定模板。

>[!CAUTION]
>
>此功能仅适用于Salesforce，且与Microsoft Dynamics或其他CRM不兼容。 从Outlook或Gmail插件访问的模板将不会被锁定，因为编辑器不受Marketo控制。

## 启用锁定模板 {#enable-lock-template}

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **管理员**，然后单击 **销售分析**.

   ![](assets/1.png)

1. 在 **设置**，单击 **编辑**.

   ![](assets/2.png)

1. 检查 **启用锁定模板的功能**. 单击 **保存**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>默认情况下，选中此框并启用锁定模板的功能。 取消选中该复选框将在电子邮件编辑器中禁用锁定模板功能。

>[!NOTE]
>
>将更改此设置作为管理员 **not** 对现有模板产生追溯影响；即不会自动锁定它们。

## 在电子邮件编辑器中锁定模板 {#lock-template-in-the-email-editor}

1. 选择要锁定的电子邮件，然后单击 **编辑草稿**.

   ![](assets/5.png)

1. 在电子邮件编辑器中，单击 **电子邮件设置**.

   ![](assets/6.png)

1. 检查 **发布到Marketo Sales Insight** 如果尚未选中。 您现在可以取消选中 **允许CRM用户编辑电子邮件** 以锁定模板。 单击 **保存**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >默认情况下，此框处于选中状态，CRM用户可以编辑电子邮件。
