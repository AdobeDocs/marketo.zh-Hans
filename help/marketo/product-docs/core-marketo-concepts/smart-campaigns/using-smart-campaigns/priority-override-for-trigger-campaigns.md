---
description: 触发器活动的优先级覆盖 — Marketo文档 — 产品文档
title: 触发器活动的优先级覆盖
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 触发器活动的优先级覆盖 {#priority-override-for-trigger-campaigns}

管理员可以覆盖Marketo Engage为触发营销活动确定的优先级，以设置更好地与业务目标一致的优先级。

>[!NOTE]
>
>此功能仅适用于触发器营销活动和已获得[“编辑触发器营销活动优先级”权限](#grant-priority-override-access)的用户。

>[!CAUTION]
>
>强烈建议您仅在有限的一组业务关键型营销活动上使用此功能（建议的最大值为25）。 在大型集上松散使用该功能可能会对整体营销活动执行产生不利影响。

## 授予优先级覆盖访问权限 {#grant-priority-override-access}

>[!NOTE]
>
>只有管理员或具有管理员责任的用户才应具有营销活动优先级覆盖访问权限。

1. 在[!UICONTROL 管理员]区域中，单击&#x200B;**[!UICONTROL 用户和角色]**。

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. 单击&#x200B;**[!UICONTROL 角色]**&#x200B;选项卡，选择要授予其访问权限的用户，然后单击&#x200B;**[!UICONTROL 编辑角色]**。

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. 在[!UICONTROL 访问营销活动]下，选择&#x200B;**[!UICONTROL 编辑触发器促销活动优先级]**。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## 覆盖优先级 {#override-priority}

1. 找到您的触发器促销活动。 右键单击并选择&#x200B;**[!UICONTROL 覆盖营销活动优先级]**。

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. 单击要启用的&#x200B;**[!UICONTROL 覆盖促销活动优先级]**&#x200B;滑块。 选择新的优先级并单击&#x200B;**[!UICONTROL 确认]**。

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   新的优先级将显示在“计划”选项卡中。

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* 您可以在[!UICONTROL 营销活动]下的[!UICONTROL 营销活动队列]中查看营销活动的默认优先级。 为了提高执行率，我们建议将营销活动优先级设置为比默认优先级高一个级别。
>* 用户集优先级仅适用于符合营销活动条件的新用户；已排队的用户不会受到影响。
>* 已在[审核记录](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md){target="_blank"}中捕获优先级覆盖。
