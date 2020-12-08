---
unique-page-id: 6848782
description: 使您的取消订阅消息在语言- Marketo Docs —— 产品文档中保持动态
title: 使取消订阅消息在语言中具有动态性
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---


# 使取消订阅消息在语言中具有动态性 {#make-your-unsubscribe-message-dynamic-for-languages}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

默认的取消订阅消息和链接为英语。 您可以使用动态内容以不同语言显示它。

>[!NOTE]
>
>下面我们为您设置了这个不错的教程。 它代表了一种最佳实践，但可以通过其他方式实现。

1. 准备数据
1. [创建名为“](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)首选语言”的自定义字段。 （如果希望此字段同步，请在CRM中设置它）。

   >[!TIP]
   >
   >将来，在创建表单时使 [用此字段](../../../../product-docs/demand-generation/forms/creating-a-form/create-a-form.md) ，以捕获语言首选项。

1. 创建分段
1. 转到数 **据库**。** ![](assets/db.png)

   **

1. 在“新 **建** ”下拉框中，单 **击“新建分段**”。

   ![](assets/two.png)

1. 将分段命名为“首 **选语言”**。 单击 **添加区段**。 键入语言。

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >默认区段为英语。

1. 继续添加区段，直到您的所有语言都显示出来。 单击 **创建**。

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. 选择区段。

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. 转至“智能 **列表** ”选项卡。 在搜 **索字段中输入** “首选语言”。 将滤镜拖放到画布上。

   ![](assets/six.png)

1. 设置相应的语言。

   ![](assets/seven.png)

1. 对所有不同语言重复上述步骤。 然后，选择“ **分段操作** ”下拉框并单击 **批准**。

   ![](assets/image2015-3-9-8-3a39-3a36.png)

1. 创建代码片断
1. 转到Design **Studio**。

   ![](assets/ds.png)

1. 在“新建 **”下拉** 菜单中，单 **击“新建代码片段**”。

   ** ![](assets/ten.png)

   **

1. 将代码片段命 **名为取消订阅消息**。 单击 **创建**。

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. 键入默认的取消订阅消息，突出显示该消息，然后单击超链接图标。

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. 复制并粘贴此令牌： **`{{system.unsubscribeLink}}`** 链接 **URL字段** 。 单击 **插入**。

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. 在“ **分段** ”部分中选择“分段依据”。

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. 从“分段”下拉框中，键入“首选 **语言** ”并选 **择“首选语言”**。 单击 **保存**。

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. 从树中选择区段。 以该语言键入您的取消订阅消息。

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. 复制并粘贴同一令牌： **`{{system.unsubscribeLink}}`** 链接 **URL字段** 。 单击 **插入**。

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. 对所有细分重复上述步骤。 然后，返回Design Studio，单击“代码片断 **操作** ”下拉框，然后单 **击“批准**”。

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   太棒了。 快到了。

1. 在电子邮件中使用代码片断
1. 在电子邮件编辑器中，单击可编辑的元素。 然后，单击齿轮图标，并选择“ **替换为代码片断”**。 如果要选择可编辑的片段元素，请单击齿轮图标，然后选择“编 **辑”**。

   ![](assets/4.1.png)

1. 从下拉列表中选择查找并选择您的代码片段，然后单击“ **保存**”。

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. 要测试它，请单击“ **上**&#x200B;一步……”

   ![](assets/4.3.png)

1. ...然后，选择 **“动态** ”选项卡。

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
   >进一步了 [解动态内](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) 容和您可以做的所有最酷的事情。

