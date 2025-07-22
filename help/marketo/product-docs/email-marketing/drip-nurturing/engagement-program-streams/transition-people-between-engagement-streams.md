---
unique-page-id: 2359947
description: 在参与流之间过渡人员 — Marketo文档 — 产品文档
title: 在参与流之间过渡人员
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 在参与流之间过渡人员 {#transition-people-between-engagement-streams}

参与计划可以有多个流。 如果您[添加流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)，您将需要定义用户从一个流移动到另一个流的方法。 这些规则称为&#x200B;**过渡规则。**

1. 转到&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/ma.png)

1. 选择您的多流参与计划并转到&#x200B;**[!UICONTROL Streams]**。

   ![](assets/multistream.jpg)

1. 单击要从其他流拉入的流的&#x200B;**[!UICONTROL Transition Rules]**，然后单击&#x200B;**[!UICONTROL Edit Transition Rules]**。

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >过渡规则提取到流中；始终定义要提取到的流中的规则。

   打开过渡规则窗口后，在您选择的触发器中进行查找和拖动。 在本例中，我们希望将添加到机会中的人员移入[!UICONTROL Mid Stage]。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 让我们将运算符设置为&#x200B;**[!UICONTROL is any]**，这样人员就可以移过该运算符来查找任何添加的机会。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >您可以将多个触发器和过滤器添加到过渡规则，但过渡规则会使用所有过滤器（使用所有过滤器是唯一的选项）。 如果您需要在过渡规则中使用OR，我们建议您改为设置外部智能营销活动。

1. 单击 **[!UICONTROL Close]**。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   太棒了！ 现在，您的参与计划中添加到商机的任何人员都将移到[!UICONTROL Mid Stage]流中。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >上述&#x200B;*do*&#x200B;步骤也适用于[暂停时](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)的人员。
