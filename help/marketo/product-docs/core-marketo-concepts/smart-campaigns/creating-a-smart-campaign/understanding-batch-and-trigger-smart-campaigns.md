---
unique-page-id: 2953132
description: 了解批处理和触发智能活动- Marketo Docs —— 产品文档
title: 了解批处理和触发智能活动
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---


# 了解批处理和触发智能活动 {#understanding-batch-and-trigger-smart-campaigns}

智能活动有两种类型：批处理和触发器。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 批智能活动 {#batch-smart-campaign}

>[!NOTE]
>
>**定义**
>
>批活动在特定时间启动并同时影响特定人员集。 例如，向加利福尼亚的所有人发送电子邮件。

批量智能活动在智能列表部分中仅具有过滤器（即，没有触发器）。

![](assets/batch-filter.png)

单击 **计划** 选项卡将确认智能活动设置为“批处理”。

![](assets/batch-c4.png)

**批智能活动**

* 可以安排重复，如每日、每周和每月。 你也可以让他们只跑一次。
* 在项目计划 [视图上可见](../../../../product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md)。\
   *请注意，智能活动中“等待”步骤后的任何内容都不会包括在视图中。

<br> 

## 触发智能活动 {#trigger-smart-campaign}

>[!NOTE]
>
>**定义**
>
>触发智能活动根据触发事件一次影响一个人。 触发器的示例包括单击电子邮件中的链接。

如果智能活动在智能列表部分内使用至少一个触发器，则该模式将自动设置为触发。

![](assets/trigger.png)

单击 **计划** 选项卡将确认智能活动设置为“已触发”。

![](assets/trigger2.png)

**触发智能活动**

* 无法安排重复。 只能将它们设置为活动或非活动状态。
* 您可以设置多个触发器。 但是，如果触发了任何触发器，则将运行活动操作。

## 观看有关创建触发式电子邮件活动的视频 {#watch-a-video-on-creating-triggered-email-campaigns}

`<iframe width="630" height="470" src="//play.vidyard.com/6zNazwTgt2LNeCjPAt3W9K.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

>[!TIP]
>
>使用 [活动日志](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) ，查看智能活动中的分步操作。 您可以在人员详细信息页面的最后一个选项卡中找到活动日志。

