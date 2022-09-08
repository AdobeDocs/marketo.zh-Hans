---
unique-page-id: 10096681
description: 了解网络研讨会计划状态 — Marketo文档 — 产品文档
title: 了解网络研讨会计划状态
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# 了解网络研讨会计划状态 {#understanding-webinar-program-statuses}

>[!IMPORTANT]
>
>自2022年8月起，ON24不再支持新的Marketo集成。 本文中的信息仅适用于现有用户。

程序状态表示人员作为事件成员进行的不同事件状态。 它们与渠道类型关联。 Marketo具有一个名为 **网络研讨会**. 状态可用于批处理和触发营销活动。

人们以线性方式浏览程序状态，并且不会返回状态。 例如，状态为 **已出席** 不能回到 **已注册**.

以下是与网络研讨会渠道关联的项目状态的简要描述。

>[!TIP]
>
>要手动更新状态，请单击  **从网络研讨会提供商刷新** 在 **事件操作** 下拉菜单。

![](assets/image2015-12-17-13-3a52-3a39.png)

**不在程序中**  — 使用此状态可从事件中删除人员。

**受邀**  — 使用此状态可向事件添加人员。

**待批准**  — 使用此状态可延迟向人员发送确认电子邮件。 请参阅 [ON24事件注册更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md) 以了解更多信息。

**已列出等待**  — 使用此状态让一些人等待更多座位。

**被拒绝**  — 使用此状态可拒绝人员注册您的事件。

**已注册**  — 当您使用ON24集成时，此状态会将用户推送到ON24。 当ON24响应该人员已成功注册时，该人员的状态会更新。

**注册错误**  — 此状态反映用户在尝试注册事件时遇到错误。

>[!NOTE]
>
>如果发生注册错误，您可以通过查看项目“成员”选项卡中的“状态原因”列来获取该人的其他信息。 修复错误后，您可以手动将用户的程序状态更改为在Marketo中已注册。

**已出席**  — 网络研讨会结束时，ON24返回了参加者的列表。 此状态会自动提取到Marketo中。

**已按需出席**  — 参加网络研讨会的存档版本的人员将收到此状态。

**无显示**  — 在网络研讨会结束时，在从ON24中提取出席数据后，注册但未参加的人员的状态将更新为“无显示”。 ON24可能需要30分钟到3小时的时间来准备最终的出席信息，并在Marketo中提供。

>[!NOTE]
>
>要使Marketo获取“无显示”状态，必须已注册人员 *在Marketo*. 无法捕获来自On24数据馈送的“无”显示。

>[!MORELIKETHIS]
>
>[了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
