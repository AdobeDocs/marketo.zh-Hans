---
unique-page-id: 12981050
description: 锁定销售模板 — Marketo文档 — 产品文档
title: 锁定销售模板
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 锁定销售模板 {#lock-sales-template}

为了阻止CRM用户编辑销售模板，管理员可以启用锁定模板的功能，然后允许用户从电子邮件编辑器单独锁定模板。

>[!CAUTION]
>
>此功能仅适用于Salesforce，与Microsoft Dynamics或其他CRM不兼容。 不会锁定从Outlook或Gmail插件访问的模板，因为编辑器不受Marketo控制。

## 启用锁定模板 {#enable-lock-template}

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **管理员**，然后单击 **销售分析**.

   ![](assets/1.png)

1. 下 **设置**，单击 **编辑**.

   ![](assets/2.png)

1. Check **启用锁定模板的功能**. 单击 **保存**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>默认情况下，此框处于选中状态，并且已启用锁定模板的功能。 取消选中该复选框将在电子邮件编辑器中禁用锁定模板功能。

>[!NOTE]
>
>以管理员身份更改此设置将会 **非** 会追溯影响现有模板；即，它不会自动锁定这些模板。

## 在电子邮件编辑器中锁定模板 {#lock-template-in-the-email-editor}

1. 选择要锁定的电子邮件，然后单击 **编辑草稿**.

   ![](assets/5.png)

1. 在电子邮件编辑器中，单击 **电子邮件设置**.

   ![](assets/6.png)

1. Check **发布到Marketo Sales Insight** 如果还没检查过。 您现在可以取消选中 **允许CRM用户编辑电子邮件** 以锁定模板。 单击 **保存**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >默认情况下，此框处于选中状态，并允许CRM用户编辑电子邮件。
