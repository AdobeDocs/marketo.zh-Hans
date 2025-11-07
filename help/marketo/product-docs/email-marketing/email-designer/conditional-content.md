---
solution: Marketo Engage
product: marketo
title: 条件内容
description: 在电子邮件中使用条件内容以根据收件人动态显示内容。
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 6b9f6d4b276115e1f3f3dac73eb64e5358a76516
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# 条件内容 {#conditional-content}

条件内容允许您动态控制哪些受众可查看哪些内容。 使用现有分段根据预定义标准确定收件人看到的内容。

>[!PREREQUISITES]
>
>已创建至少一个分段[&#128279;](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)并批准[&#128279;](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)。

## 添加条件内容 {#add-conditional-content}

1. 打开所需的电子邮件，然后单击&#x200B;**编辑电子邮件内容**。

   ![](assets/conditional-content-1.png)

1. 选择要作为条件内容的内容（在本例中，我们将选择页眉图像）。 单击&#x200B;_启用条件内容_&#x200B;图标。

   ![](assets/conditional-content-2.png)

1. 高亮框变为橙色。 在左侧，单击&#x200B;_选择条件_&#x200B;图标(![](assets/icon-select-condition.png))以定义变体。

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. 选择所需的区段，然后单击&#x200B;**选择**。

   ![](assets/conditional-content-4.png)

1. 单击&#x200B;_编辑图像_&#x200B;图标以替换变体的现有图像。 选择新图像的源。 在本例中，我们在Marketo Engage订阅中选择&#x200B;_图像和文件_&#x200B;库。

   ![](assets/conditional-content-5.png)

1. 选择适用的图像并单击&#x200B;**选择**。

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. 此时会出现新图像。 最好重命名您的变体，使其更易于识别。 只需单击省略号并选择&#x200B;**重命名**。

   >[!NOTE]
   >
   >单击省略号还可让您查看变体的定义条件并复制它。 如果有多个变体，则可以使用删除选项。 如果您只有一个变体，则删除该变体的方法只是重新单击&#x200B;_启用条件内容_&#x200B;图标（将鼠标悬停在该变体上时，它现在会显示&#x200B;_禁用条件内容_）。

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. 要添加其他变体（可选），请单击&#x200B;**添加变体**&#x200B;并按照相同的步骤操作。

   ![](assets/conditional-content-8.png)

1. 完成后，每个变体都会显示您选择的内容。

   ![](assets/conditional-content-9.gif)

1. 收件人可根据每个区段中定义的规则查看内容。 在上面的示例中，在您的Marketo Engage场&#x200B;_最喜爱的运动_&#x200B;中列出“足球”的每个人都将看到足球图像。

>[!MORELIKETHIS]
>
>* [定义区段规则](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [在Marketo中创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
