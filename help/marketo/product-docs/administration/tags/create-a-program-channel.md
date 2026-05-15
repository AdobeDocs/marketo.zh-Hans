---
unique-page-id: 2950682
description: 创建项目渠道的步骤，其中包含状态和进展步骤，包括项目类型、成功状态和事件的移动设备签入选项。
title: 创建项目渠道
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
TQID: https://experienceleague.adobe.com/Ficlv7OfEScqLRVbOfc2hc-S3cQ2YjriiKWnbS1Op9A
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 390
ht-degree: 4%

---

# 创建项目渠道 {#create-a-program-channel}

项目是一项特定的营销计划。 渠道旨在作为投放机制，例如网络研讨会、赞助或在线广告。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>了解有关Marketo中最重要的元素[程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)的更多信息。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/create-a-program-channel-1.png)

1. 单击 **[!UICONTROL Tags]**。

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >为什么要添加标记？ 频道是描述节目的一种方式，与其他标记类似。 该渠道具有特殊的额外功能。

1. 单击[!UICONTROL Channel]旁边的&#x200B;**+**&#x200B;符号展开并查看现有渠道。

   ![](assets/create-a-program-channel-3.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;下，单击&#x200B;**[!UICONTROL New Channel]**。

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**示例**
   >
   >频道：公告牌
   >
   >* 应用到：默认
   >* 晋升：成员、参与（这些是适当的默认值）
   >* 成功：已参与
   >
   >渠道：参与方
   >
   >* 应用到：事件
   >* 进度：已邀请、已注册、无节目和已参加
   >* 成功：已参加
   >
   >查看现有渠道的进展情况，以获取有关如何使用这些渠道的指导。

1. 以参与方渠道为例，命名您的新&#x200B;**[!UICONTROL Channel]**&#x200B;并选择它将应用到的节目类型。

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >有几种类型的程序。 将渠道与正确的类型匹配。 如果不确定，请选择&#x200B;**[!UICONTROL Default]**。

   >[!NOTE]
   >
   >使用“[!UICONTROL Event with Webinar]”时，系统映射将被锁定（根据网络研讨会集成的要求）且无法编辑。

1. 输入前两个程序状态名称，然后单击&#x200B;**[!UICONTROL Add Step]**。

   ![](assets/create-a-program-channel-6.png)

1. 输入其他节目&#x200B;**[!UICONTROL Status]**&#x200B;和&#x200B;**[!UICONTROL Step]**&#x200B;编号，然后单击&#x200B;**[!UICONTROL Add Step]**。

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >**[!UICONTROL Step]**&#x200B;编号用于排序程序状态。 请注意，人们不能在这些进展步骤中后退。 它们只能将状态更改为更高或等值的状态。 当状态要来回切换而不是按级数切换时，请使用相等值。

1. 输入最后一个节目&#x200B;**[!UICONTROL Status]**&#x200B;和&#x200B;**[!UICONTROL Step]**&#x200B;编号。

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >使用类型“[!UICONTROL Event]”时，需要系统映射“已注册”、“轮候”和“已参加”状态。 因此，无法隐藏这些状态。

1. 为&#x200B;**[!UICONTROL Registered]**&#x200B;选择&#x200B;**[!UICONTROL Mobile Check-in Status]**。

   ![](assets/create-a-program-channel-9.png)

1. 为&#x200B;**[!UICONTROL Attended]**&#x200B;选择&#x200B;**[!UICONTROL Mobile Check-in Status]**。

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**[!UICONTROL Mobile Check-in Status]**&#x200B;选项仅在渠道适用于事件项目时才可用。

   >[!NOTE]
   >
   >只有拥有&#x200B;**[!UICONTROL Registered]**&#x200B;和&#x200B;**[!UICONTROL Attended]**&#x200B;的&#x200B;**[!UICONTROL Mobile Check-in Status]**&#x200B;的用户才能在[移动设备签入应用](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md)中可见。

   >[!TIP]
   >
   >如果在移动设备签入应用中创建了新人员，则事件程序中将它设置为[!UICONTROL Registered]。 如果某人已登记到应用程序上的事件，则事件程序中的该人将被设置为[!UICONTROL Attended]。

1. 选择&#x200B;**[!UICONTROL Success]**&#x200B;程序状态，然后单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/create-a-program-channel-11.png)

   当您制作该类型的新节目时，此新频道将是选项之一。
