---
unique-page-id: 10096681
description: 了解网络研讨会计划状态 — Marketo文档 — 产品文档
title: 了解网络研讨会计划状态
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 了解网络研讨会计划状态 {#understanding-webinar-program-statuses}

项目群状态表示人员作为事件成员所处理的不同事件状态。 它们与渠道类型相关联。 Marketo具有内置渠道类型，称为 **网络研讨会**. 状态既可用于批处理，也可用于触发营销活动。

人们以线性方式在项目状态中移动，而不会回到状态。 例如，状态为 **已参加** 无法移回 **已注册**.

以下是与网络研讨会渠道关联的计划状态的简短描述。

>[!TIP]
>
>要手动更新状态，请单击  **从网络研讨会提供商刷新** 在 **事件操作** 下拉菜单。

![](assets/image2015-12-17-13-3a52-3a39.png)

**不在计划中**  — 使用此状态可从事件中删除人员。

**已邀请**  — 使用此状态向事件添加人员。

**未决批准**  — 使用此状态可延迟向您的人员发送确认电子邮件。 请参阅中的“手动审批注册者” [ON24事件注册更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} 以了解更多信息。

**等待已列出**  — 使用此状态可让某些人等待，直到有额外的名额可用。

**被拒绝**  — 使用此状态可拒绝人员注册您的事件。

**已注册**  — 当您使用ON24集成时，此状态会将用户推送到ON24。 当ON24响应人员已成功注册时，人员的状态会更新。

**注册错误**  — 此状态表示用户在尝试注册事件时遇到错误。

>[!NOTE]
>
>如果发生注册错误，您可以通过查看项目群成员选项卡中的状态原因列获取该人员的附加信息。 修复错误后，您可以手动将用户的程序状态更改为Marketo中的已注册。

**已参加**  — 网络研讨会结束时，ON24会返回与会者名单。 此状态会自动提取到Marketo中。

**按需参加**  — 参加网络研讨会存档版本的人员将获得此状态。

**无节目**  — 网络研讨会结束后，在从ON24提取出席数据后，已注册但未出席的人员状态将更新为“不显示”。 使用ON24，可能需要30分钟到3小时的时间来准备最终出席信息并在Marketo中提供。

>[!NOTE]
>
>为了让Marketo能够提取不显示状态，人员必须已注册 *在Marketo中*. 我们无法捕获来自On24数据馈送的“否”节目。

>[!MORELIKETHIS]
>
>[了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
