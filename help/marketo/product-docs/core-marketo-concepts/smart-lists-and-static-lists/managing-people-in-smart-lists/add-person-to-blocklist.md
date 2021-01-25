---
unique-page-id: 9438139
description: 将人添加阻止列表到- Marketo Docs —— 产品文档
title: 将人添加到阻止列表
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# 将人员添阻止列表加到{#add-person-to-blocklist}

将人添加到您的阻止列表会阻止他们收到您的信件。

>[!NOTE]
>
>Marketo正在更改黑名单和白名单等术语，以在我们的产阻止列表品中进允许列表行和。 在此更新过程中，您可能会在我们的UI和文档屏幕截图中看到旧条款，在我们的文档文本中看到新条款。 我们为任何混淆表示歉意。

1. [新建一个默认程](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) 序并将其命 **名为“添阻止列表加”**。

1. 单击&#x200B;**新建**，然后选择&#x200B;**新建本地资产**。

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. 命名列表，然后单击&#x200B;**创建**。

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. 将所有人添加到您的&#x200B;**智能列表**，您希望将其添加到您的阻止列表。

   >[!NOTE]
   >
   >您的人阻止列表员不会收到操作电子邮件。

   ![](assets/three-6.png)

1. 单击&#x200B;**新建**&#x200B;并选择&#x200B;**新建智能活动**。

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. 命名&#x200B;**新智能活动**。 单击&#x200B;**创建**。

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. 拖放&#x200B;**智能列表的成员**。

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. 选择您刚刚创建的智能列表。

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. 拖放&#x200B;**更改数据值**。

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. 对于&#x200B;**Flow**，输入&#x200B;**属性**&#x200B;的&#x200B;**Block Listed**&#x200B;并将&#x200B;**New Value**&#x200B;设置为&#x200B;**true**。

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. 在&#x200B;**计划**&#x200B;选项卡上，选择&#x200B;**运行一次**。

   ![](assets/ten.png)

1. 选择&#x200B;**立即运行**&#x200B;并单击&#x200B;**运行**。

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   耶！ 这些人将不再收到电子邮件。

   >[!TIP]
   >
   >使用&#x200B;**更改数据值**&#x200B;创建[触发智能活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)，其中&#x200B;**列出的块为true**，以便将来具有可属性的所阻止列表有人。
