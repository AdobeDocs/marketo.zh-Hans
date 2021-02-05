---
unique-page-id: 2359947
description: 过渡人员在互动流——营销文档——产品文档
title: 过渡参与流之间的人员
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# 过渡参与流之间的人员{#transition-people-between-engagement-streams}

参与项目可以有多个流。 如果[添加流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)，您将希望定义人们从一个流移动到另一个流的方式。 这些规则称为&#x200B;**过渡规则。**

1. 转到&#x200B;**营销活动**。

   ![](assets/ma.png)

1. 选择您的多流参与项目并转到&#x200B;**流**。

   ![](assets/multistream.jpg)

1. 单击要从其他流中拉入的流的&#x200B;**过渡规则**，然后单击&#x200B;**编辑过渡规则**。

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >过渡规则进入一条河；始终定义要拉入的流的规则。

   打开过渡规则窗口后，查找并拖入所选触发器。 在这种情况下，我们希望在将人员添加到机会时将其迁移到Mid Stage。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 让我们将运算符设置为&#x200B;**是任何**，这样，人员就可以移动，以获得任何添加的机会。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >您可以向过渡规则添加多个触发器和过滤器，但过渡规则使用所有过滤器(只能使用ALL过滤器)。 如果您需要在过渡规则中使用OR，我们建议您设置外部智能活动。

1. 单击&#x200B;**关闭**。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   太好了！ 现在，您的参与项目中任何添加到机会的人员都将移入“中级”流。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >上述步骤&#x200B;*do*&#x200B;也适用于暂停](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)的[用户。
