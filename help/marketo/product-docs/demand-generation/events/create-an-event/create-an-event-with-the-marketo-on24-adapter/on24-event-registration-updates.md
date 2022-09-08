---
unique-page-id: 10096683
description: ON24事件注册更新 — Marketo文档 — 产品文档
title: ON24事件注册更新
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# ON24事件注册更新 {#on-event-registration-updates}

>[!IMPORTANT]
>
>自2022年8月起，ON24不再支持新的Marketo集成。 本文中的信息仅适用于现有用户。

## 手动批准注册者 {#manually-approving-registrants}

您可以在向注册者发送确认电子邮件之前，手动批准他们。 为此，您需要配置营销活动以处理此额外步骤：

1. 对于注册触发器营销活动：

   * 在智能列表中，将触发器设置为 **填写表单**.
   * 在“流”中，将“进度”状态设置为 **待批准**.

1. 转到事件，然后单击 **成员** 选项卡。 此选项卡显示填写表单的所有人员。 其状态应设置为 **待批准**.
1. 使用网格顶部的过滤器仅查看状态为 **待批准**.
1. 选择要注册的人员（按住Shift键单击、按住Control键单击或选择全部）。
1. 在菜单中，单击 **更改状态**. 选择 **已注册**, **被拒绝**、或任何其他适用状态。

## 处理注册错误的人员 {#handling-people-with-a-registration-error}

如果某个人最终未注册，而是设置为“注册错误”状态，则恢复为正常时间不晚。

1. 从成员选项卡中，筛选状态为的人员列表 **注册错误**.
1. 在继续操作之前，请确保已确定并修复了集成问题（检查以确保下没有错误） **活动合作伙伴** 中)。
1. 问题解决后，选择“注册错误”状态的所有人员，并将其状态更改为 **已注册**. 这将尝试在ON24中再次注册它们。

## 从ON24更新成员状态 {#updating-member-status-from-on}

Marketo每天晚上大约11点自动提取出勤信息。 要手动更新考勤信息，请单击 **从网络研讨会提供商刷新** 在 **事件操作**.

>[!MORELIKETHIS]
>
>[了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
