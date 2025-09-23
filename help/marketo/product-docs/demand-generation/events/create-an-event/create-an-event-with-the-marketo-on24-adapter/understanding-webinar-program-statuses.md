---
unique-page-id: 10096681
description: 了解网络研讨会计划状态 — Marketo文档 — 产品文档
title: 了解网络研讨会项目状态
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# 了解网络研讨会项目状态 {#understanding-webinar-program-statuses}

项目群状态表示人员作为事件成员所处理的不同事件状态。 它们与渠道类型相关联。 Marketo具有名为&#x200B;**网络研讨会**&#x200B;的内置渠道类型。 状态既可用于批处理，也可用于触发营销活动。

人们以线性方式在项目状态中移动，而不会回到状态。 例如，状态为&#x200B;**已参加**&#x200B;的人员无法移回&#x200B;**已注册**。

以下是与网络研讨会渠道关联的计划状态的简短描述。

>[!TIP]
>
>要手动更新状态，请在&#x200B;**事件操作**&#x200B;下拉列表中单击&#x200B;**网络研讨会提供程序**&#x200B;中的“刷新”。

![](assets/image2015-12-17-13-3a52-3a39.png)

**不在程序**&#x200B;中 — 使用此状态从事件中删除人员。

**已邀请** — 使用此状态向活动添加联系人。

**未决批准** — 使用此状态可延迟向您的联系人发送确认电子邮件。 有关详细信息，请参阅[ON24事件注册更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}中的“手动批准注册者”。

**等待已列出** — 使用此状态可让某些人等待，直到有更多的名额可用。

**已拒绝** — 使用此状态可拒绝人员注册您的事件。

**已注册** — 使用ON24集成时，此状态会将用户推送到ON24。 当ON24响应人员已成功注册时，人员的状态会更新。

**注册错误** — 此状态反映用户尝试注册事件时遇到错误。

>[!NOTE]
>
>如果发生注册错误，您可以通过查看项目群成员选项卡中的状态原因列获取该人员的附加信息。 修复错误后，您可以手动将用户的程序状态更改为Marketo中的已注册。

**已参加** — 在网络研讨会结束时，ON24会返回已参加的人员列表。 此状态会自动提取到Marketo中。

**按需参加** — 参加已存档的网络研讨会版本的用户将收到此状态。

**无节目** — 网络研讨会结束时，在从ON24提取出席率数据后，已注册但未出席的人员状态将更新为“无节目”。 使用ON24，可能需要30分钟到3小时的时间来准备最终出席信息并在Marketo中提供。

>[!NOTE]
>
>为了使Marketo能够提取“不显示”状态，用户必须在Marketo *中注册*。 我们无法捕获来自On24数据馈送的“否”节目。

>[!MORELIKETHIS]
>
>[了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
