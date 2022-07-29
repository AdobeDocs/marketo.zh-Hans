---
unique-page-id: 2359545
description: 定义A/B测试入选者标准 — Marketo文档 — 产品文档
title: 定义A/B测试入选者标准
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
source-git-commit: 67ae4605d541a475b42a5094a5588c469a9d975d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 定义A/B测试入选者标准 {#define-the-a-b-test-winner-criteria}

When [添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;}添加到您的电子邮件程序，您需要选择测试类型， [计划A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}，然后定义入选者标准。 下面是如何决定哪封电子邮件会成功。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;}

## 入选者标准 {#winner-criteria}

1. 默认 **入选者标准** 选项列在首位。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>打开</b></td>
   <td>打开会在将图像下载到电子邮件中时进行注册。 即使您不包含图像，默认情况下，Marketo也会在所有HTML电子邮件中插入单个跟踪像素。</td>
   </tr>
   <tr>
   <td><b>点击次数</b></td>
   <td>默认情况下，电子邮件中的链接中嵌入了跟踪，以便您查看点击了哪个链接的用户、点击了总链接的数量等。</td>
   </tr>
   <tr>
   <td><b>单击以打开%</b></td>
   <td>已打开并在电子邮件中点击链接的电子邮件的百分比。 这通过采用唯一点击次数除以唯一打开次数，然后乘以100将其显示为百分比来衡量电子邮件的相关性和上下文。</td>
   </tr>
   <tr>
   <td><b>参与度分数</b></td>
   <td>的 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">参与度分数</a> 可帮助您确定内容的有效性。</td>
   </tr>
   </table>

   >[!TIP]
   >
   >如果您选择了“参与度得分”，则测试需要至少运行24小时。 详细了解 [了解参与度分数](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target=&quot;_blank&quot;}。

1. 您还可以通过选择自定义转化并单击编辑来自定义您的标准。

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >自定义转化允许您使用触发器和过滤器选择任何事件作为转化。

1. 随即会打开一个窗口。 查找您选择的触发器，并将其拖到画布中。

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. 定义触发器。

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo仅允许通过此电子邮件程序发送电子邮件的人员使用触发器/过滤器，因此无需添加“已发送电子邮件”过滤器。 此外，在使用与电子邮件相关的触发器/过滤器时，请确保使用“is any”作为运算符。

1. 单击 **关闭**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   太棒了！ 现在该决定如何确定入选者了。

## 声明入选者 {#declare-winner}

1. 从两个可用选项中选取一个。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >如果您正在执行 **日期/时间** A/B测试，您只能选择 **手动**.

   A/B测试结束后，Marketo可以在计划时间自动发送入选电子邮件，也可以查看结果并决定何时发出哪封电子邮件。

1. 自动化功能非常棒，是默认选项。 只需单击 **下一个**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >选择 **手动** 将发出测试并等待您声明入选者。 您将收到结果报告。

完美！ 现在，让我们 [计划A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}。
