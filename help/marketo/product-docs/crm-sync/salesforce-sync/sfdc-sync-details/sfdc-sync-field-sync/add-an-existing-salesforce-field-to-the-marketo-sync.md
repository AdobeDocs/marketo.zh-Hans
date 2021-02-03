---
unique-page-id: 4719308
description: 将现有Salesforce字段添加到Marketo Sync - Marketo Docs —— 产品文档
title: 将现有Salesforce字段添加到Marketo同步
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# 向Marketo同步{#add-an-existing-salesforce-field-to-the-marketo-sync}添加现有Salesforce字段

>[!NOTE]
>
>**需要管理员权限**

通常，Salesforce中的新自定义字段会自动同步到Marketo。 否则，Marketo Sync用户可能无法看到这些字段。 这是你如何解决的。

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

   真贴心！ 在下一个同步周期中，Marketo将看到该字段，并开始魔术。

   >[!NOTE]
   >
   > 如果字段在Salesforce中已有值，则直到下一个记录更新，这些值才会同步到Marketo。
