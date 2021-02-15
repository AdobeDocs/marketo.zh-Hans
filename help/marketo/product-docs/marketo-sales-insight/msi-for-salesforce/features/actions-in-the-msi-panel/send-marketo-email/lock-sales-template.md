---
unique-page-id: 12981050
description: 锁定销售模板 — Marketo Docs — 产品文档
title: 锁定销售模板
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# 锁定销售模板{#lock-sales-template}

为防止CRM用户编辑销售模板，管理员可以启用锁定模板的功能，然后允许用户从电子邮件编辑器中单独锁定模板。

>[!CAUTION]
>
>此功能仅适用于Salesforce，与Microsoft Dynamics或其他CRM不兼容。 从Outlook或Gmail插件访问的模板将不会被锁定，因为编辑器不受Marketo控制。

## 启用锁定模板{#enable-lock-template}

>[!NOTE]
>
>**需要管理权限**

1. 转至&#x200B;**Admin**，然后单击&#x200B;**Sales Insight**。

   ![](assets/1.png)

1. 在&#x200B;**Settings**&#x200B;下，单击&#x200B;**Edit**。

   ![](assets/2.png)

1. 选中&#x200B;**启用锁定模板的功能**。 单击&#x200B;**保存**。

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>默认情况下，选中此框，并启用锁定模板的功能。 取消选中此选项将在电子邮件编辑器中禁用锁定模板功能。

>[!NOTE]
>
>将此设置更改为管理员将&#x200B;**不会对现有模板产生追溯影响；即，它不会自动锁定它们。**

## 在电子邮件编辑器{#lock-template-in-the-email-editor}中锁定模板

1. 选择要锁定的电子邮件，然后单击&#x200B;**编辑草稿**。

   ![](assets/5.png)

1. 在电子邮件编辑器中，单击&#x200B;**电子邮件设置**。

   ![](assets/6.png)

1. 如果尚未选中&#x200B;**发布到Marketo Sales Insight**，请选中。 您现在可以取消选中&#x200B;**允许CRM用户编辑电子邮件**&#x200B;以锁定模板。 单击&#x200B;**保存**。

   ![](assets/7.png)

   >[!NOTE]
   >
   >默认情况下，此框处于选中状态，并允许CRM用户编辑电子邮件。
