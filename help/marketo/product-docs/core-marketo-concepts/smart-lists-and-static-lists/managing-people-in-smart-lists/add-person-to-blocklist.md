---
unique-page-id: 9438139
description: 将人添加阻止列表到- Marketo Docs —— 产品文档
title: 将人添加到阻止列表
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# 将人添加到阻止列表 {#add-person-to-blocklist}

将人添加到您的阻止列表会阻止他们收到您的信件。

>[!NOTE]
>
>Marketo正在更改黑名单和白名单等术语，以在我们的产阻止列表品中进允许列表行和。 在此更新过程中，您可能会在我们的UI和文档屏幕截图中看到旧条款，在我们的文档文本中看到新条款。 我们为任何混淆表示歉意。

1. [创建新的默认项目](../../../../product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) ，并将其命 **名为“添阻止列表加”**。
1. 单击 **新建** ，然后选择 **新建本地资产**。

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. 命名列表，然后单 **击创建**。

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. 将所有人添加到您 **的智能列表** ，以便添加到您的阻止列表。

   >[!NOTE]
   >
   >您的人阻止列表员不会收到操作电子邮件。

   ![](assets/three-6.png)

1. 单击 **新建** ，然后选 **择新建智能活动**。

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. 命名新 **智能活动**。 单击 **创建**。

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. 拖放智 **能列表的成员**。

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. 选择您刚刚创建的智能列表。

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. 拖放更改 **数据值**。

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. 对于流 ****，为“属性” **输入** “列出的块 **”，并将** “新值”设 ********&#x200B;置为真。

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. 在“计划 **”选** 项卡上，选 **择“运行一次**”。

   ![](assets/ten.png)

1. 选择 **立即运行** ，然后单 **击运行**。

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   耶！ 这些人将不再收到电子邮件。

   >[!TIP]
   >
   >使用“更 [改数据值并列出块](../../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) ”创建触 **发器智能活动，这****** 对于将来具有可属性的所有人而言是阻止列表真的。

