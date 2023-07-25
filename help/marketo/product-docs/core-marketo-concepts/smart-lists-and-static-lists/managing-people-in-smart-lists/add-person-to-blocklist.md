---
unique-page-id: 9438139
description: 将人员添加到阻止列表- Marketo文档 — 产品文档
title: 将人员添加到阻止列表
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 将人员添加到阻止列表 {#add-person-to-blocklist}

将人员添加到您的阻止列表会阻止他们接收您的信件。

>[!NOTE]
>
>Marketo正在将黑名单和白名单等术语更改为产品中的阻止列表允许列表和。 在本次更新中，您可能会在UI和文档屏幕截图中看到旧术语，并在文档文本中看到新术语。 造成任何混淆，我们深表歉意。

1. [创建新的默认程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) 并为其命名 **添加到阻止列表**.

1. 单击 **新** 并选择 **新建本地资产**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. 命名列表并单击 **创建**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. 将所有人员添加到您的 **智能列表** 您希望将添加到阻止列表。

   >[!NOTE]
   >
   >您阻止列表上的人员不会收到操作电子邮件。

   ![](assets/three-6.png)

1. 单击 **新** 并选择 **新建智能营销活动**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. 命名 **新建智能营销活动**. 单击&#x200B;**创建**。

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. 拖放 **智能列表的成员**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. 选择您刚刚创建的智能列表。

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. 拖放 **更改数据值**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. 对于 **流量**，输入 **已列出阻止** 对于 **属性** 和设置 **新值** 到 **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. 在 **计划** 选项卡，选择 **运行一次**.

   ![](assets/ten.png)

1. 选择 **立即运行** 并单击 **运行**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   耶！ 这些用户将不再收到电子邮件。

   >[!TIP]
   >
   >创建 [触发智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) 使用 **更改数据值** 替换为 **列出的块为true** 面向所有未来具有阻止列表属性的人。
