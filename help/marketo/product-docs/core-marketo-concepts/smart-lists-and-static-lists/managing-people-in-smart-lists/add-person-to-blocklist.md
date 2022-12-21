---
unique-page-id: 9438139
description: 将人员添加阻止列表到 — Marketo文档 — 产品文档
title: 将人员添加到阻止列表
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 将人员添加到阻止列表 {#add-person-to-blocklist}

将人员添加到您阻止列表的，会阻止他们接收您的通信。

>[!NOTE]
>
>Marketo正在更改黑名单和白名单等术语，以便在我们的产阻止列表品中允许列表和。 在此更新过程中，您可能会在我们的UI和文档屏幕截图中看到旧术语，在我们的文档文本中看到新术语。 我们为任何混淆道歉。

1. [创建新的默认程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) 然后命名 **添加到阻止列表**.

1. 单击 **新建** 选择 **新建本地资产**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. 命名列表并单击 **创建**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. 将所有人员添加到 **智能列表** 要添加到您的阻止列表。

   >[!NOTE]
   >
   >您的阻止列表人员将不会收到操作电子邮件。

   ![](assets/three-6.png)

1. 单击 **新建** 选择 **新的智能营销活动**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. 将 **新的智能营销活动**. 单击&#x200B;**创建**。

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. 拖放 **智能列表成员**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. 选择之前创建的智能列表。

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. 拖放 **更改数据值**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. 对于 **流量**，输入 **列出的块** 对于 **属性** 设置 **新值** to **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. 在 **计划** 选项卡，选择 **运行一次**.

   ![](assets/ten.png)

1. 选择 **立即运行** 单击 **运行**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   耶！ 这些用户将不再收到电子邮件。

   >[!TIP]
   >
   >创建 [触发智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) 使用 **更改数据值** with **列出的块为true** 适用于将来具有可属阻止列表性的所有人。
