---
unique-page-id: 6848782
description: 使您的取消订阅消息在语言- Marketo Docs —— 产品文档中保持动态
title: 使取消订阅消息在语言中具有动态性
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---


# 使取消订阅消息对语言{#make-your-unsubscribe-message-dynamic-for-languages}具有动态性

默认的取消订阅消息和链接为英语。 您可以使用动态内容以不同语言显示它。

>[!NOTE]
>
>下面我们为您设置了这个不错的教程。 它代表了一种最佳实践，但可以通过其他方式实现。

1. 准备数据
1. [创建名为“](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)首选语言”的自定义字段。（如果希望此字段同步，请在CRM中设置它）。

   >[!TIP]
   >
   >以后，当您[创建表单](../../../../product-docs/demand-generation/forms/creating-a-form/create-a-form.md)以捕获语言首选项时，请使用此字段。

1. 创建分段
1. 转到&#x200B;**Database**。
** ![](assets/db.png)

   **

1. 在&#x200B;**新建**&#x200B;下拉框中，单击&#x200B;**新建分段**。

   ![](assets/two.png)

1. 命名分段&#x200B;**首选语言**。 单击&#x200B;**添加区段**。 键入语言。

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >默认区段为英语。

1. 继续添加区段，直到您的所有语言都显示出来。 单击&#x200B;**创建**。

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. 选择区段。

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. 转到&#x200B;**智能列表**&#x200B;选项卡。 在搜索字段中输入&#x200B;**首选语言**。 将滤镜拖放到画布上。

   ![](assets/six.png)

1. 设置相应的语言。

   ![](assets/seven.png)

1. 对所有不同语言重复上述步骤。 然后，选择&#x200B;**分段操作**&#x200B;下拉框并单击&#x200B;**批准**。

   ![](assets/image2015-3-9-8-3a39-3a36.png)

1. 创建代码片断
1. 转到&#x200B;**Design Studio**。

   ![](assets/ds.png)

1. 在&#x200B;**New**&#x200B;下拉列表中，单击&#x200B;**New Dispet**。

   ** ![](assets/ten.png)

   **

1. 将代码片段命名为&#x200B;**取消订阅消息**。 单击&#x200B;**创建**。

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. 键入默认的取消订阅消息，突出显示该消息，然后单击超链接图标。

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. 复制并粘贴此令牌：**`{{system.unsubscribeLink}}`**&#x200B;进入&#x200B;**链接URL**&#x200B;字段。 单击&#x200B;**插入**。

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. 在“分段”部分选择&#x200B;**“分段依据”**。

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. 在“分段”下拉框中，键入&#x200B;**Preferred**&#x200B;并选择&#x200B;**Preferred Language**。 单击&#x200B;**保存**。

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. 从树中选择区段。 以该语言键入您的取消订阅消息。

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. 复制并粘贴同一令牌：**`{{system.unsubscribeLink}}`**&#x200B;进入&#x200B;**链接URL**&#x200B;字段。 单击&#x200B;**插入**。

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. 对所有细分重复上述步骤。 然后，返回Design Studio，单击&#x200B;**代码片断操作**&#x200B;下拉框，然后单击&#x200B;**批准**。

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   太棒了。 快到了。

1. 在电子邮件中使用代码片断
1. 在电子邮件编辑器中，单击可编辑的元素。 然后，单击齿轮图标并选择&#x200B;**替换为代码片断**。 如果要选择可编辑的片段元素，请单击齿轮图标，然后选择&#x200B;**编辑**。

   ![](assets/4.1.png)

1. 从下拉列表中查找并选择您的代码片断，然后单击&#x200B;**保存**。

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. 要测试，请单击&#x200B;**返回**...

   ![](assets/4.3.png)

1. ...然后，选择&#x200B;**Dynamic**&#x200B;选项卡。

   ![](assets/4.4.png)

1. 单击不同语言可查看代码片段的更改。

   ![](assets/4.5.png)

   >[!TIP]
   >
   >当然，您还可以编辑电子邮件的其余部分，使用动态语言。 在退订页面上执行相同的操作。

1. 使用动态内容自定义取消订阅页面

   如果您希望人员使用其首选语言进入取消订阅页面，则可以在登陆页和确认页面上使用动态内容。

   导航到Design Studio。

   ![](assets/ds.png)

   在搜索字段中键入“取消订阅”。 您应该找到您的取消订阅页面。

   ![](assets/image2015-3-9-8-3a51-3a53.png)

   单击“编辑草稿”。

   ![](assets/image2015-3-9-8-3a52-3a23.png)

   选择区段依据。

   ![](assets/image2015-3-9-8-3a52-3a57.png)

   查找首选语言部分。 单击“保存”。

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   为每个登陆页编辑内容、批准，一切就绪！

   >[!NOTE]
   >
   >**深潜**
   >
   >
   >进一步了解[动态内容](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md)以及您可以做的所有最酷的事情。

