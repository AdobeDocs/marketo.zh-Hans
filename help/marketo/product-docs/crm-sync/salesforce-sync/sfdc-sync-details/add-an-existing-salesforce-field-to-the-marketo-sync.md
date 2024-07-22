---
unique-page-id: 4719308
description: 将现有Salesforce字段添加到Marketo同步 — Marketo文档 — 产品文档
title: 将现有Salesforce字段添加到Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 将现有Salesforce字段添加到Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理员权限**

通常，Salesforce中的新自定义字段会自动同步到Marketo Engage。 如果不能，这些字段可能对Marketo同步用户不可见。 下面是如何解决此问题的。

1. 单击您的名称，然后选择&#x200B;**[!UICONTROL 设置]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 在左侧搜索栏中输入“配置文件”，然后单击“**[!UICONTROL 管理用户]**”下的“**[!UICONTROL 配置文件]**”。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 单击同步用户的配置文件。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. 在&#x200B;**[!UICONTROL 字段级安全性]**&#x200B;部分下，单击包含该字段的对象旁边的&#x200B;**[!UICONTROL 查看]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 单击&#x200B;**[!UICONTROL 编辑]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 选中要添加到同步中的字段的&#x200B;**[!UICONTROL 可见]**&#x200B;复选框，然后单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   在下一个同步周期中，Marketo将看到该字段并开始施展魔术。

   >[!NOTE]
   >
   > 如果该字段在Salesforce中已有值，则这些值在下一次记录更新之前不会同步到Marketo。
