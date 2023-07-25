---
description: 触发器促销活动的优先级覆盖 — Marketo文档 — 产品文档
title: 触发器营销活动的优先级覆盖
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 触发器营销活动的优先级覆盖 {#priority-override-for-trigger-campaigns}

管理员可以覆盖Marketo确定的触发营销活动的优先级，以设置更好地与业务目标保持一致的优先级。

>[!NOTE]
>
>此功能仅适用于触发器营销活动和已获得授权的用户 [“编辑触发器促销活动优先级”权限](#grant-priority-override-access).

>[!CAUTION]
>
>强烈建议您在有限的一组业务关键型营销活动上使用此功能（建议的最大值为25）。 在大型集上松散使用该功能可能会对整体营销活动执行产生负面影响。

## 授予优先级覆盖访问权限 {#grant-priority-override-access}

>[!NOTE]
>
>只有管理员或负有管理员责任的用户才应具有营销活动优先级覆盖访问权限。

1. 在 [!UICONTROL 管理员] 区域，单击 **[!UICONTROL 用户和角色]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. 单击 **[!UICONTROL 角色]** 选项卡，选择要向其授予访问权限的用户，然后单击 **[!UICONTROL 编辑角色]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. 下 [!UICONTROL 访问营销活动]，选择 **[!UICONTROL 编辑触发器营销活动优先级]**. 单击 **[!UICONTROL 保存]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## 覆盖优先级 {#override-priority}

1. 找到您的触发器营销活动。 右键单击并选择 **[!UICONTROL 覆盖营销活动优先级]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. 单击 **[!UICONTROL 覆盖营销活动优先级]** 要启用的滑块。 选择新的优先级并单击 **[!UICONTROL 确认]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   新的优先级将显示在“计划”选项卡中。

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* 您可以在以下位置查看营销活动的默认优先级： [!UICONTROL 营销活动队列] 下 [!UICONTROL 营销活动]. 为了提高执行率，我们建议将营销活动优先级设置为比默认优先级高一个级别。
>* 用户设置优先级仅适用于符合营销活动条件的新用户；已排队的用户不会受到影响。
>* 优先级覆盖捕获于 [审核记录](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md).
