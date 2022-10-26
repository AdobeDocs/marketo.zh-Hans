---
unique-page-id: 4719308
description: 向Marketo同步 — Marketo文档 — 产品文档中添加现有Salesforce字段
title: 将现有Salesforce字段添加到Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 81bc90bcccc8073511c9f331471c0cda9f4147cb
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 将现有Salesforce字段添加到Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理员权限**

通常，Salesforce中的新自定义字段会自动同步到Marketo。 如果没有，则Marketo同步用户可能看不到这些字段。 这就是你如何解决的。

1. 单击您的名称，然后选择 **设置**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 输入 **个人资料** 在左侧搜索栏中，单击 **用户档案** 在 **管理用户**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 单击同步用户的配置文件。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. 在 **字段级别安全性** ，单击 **查看** 字段。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 单击 **编辑**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 检查 **可见** 复选框，然后单击要添加到同步的字段 **保存**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   真贴心！ 在下一个同步周期中，Marketo将看到字段并启动魔术。

   >[!NOTE]
   >
   > 如果字段在Salesforce中已具有值，则在下次更新记录之前，这些值不会同步到Marketo。
