---
unique-page-id: 2359545
description: 定义A/B测试入选者标准 — Marketo文档 — 产品文档
title: 定义A/B测试入选者标准
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 定义A/B测试入选者标准 {#define-the-a-b-test-winner-criteria}

当[将A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}添加到您的电子邮件计划时，您需要选择一个测试类型，[计划A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}，然后定义入选者条件。 下面是如何确定哪封电子邮件入选。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## 入选者条件 {#winner-criteria}

1. 首先列出默认&#x200B;**[!UICONTROL Winner Criteria]**&#x200B;选项。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>[!UICONTROL Opens]</b></td>
   <td>当图像下载到电子邮件中时，打开注册表。 即使不包含图像，默认情况下Marketo也会在所有HTML电子邮件中插入一个跟踪像素。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Clicks]</b></td>
   <td>默认情况下，电子邮件中的链接嵌入了跟踪，使您能够查看点击哪个链接的人员、点击的链接总数等。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Click to Open] %</b></td>
   <td>已打开并在电子邮件中单击链接的电子邮件的百分比。 此方法测量电子邮件的相关性和上下文，方法是用唯一点击数除以唯一打开数，然后乘以100以百分比显示电子邮件。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Engagement Score]</b></td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">参与度分数</a>可帮助您确定内容的有效性。</td>
   </tr>
   </table>

   >[!TIP]
   >
   >如果您选择参与度分数，则该测试需要运行至少24小时。 详细了解[了解参与度分数](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}。

1. 您还可以通过选择&#x200B;**[!UICONTROL Custom Conversion]**&#x200B;并单击&#x200B;**[!UICONTROL Edit]**&#x200B;来自定义您的条件。

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >自定义转化允许您通过使用触发器和过滤器选择任何事件作为转化。

1. 随即会打开一个窗口。 找到您选择的触发器，并将其拖动到画布中。

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. 定义触发器。

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo仅允许从此电子邮件程序发送了电子邮件的用户使用触发器/过滤器，因此无需添加“已发送电子邮件”过滤器。 此外，在使用与电子邮件相关的触发器/过滤器时，请确保使用“is any”作为运算符。

1. 单击 **[!UICONTROL Close]**。

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   太棒了！ 现在是时候决定如何决定赢家了。

## 声明入选方 {#declare-winner}

1. 从两个可用选项中选择一个。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >如果您正在进行&#x200B;**日期/时间** A/B测试，则只能选择&#x200B;**[!UICONTROL Manual]**。

   A/B测试结束后，Marketo可以在计划的时间自动发送入选电子邮件，您也可以查看结果并决定何时发送出哪些电子邮件。

1. “自动”功能非常强大，而且是默认选项。 只需单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >选择&#x200B;**[!UICONTROL Manual]**&#x200B;将发送测试，并等待您声明入选者。 您会收到一份结果报告。

完美！ 现在，我们[安排A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}。
