---
title: priority-override-for-trigger-活动
description: 触发器活动的优先级覆盖
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# 触发器活动的优先级覆盖

<br> 

管理员可以覆盖Marketo确定的优先级，以触发活动来设置更符合业务目标的优先级。

>[!NOTE]
>
>此功能仅适用于触发活动和已被授予“编辑触发活动优先级”权限的用户。

>[!CAUTION]
>
>强烈建议您在有限的业务关键活动集上使用此功能（建议最大值为25）。 松散地在大型集合上使用该功能可能会对整体活动执行产生不利影响。

## 覆盖优先级

1. 在触发器活动下，单击&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL Override Priority]**。

   ![图像1](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. 从下拉菜单中选择新的优先级。 单击&#x200B;**[!UICONTROL Confirm]**。

   ![图像2](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![图3](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* 您可以在[!UICONTROL Marketing Activities]下的[!UICONTROL Campaign Queue]中视图活动的默认优先级。 要提高执行率，我们建议将活动优先级设置为比其默认优先级高一级。
>* 用户设置优先级仅适用于符合活动资格的新用户；已排队的人员不会受到影响。


## 重置优先级

1. 要将活动优先级重置回系统默认值，请转到触发活动中的&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL Reset Priority]**。

   ![图像4](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. 单击&#x200B;**[!UICONTROL Reset]**&#x200B;进行确认。

   ![图像5](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>优先级改写和重置在审核跟踪中捕获。 您可以在经典体验中通过[!UICONTROL Admin]区域视图[审核跟踪](https://docs.marketo.com/x/GZ2t)。

## 授予优先权覆盖访问权限

>[!CAUTION]
>
>只有具有管理员职责的管理员或用户才应具有活动优先权覆盖访问权限。

1. 在[!UICONTROL Admin]区域，单击&#x200B;**[!UICONTROL Users & Roles]**。

   ![图6](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. 单击&#x200B;**[!UICONTROL Roles]**&#x200B;选项卡，选择要授予访问权限的用户，然后单击&#x200B;**[!UICONTROL Edit Role]**。

   ![图像七](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. 在[!UICONTROL Access Marketing Activities]下，检查&#x200B;**[!UICONTROL Edit Trigger Campaign Priority]**。 单击&#x200B;**[!UICONTROL Save]**。

   ![图像8](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## 视图活动在营销中的优先地位

您可以通过单击触发器视图中的&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡，来活动[!DNL Classic]体验中的活动优先级。

![图像9](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>[!DNL Classic]体验中的优先级仅限视图。 更改或重置活动优先级只能通过Marketo Sky来使用。
