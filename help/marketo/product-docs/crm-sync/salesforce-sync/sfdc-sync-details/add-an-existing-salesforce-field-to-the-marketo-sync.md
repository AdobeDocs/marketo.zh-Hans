---
unique-page-id: 4719308
description: 将现有Salesforce字段添加到Marketo同步 — Marketo文档 — 产品文档
title: 将现有Salesforce字段添加到Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 将现有Salesforce字段添加到Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理员权限**

通常，Salesforce中的新自定义字段会自动同步到Marketo。 如果不能，这些字段可能对Marketo同步用户不可见。 下面是如何解决此问题的。

1. 单击您的姓名，然后选择 **设置**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 输入 **个人资料** 在左搜索栏中单击 **配置文件** 下 **管理用户**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 单击同步用户的配置文件。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. 在 **字段级安全性** 部分，单击 **视图** 在包含字段的对象旁边。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 单击 **编辑**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 查看 **可见** 要添加到同步的字段对应的复选框，然后单击 **保存**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   真贴心！ 在下一个同步周期中，Marketo将看到该字段并开始施展魔术。

   >[!NOTE]
   >
   > 如果该字段在Salesforce中已有值，则这些值在下一次记录更新之前不会同步到Marketo。
