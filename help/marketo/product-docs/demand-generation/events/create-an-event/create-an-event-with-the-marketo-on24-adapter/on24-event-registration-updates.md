---
unique-page-id: 10096683
description: ON24事件注册更新 — Marketo文档 — 产品文档
title: ON24 事件注册更新
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 3%

---

# ON24 事件注册更新 {#on-event-registration-updates}

## 手动审批注册者 {#manually-approving-registrants}

您可以在向注册者发送确认电子邮件之前手动批准注册者。 要实现此目的，您需要配置营销活动以处理此附加步骤：

1. 对于注册触发器活动：

   * 在[!UICONTROL Smart List]中，将触发器设置为&#x200B;**[!UICONTROL Fills Out Form]**。
   * 在流中，将[!UICONTROL Status in Progression]设置为&#x200B;**[!UICONTROL Pending Approval]**。

1. 转到“事件”并单击&#x200B;**[!UICONTROL Members]**&#x200B;选项卡。 此选项卡显示填写了表单的所有人员。 它们的状态应设置为&#x200B;**[!UICONTROL Pending Approval]**。
1. 使用网格顶部的筛选器仅查看状态为&#x200B;**[!UICONTROL Pending Approval]**&#x200B;的人员。
1. 选择要注册的人员（按住Shift并单击、按住Control并单击或全选）。
1. 从菜单中，单击&#x200B;**[!UICONTROL Change Status]**。 选择&#x200B;**[!UICONTROL Registered]**、**[!UICONTROL Rejected]**&#x200B;或任何其他适用的状态。

## 处理出现注册错误的人员 {#handling-people-with-a-registration-error}

如果人员最终未注册，而是设置为状态[!UICONTROL Registration Error]，则进行恢复还为时未晚。

1. 从[!UICONTROL Members]选项卡中，筛选状态为&#x200B;**[!UICONTROL Registration Error]**&#x200B;的人员列表。
1. 在继续之前，请确保您已确定并修复了集成问题（请检查以确保“管理员”中的&#x200B;**[!UICONTROL Event Partners]**&#x200B;下没有错误）。
1. 问题解决后，选择所有状态为[!UICONTROL Registration Error]的人员，并将其状态更改为&#x200B;**[!UICONTROL Registered]**。 这将尝试在ON24中再次注册它们。

## 从ON24更新成员状态 {#updating-member-status-from-on}

Marketo每晚在太平洋时间晚上11点左右自动提取出席信息。 要手动更新出席信息，请单击&#x200B;**[!UICONTROL Refresh from Webinar Provider]**&#x200B;下的&#x200B;**[!UICONTROL Event Actions]**。

>[!MORELIKETHIS]
>
>[了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
