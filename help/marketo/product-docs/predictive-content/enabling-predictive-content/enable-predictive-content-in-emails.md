---
unique-page-id: 11385020
description: 在电子邮件中启用预测内容 — Marketo文档 — 产品文档
title: 在电子邮件中启用预测内容
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# 在电子邮件中启用预测内容 {#enable-predictive-content-in-emails}

使您的电子邮件中的一个或多个图像成为预测性图像，为每个收件人定制体验。

>[!NOTE]
>
>建议您在测试和使用预测内容之前，为每个类别和每个源（电子邮件、富媒体、条形图）启用超过五项内容。 更多内容为您提供更好的预测结果。

>[!PREREQUISITES]
>
>在启用预测内容之前，您必须：
>
>* **准备您的预测内容**
>
>   * [编辑电子邮件的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"}或
>   * [编辑富媒体的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"}或
>   * [编辑推荐栏的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [批准预测内容的标题](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## 使用Email 2.0编辑器添加预测内容 {#adding-predictive-content-using-the-email-editor}

1. 单击 **[!UICONTROL Marketing Activities]**。

   ![](assets/one.png)

1. 选择您的电子邮件并单击&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/two.png)

1. 单击要预测的图像。 出现齿轮图标时，单击该图标并选择&#x200B;**[!UICONTROL Enable ContentAI]** （ContentAI是预测内容之前的名称）。

   ![](assets/three.png)

1. 要选择一个或多个类别，请单击&#x200B;**[!UICONTROL Categories]**&#x200B;下拉列表，进行选择，然后单击&#x200B;**[!UICONTROL Apply]**。

   ![](assets/four.png)

   >[!NOTE]
   >
   >选择特定类别或更改预测布局是可选的。

1. 您的图像现在为预测图像。 对其他图像（如果需要）重复步骤3和4。

   ![](assets/five.png)

1. 要预览电子邮件，请单击右上角的&#x200B;**[!UICONTROL Preview]**。

   ![](assets/six.png)

1. 要查看其他可能的图像，请单击&#x200B;**[!UICONTROL Refresh]**。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >在收件人打开电子邮件&#x200B;**_之前，未选择_**&#x200B;图像。 因此，您在预览中看到的只是一个示例，不一定是收件人看到的图像。

1. 预览完电子邮件后，单击&#x200B;**[!UICONTROL Preview Actions]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL Approve and Close]**。 或者，如果您仍然需要编辑，请单击右侧的&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >发送示例时，将选择一个随机图像。

批准电子邮件后，该电子邮件将配备预测内容并可供发送！

>[!CAUTION]
>
>收件人打开电子邮件后，预测图像即被锁定。 如果稍后删除内容，收件人将看到内容所在的损坏图像。

## 在不使用Email 2.0编辑器时添加预测内容 {#adding-predictive-content-when-not-using-the-email-editor}

如果不使用[Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"}模板，则只需将模板中的图像标记为Marketo可编辑的图像元素，即可向电子邮件添加预测内容。

在此处了解[Marketo特定的语法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}。

以下是代码应呈现的外观示例（这只是示例，请不要完全复制下面的代码）。

**示例**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
