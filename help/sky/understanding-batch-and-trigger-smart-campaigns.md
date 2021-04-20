---
title: 理解批处理和触发智能活动
description: 了解批处理和触发智能活动
exl-id: 54f38ecc-1b4c-4944-9f42-d8c1190c99d0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 了解批处理和触发智能活动

<br> 

智能活动有两种：批处理和触发器。

## 批量智能活动

批活动在特定时间启动并同时影响特定的一组人员。 例如，向您数据库中居住在加利福尼亚州的每个人发送电子邮件。

批量智能活动在智能列表部分中仅具有过滤器（即，没有触发器）。

![图像1](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

单击&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡将确认智能活动设置为“Batch”。

![图2](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**批智能活动**

* 可以安排重复使用，如每日、每周和每月。 你也可以让他们只跑一次。
* 在[项目计划视图](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)上可见。
* 智能活动中“等待”步骤后的任何内容都不会包含在视图中。

## 触发智能活动

触发智能活动根据触发的事件一次影响一个人。 触发器的示例包括单击电子邮件中的链接。

如果智能活动在智能列表部分内使用至少一个触发器，则模式将自动设置为触发。

![图3](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

单击&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡将确认智能活动设置为“触发器”。

![图4](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**触发智能活动**

* 无法为递归安排时间。 只能将它们设置为活动或非活动。
* 可以设置多个触发器。 但是，如果触发&#x200B;_任何_&#x200B;触发器，则将运行活动操作。

>[!TIP]
>
>使用[活动日志](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person)查看智能活动中发生的分步操作。 您可以在人员详细信息页面的最后一个选项卡中找到活动日志。
