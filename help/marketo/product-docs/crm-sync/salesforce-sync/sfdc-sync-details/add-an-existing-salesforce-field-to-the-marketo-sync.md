---
unique-page-id: 4719308
description: 向Marketo同步 — Marketo文档 — 产品文档中添加现有Salesforce字段
title: 将现有Salesforce字段添加到Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 将现有Salesforce字段添加到Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理员权限**

通常，Salesforce中的新自定义字段会自动同步到Marketo。 如果没有，则Marketo同步用户可能看不到这些字段。 这就是你如何解决的。

1. 单击您的名称，然后选择&#x200B;**Setup**。

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. 在左搜索栏中输入&#x200B;**profile**，然后单击&#x200B;**管理用户**&#x200B;下的&#x200B;**Profiles**。

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. 单击同步用户的配置文件。

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. 在&#x200B;**Field-Level Security**&#x200B;部分下，单击包含该字段的对象旁边的&#x200B;**查看**。

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. 单击&#x200B;**编辑**。

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. 选中要添加到同步的字段所对应的&#x200B;**Visible**&#x200B;复选框，然后单击&#x200B;**Save**。

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   真贴心！ 在下一个同步周期中，Marketo将看到字段并启动魔术。

   >[!NOTE]
   >
   > 如果字段在Salesforce中已具有值，则在下次更新记录之前，这些值不会同步到Marketo。
