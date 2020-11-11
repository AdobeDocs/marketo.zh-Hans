---
title: priority-override-for-trigger-活动
description: 触发器活动的优先级覆盖
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '320'
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

1. 在触发器活动中，单击 [!UICONTROL **计划**] 选项卡，然后单 [!UICONTROL **击覆盖优先级**]。

   ![图像1](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. 从下拉菜单中选择新的优先级。 单击 [!UICONTROL **确认**]。

   ![图像2](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![图3](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* 您可以在下方视图活动的默认优先 [!UICONTROL Campaign Queue] 级 [!UICONTROL Marketing Activities]。 要提高执行率，我们建议将活动优先级设置为比其默认优先级高一级。
>* 用户设置优先级仅适用于符合活动资格的新用户；已排队的人员不会受到影响。


## 重置优先级

1. 要将活动优先级重置回系统默认值，请转到触 [!UICONTROL **发活动**] 中的计划选项卡，然后单 [!UICONTROL **击重置优先级**]。

   ![图像4](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. 单击 [!UICONTROL **重置**] ，以进行确认。

   ![图像5](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>优先级改写和重置在审核跟踪中捕获。 您可以在经 [典体验中](https://docs.marketo.com/x/GZ2t) ，通 [!UICONTROL Admin] 过区域视图审核跟踪。

## 授予优先权覆盖访问权限

>[!CAUTION]
>
>只有具有管理员职责的管理员或用户才应具有活动优先权覆盖访问权限。

1. 在区域 [!UICONTROL Admin] 中，单击“用 [!UICONTROL **户和角色”**]。

   ![图6](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. 单击“ [!UICONTROL **角色**] ”选项卡，选择要授予访问权限的用户，然后单击“编 [!UICONTROL **辑角色”**]。

   ![图像七](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. 在“编 [!UICONTROL Access Marketing Activities]辑触发 [!UICONTROL **器优先级”下选中**]。 单击 [!UICONTROL **保存**]。

   ![图像8](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## 视图活动在营销中的优先地位

您可以通过单击触发视图中 [!DNL Classic] 的计划选项卡 [!UICONTROL **来活动**] 体验中的活动优先级。

![图像9](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>体验的优先 [!DNL Classic] 级是仅视图。 更改或重置活动优先级只能通过Marketo Sky来使用。
