---
unique-page-id: 10096683
description: ON24事件注册更新- Marketo Docs —— 产品文档
title: ON24事件注册更新
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# ON24事件注册更新 {#on-event-registration-updates}

## 手动批准注册者 {#manually-approving-registrants}

您可以在向注册者发送确认电子邮件之前手动批准他们。 为此，您需要配置活动以处理此额外步骤：

1. 对于注册触发器活动:

   * 在智能列表中，将触发器设置 **为填充表单**。
   * 在“流”中，将“进展状态”设置为“待 **批准”**。

1. 转到事件并单击“成 **员** ”选项卡。 此选项卡显示已填写表单的所有人员。 其状态应设置为“待 **批准”**。
1. 使用网格顶部的过滤器仅视图状态为“待批准” **的人员**。
1. 选择要注册的人员（按住Shift键单击、按住Ctrl键单击或选择全部）。
1. 在菜单中，单击“ **更改状态**”。 选择 **“已注册**”、 **“被拒绝**”或任何其他适用状态。

## 处理带有注册错误的人员 {#handling-people-with-a-registration-error}

如果某人最终未注册，而是设置为“注册错误”状态，则恢复还为时不晚。

1. 从“成员”选项卡中，过滤状态为“注册错误” **的人员的列表**。
1. 在继续操作之前，请确保您已确定并修复了集成问题(检查以确保“管理员”中的“事件合 **作伙伴** ”下没有错误)。
1. 问题解决后，选择“注册错误”状态的所有人员，并将其状态更改为“已注 **册”**。 这将尝试在ON24中重新注册它们。

## 从ON24更新成员状态 {#updating-member-status-from-on}

Marketo每天晚上大约11点自动收集出席信息。 要手动更新出席信息，请单击“ **事件操作”下的“从网络研讨** 会提供 **者刷新”**。

>[!MORELIKETHIS]
>
>* [了解ON24适配器的营销事件](understanding-marketo-on24-adapter-events.md)

>



