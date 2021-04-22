---
unique-page-id: 4719308
description: 向Marketo同步 — Marketo文档 — 产品文档中添加现有Salesforce字段
title: 向Marketo同步添加现有Salesforce字段
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 向Marketo同步{#add-an-existing-salesforce-field-to-the-marketo-sync}添加现有Salesforce字段

>[!NOTE]
>
>**需要管理权限**

通常，Salesforce中的新自定义字段会自动同步到Marketo。 否则，Marketo Sync用户可能看不到这些字段。 您可以通过以下方式来解决此问题。

1. 单击您的姓名，然后选择&#x200B;**Setup**。

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. 在左搜索栏中输入&#x200B;**用户档案**，然后单击&#x200B;**管理用户**&#x200B;下的&#x200B;**用户档案**。

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. 单击同步用户的用户档案。

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. 在&#x200B;**字段级安全**&#x200B;部分下，单击包含字段的对象旁边的&#x200B;**视图**。

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. 单击&#x200B;**编辑**。

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. 选中要添加到同步的字段的&#x200B;**Visible**&#x200B;复选框，然后单击&#x200B;**Save**。

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   真贴心！ 在下一个同步周期中，Marketo将看到该字段并开始该魔术。

   >[!NOTE]
   >
   > 如果字段在Salesforce中已有值，则直到下次更新记录时，这些值才会同步到Marketo。
