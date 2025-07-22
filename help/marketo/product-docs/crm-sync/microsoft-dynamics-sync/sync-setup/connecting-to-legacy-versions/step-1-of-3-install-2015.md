---
unique-page-id: 7504736
description: 安装适用于Microsoft Dynamics 2015的Marketo本地步骤1/3 - Marketo文档 — 产品文档
title: 安装适用于Microsoft Dynamics 2015的Marketo本地步骤1/3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 1%

---

# 第1步（共3步）：为Marketo配置同步用户（2015年内部部署） {#step-of-configure-sync-user-for-marketo-on-premises-2015}

在与Marketo同步[!DNL Microsoft Dynamics] 2015年内部部署之前，您需要先在[!DNL Dynamics]中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，无法将新的CRM同步到现有的Marketo实例。

>[!PREREQUISITES]
>
>如果您正在使用[!DNL Microsoft Dynamics]内部部署，则必须配置[面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)和[Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS)。 注意：单击该链接时，会自动下载IFD文档。
>
>在开始之前[下载Marketo潜在客户管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。

>[!NOTE]
>
>**需要Dynamics管理员权限**。
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到&#x200B;**[!DNL Dynamics]。**&#x200B;单击&#x200B;**[!UICONTROL Microsoft Dynamics CRM]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2015-3-19-8-33-29.png)

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;下，选择&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/image2015-3-19-8-33-3.png)

1. 单击 **[!UICONTROL Import]**。

   ![](assets/image2015-3-19-8-34-8.png)

1. 单击&#x200B;**[!UICONTROL Browse]**&#x200B;并选择您[下载的解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 单击 **[!UICONTROL Next]**。

   ![](assets/image2015-3-19-9-20-56.png)

1. 查看[!UICONTROL Solution Information]并单击&#x200B;**[!UICONTROL View solution package details]**。

   ![](assets/image2015-11-18-11-12-8.png)

1. 检查完所有详细信息后，单击&#x200B;**[!UICONTROL Close]**。

   ![](assets/step6.png)

1. 返回[!UICONTROL Solution Information]页面，单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2015-3-19-9-21-50.png)

1. 确保选中SDK选项复选框。 单击 **[!UICONTROL Import]**。

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待导入完成。

   >[!TIP]
   >
   >您需要启用浏览器上的弹出窗口才能完成安装过程。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下载日志文件（如果需要），然后单击&#x200B;**[!UICONTROL Close]**。

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，但有警告”。 这是完全符合预期的。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo潜在客户管理现在将显示在&#x200B;**[!UICONTROL All Solutions]**&#x200B;页面上。

   ![](assets/image2015-3-19-8-40-38.png)

1. 选择Marketo解决方案并单击&#x200B;**[!UICONTROL Publish All Customizations]**。

   ![](assets/image2015-3-19-8-41-21.png)

   做得不错！安装完成。

   >[!CAUTION]
   >
   >禁用任何Marketo SDK消息传递过程都将导致安装中断！

   >[!MORELIKETHIS]
   >
   >[为 [!DNL Microsoft Dynamics] 2015年内部部署安装Marketo第2步（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)
