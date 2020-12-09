---
title: 理解批触发智能活动
description: 了解批处理和触发智能活动
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# 了解批处理和触发智能活动

<br> 

智能活动有两种类型：批处理和触发器。

## 批智能活动

批活动在特定时间启动并同时影响特定人员集。 例如，向您数据库中居住在加利福尼亚的每个人发送电子邮件。

批量智能活动在智能列表部分中仅具有过滤器（即，没有触发器）。

![图像1](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

单击选 **[!UICONTROL Schedule]** 项卡将确认智能活动设置为“批”。

![图像2](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**批智能活动**

* 可以安排重复，如每日、每周和每月。 你也可以让他们只跑一次。
* 在项目计划 [视图上可见](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)。
* 智能活动中“等待”步骤后的任何内容都不会包括在视图中。

## 触发智能活动

触发智能活动根据触发事件一次影响一个人。 触发器的示例包括单击电子邮件中的链接。

如果智能活动在智能列表部分内使用至少一个触发器，则该模式将自动设置为触发。

![图3](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

单击选 **[!UICONTROL Schedule]** 项卡将确认智能活动设置为“触发器”。

![图像4](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**触发智能活动**

* 无法安排重复。 只能将它们设置为活动或非活动状态。
* 您可以设置多个触发器。 但是，如 _果触发_ 了任何触发器，将运行活动操作。

>[!TIP]
>
>使用 [活动日志](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) ，查看智能活动中的分步操作。 您可以在人员详细信息页面的最后一个选项卡中找到活动日志。
