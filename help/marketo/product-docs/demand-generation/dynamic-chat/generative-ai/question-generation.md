---
description: 问题生成 — Marketo文档 — 产品文档
title: 问题生成
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 2%

---

# 问题生成 {#question-generation}

查看您的所有任务及其相关详细信息，例如何时生成任务、问题总数、审批状态等。

## 生成问题 {#generate-questions}

1. 在“生成AI”下，单击&#x200B;**[!UICONTROL Assisted responses]**。

   ![](assets/question-generation-1.png)

1. 单击 **[!UICONTROL Generate questions]**。

   ![](assets/question-generation-2.png)

1. 为您的任务提供一个名称并输入源URL（最多10个），将从其中提取所有内容。 输入所需的主题/关键字，然后在键盘上按Enter键。 完成后，单击&#x200B;**[!UICONTROL Generate]**。

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >要确保Marketo Engage列入允许列表能够从提供的URL中擦除内容，您必须先多个IP地址。 [有关详细信息，请参阅下文](#ip-addresses-to-allowlist)。

   >[!NOTE]
   >
   >站点/页面必须是公共的（即，不隐藏在登录名后面），以便刮取其信息。

1. 根据您的内容，生成问题和响应最多可能需要30分钟。 单击 **[!UICONTROL OK]**。

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >点击刷新以查看问题生成的最新状态。

   ![](assets/question-generation-5.png)

## 下载问题和回答 {#download-questions-and-responses}

>[!NOTE]
>
>生成的问题和响应也可在[响应库](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md)中查看。

1. 找到所需的任务，然后单击其名称旁边的下载图标。

   ![](assets/question-generation-6.png)

1. 在浏览器中找到downloads文件夹，然后选择该文件。 根据您使用的浏览器，这可能看起来有所不同。

   ![](assets/question-generation-7.png)

1. 在Excel文件中，**[!DNL Task details]**&#x200B;仅显示该任务的各种详细信息，包括有关如何添加/编辑问题和/或响应的说明。

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >如果您确实决定批量添加/编辑问题和/或响应，请[了解如何在此处重新上传它们](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md)。

1. **[!DNL Q&Rs]**&#x200B;选项卡提供了其他详细信息，包括生成的问题和响应。

   ![](assets/question-generation-9.png)

## 要允许列表的IP地址 {#ip-addresses-to-allowlist}

为了能够在生成问题和响应期间从Web URL提取内容，请在下面找到您所在的区域，并确保与其关联的IP地址由您的Web团队列入允许列表。

<table width="450">
<thead>
  <tr>
    <th>北美洲</th>
    <th>欧洲</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20.213.91.77</td>
  </tr>
</tbody>
</table>
