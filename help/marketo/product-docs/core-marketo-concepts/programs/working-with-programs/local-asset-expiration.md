---
description: 本地资产过期 — Marketo文档 — 产品文档
title: 本地资产到期
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 本地资产到期 {#local-asset-expiration}

设置过期日期/时间以取消发布登陆页面、取消激活触发器活动或停止循环的批量活动。

## 授予计划资产过期权限 {#grant-schedule-asset-expiration-permission}

在安排资源到期之前，您的Marketo角色必须启用适当的权限。

>[!NOTE]
>
>**需要管理员权限**

1. 在[!UICONTROL 管理员]区域中，单击&#x200B;**[!UICONTROL 用户和角色]**。

   ![](assets/local-asset-expiration-1.png)

1. 单击&#x200B;**[!UICONTROL 角色]**&#x200B;选项卡，选择要授予其访问权限的用户，然后单击&#x200B;**[!UICONTROL 编辑角色]**。

   ![](assets/local-asset-expiration-2.png)

1. 在[!UICONTROL 访问营销活动]下，选择&#x200B;**[!UICONTROL 计划本地资产过期]**，然后单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/local-asset-expiration-3.png)

## 设置到期日期 {#set-an-expiration-date}

1. 右键单击所需的程序，然后选择&#x200B;**[!UICONTROL 设置本地资产过期]**。

   ![](assets/local-asset-expiration-4.png)

1. 选中要为其设置到期日期的资源，然后单击&#x200B;**[!UICONTROL 设置到期日期]**。

   ![](assets/local-asset-expiration-5.png)

1. 选择到期日期。

   ![](assets/local-asset-expiration-6.png)

1. 设置时间。 您必须计划一个至少为将来15分钟的时间（不要忘记输入上午/下午）。 完成后单击&#x200B;**[!UICONTROL 确认]**。

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* 要编辑现有过期日期，只需检查资产并单击&#x200B;**[!UICONTROL 设置过期日期]**&#x200B;即可。
>* 资产过期后，将不再显示在过期网格中。 网格将仅显示已发布的登陆页面、活动的触发营销活动和循环的批处理营销活动。
>* 如果将资产移至其他项目，则将删除计划的过期日期。

## 删除到期日期 {#remove-an-expiration-date}

1. 要删除过期日期，请检查资产并单击&#x200B;**[!UICONTROL 删除过期日期]**。

   ![](assets/local-asset-expiration-8.png)

1. 查看受影响的资源，然后单击&#x200B;**[!UICONTROL 确认]**。

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>不能删除未来15分钟内的过期日期。 要“删除”过期时间，您需要等待资源过期，然后重新批准或激活该资源。
