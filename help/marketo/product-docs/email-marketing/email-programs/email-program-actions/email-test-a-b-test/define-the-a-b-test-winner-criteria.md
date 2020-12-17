---
unique-page-id: 2359545
description: 定义A/B测试优胜者标准- Marketo Docs —— 产品文档
title: 定义A/B测试入选方标准
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# 定义A/B测试入选方标准{#define-the-a-b-test-winner-criteria}

当[将A/B测试](add-an-a-b-test.md)添加到电子邮件项目时，您需要选择测试类型[计划A/B测试](schedule-the-a-b-test.md)，然后定义入选方标准。 下面将介绍如何确定哪封电子邮件最终胜出。

>[!PREREQUISITES]
>
>* [添加A/B测试](add-an-a-b-test.md)

>



## 入选方标准{#winner-criteria}

1. 首先列出默认的&#x200B;**入选方标准**&#x200B;选项。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **打开** | 当图像下载到电子邮件中时，打开会注册。 即使您不包含图像，默认情况下Marketo也会在所有HTML电子邮件中插入单个跟踪像素。 |
   |---|---|
   | **点击** | 默认情况下，电子邮件中的链接会跟踪其中嵌入的链接，这样您就可以查看谁点击了哪个链接，点击了多少个总链接，等等。 |
   | **单击以打开%** | 已打开并在电子邮件中单击链接的电子邮件百分比。 这通过采用唯一点击次数除以唯一打开次数，再乘以100将其显示为百分比，来衡量电子邮件的相关性和上下文。 |
   | **参与分数** | [参与分数](http://docs.marketo.com/display/DOCS/Understanding+the+Engagement+Score)可帮助您确定内容的有效性。 |

   >[!TIP]
   >
   >如果您选择“参与得分”，则测试至少需要运行24小时。 了解有关[了解参与情况得分](../../../../../product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md)的更多信息。

   您还可以通过选择“自定义转换”并单击“编辑”来自定义条件。
   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >“自定义转换”允许您使用触发器和事件来选择任何过滤器作为转换。

   窗子会打开。 找到您选择的触发器并将其拖入画布。
   ![](assets/image2014-9-12-15-3a52-3a18.png)

   >[!NOTE]
   >
   >**深潜**
   >
   >
   >进一步了解[智能列表和静态列表](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)。

   定义触发器。
   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo将仅允许从此电子邮件项目发送电子邮件的人员使用触发器。 无需添加“已发送电子邮件”过滤器。

   单击关闭。
   ![](assets/image2014-9-12-15-3a53-3a36.png)

   太好了！ 现在是时候决定胜者的决定了。

## 声明入选方{#declare-winner}

1. 从两个可用选项中选择一个。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >如果您正在进行&#x200B;**日期／时间** A/B测试，则只能选择&#x200B;**手动**。

   A/B测试结束后，Marketo可以在计划的时间自动发送入选方电子邮件，您也可以查看结果并决定何时发出哪封电子邮件。

1. “自动”是超棒的，是默认选项。 只需单击&#x200B;**Next**。

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >选择&#x200B;**手动**&#x200B;将发出测试并等待您声明入选方。 您将收到结果报告。

   [计划A/B测试](schedule-the-a-b-test.md)

完美！ 现在，让我们。.