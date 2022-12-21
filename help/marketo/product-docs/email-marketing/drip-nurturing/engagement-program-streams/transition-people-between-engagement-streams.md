---
unique-page-id: 2359947
description: 在参与流 — Marketo文档 — 产品文档之间迁移人员
title: 在参与流之间迁移人员
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 在参与流之间迁移人员 {#transition-people-between-engagement-streams}

参与项目可以有多个流。 如果您 [添加流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)，则需要定义用户从一个流移动到另一个流的方式。 这些名称 **过渡规则。**

1. 转到 **营销活动**.

   ![](assets/ma.png)

1. 选择您的多流参与计划并转到 **流**.

   ![](assets/multistream.jpg)

1. 单击 **过渡规则** 对于要从其他流提取到的流，请单击 **编辑过渡规则**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >过渡规则进入流；始终定义要提取到的流中的规则。

   打开过渡规则窗口后，在您选择的触发器中查找并拖动。 在这种情况下，我们希望在将人员添加到机会中时，将其移入Mid Stage。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 我们将运算符设置为 **any** 这样人们就会搬过来，以获得更多的机会。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >您可以向过渡规则中添加多个触发器和过滤器，但过渡规则使用所有过滤器（只能使用“全部过滤器”选项）。 如果您需要在过渡规则中使用OR，我们建议您改为设置外部智能营销活动。

1. 单击&#x200B;**关闭**。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   太棒了！ 现在，您的参与项目中任何添加到商机的人员都将被移至中端流。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >上述步骤 *do* 适用于 [在暂停时](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) 也是。
