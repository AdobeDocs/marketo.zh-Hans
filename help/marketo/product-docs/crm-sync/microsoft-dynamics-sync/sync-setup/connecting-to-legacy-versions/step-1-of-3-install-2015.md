---
unique-page-id: 7504736
description: 安装Marketo for Microsoft Dynamics 2015本地步骤1/3 - Marketo文档 — 产品文档
title: 安装Marketo for Microsoft Dynamics 2015本地步骤1/3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# 第1步（共3步）：为Marketo配置同步用户（2015年内部部署） {#step-of-configure-sync-user-for-marketo-on-premises-2015}

在将Microsoft Dynamics 2015内部部署与Marketo Engage同步之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，无法将新的CRM同步到现有的Marketo实例。

>[!PREREQUISITES]
>
>如果您使用的是Microsoft Dynamics On-Premise，则必须具有 [面向互联网的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 已配置2.0+ (ADFS)。 注意：单击该链接时，会自动下载IFD文档。
>
>[下载Marketo商机管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} 开始之前。

>[!NOTE]
>
>**需要Dynamics管理员权限**.
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到Dynamics。 单击 **[!UICONTROL Microsoft Dynamics CRM]** 下拉菜单并选择 **[!UICONTROL 设置]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. 下 **[!UICONTROL 设置]**，选择 **[!UICONTROL 解决方案]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. 单击 **[!UICONTROL 导入]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. 单击 **[!UICONTROL 浏览]** 并选择您的解决方案 [已下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2015-3-19-9-20-56.png)

1. 查看解决方案信息并单击 **[!UICONTROL 查看解决方案包详细信息]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. 检查完所有详细信息后，单击 **[!UICONTROL 关闭]**.

   ![](assets/step6.png)

1. 返回“解决方案信息”页面，单击 **[!UICONTROL 下一个]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. 确保选中SDK选项复选框。 单击 **[!UICONTROL 导入]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待导入完成。

   >[!TIP]
   >
   >您需要启用浏览器上的弹出窗口才能完成安装过程。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下载日志文件（如果需要），然后单击 **[!UICONTROL 关闭]**.

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，但有警告”。 这是完全符合预期的。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management现在将显示在 **[!UICONTROL 所有解决方案]** 页面。

   ![](assets/image2015-3-19-8-40-38.png)

1. 选择Marketo解决方案，然后单击 **[!UICONTROL 发布所有自定义项]**.

   ![](assets/image2015-3-19-8-41-21.png)

   做得不错！安装完成。

   >[!CAUTION]
   >
   >禁用任何Marketo SDK消息传递过程都将导致安装中断！

   >[!MORELIKETHIS]
   >
   >[安装Marketo for Microsoft Dynamics 2015本地步骤2（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md){target="_blank"}
