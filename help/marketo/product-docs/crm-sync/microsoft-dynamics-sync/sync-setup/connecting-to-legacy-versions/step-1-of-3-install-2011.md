---
unique-page-id: 3571805
description: 第1步（共3步） — 安装Marketo解决方案（2011年内部部署） — Marketo文档 — 产品文档
title: 步骤1/3 — 安装Marketo解决方案（2011年内部部署）
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 6%

---

# 第 1 步（共 3 步）：安装 Marketo 解决方案（2011 本地部署） {#step-of-install-the-marketo-solution-on-premises}

在同步[!DNL Microsoft Dynamics]内部部署和Marketo之前，您需要先在[!DNL Dynamics]中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，如果不替换该实例，则无法执行新的同步。

>[!PREREQUISITES]
>
>必须配置了[Active Directory联合身份验证服务](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} 2.0、2.1或3.0 (ADFS)的[面向Internet的部署](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (IFD)。 **注意**：单击链接时，IFD文档会自动下载。
>
>在开始之前[下载Marketo潜在客户管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。

>[!NOTE]
>
>需要&#x200B;**[!DNL Dynamics]管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到&#x200B;**[!DNL Dynamics]**，在左下角菜单中选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 在树中选择&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 单击 **[!UICONTROL Import]**。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 单击&#x200B;**[!UICONTROL Browse]**。 选择您[下载的Marketo潜在客户管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 单击 **[!UICONTROL Next]**。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 查看解决方案信息并单击&#x200B;**[!UICONTROL View solution package details]**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击&#x200B;**[!UICONTROL Close]**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页面，单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 确保选中SDK消息选项复选框。 单击 **[!UICONTROL Next]**。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您需要启用浏览器上的弹出窗口才能完成安装过程。

1. 现在等待导入完成。 起床做些伸展运动。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 单击 **[!UICONTROL Close]**。

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，但有警告”。 这是完全符合预期的。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. [!UICONTROL Marketo Lead Management]现在将显示在&#x200B;**[!UICONTROL All Solutions]**&#x200B;页面上。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 选择 [!UICONTROL Marketo Lead Management] 并点击 **[!UICONTROL Publish All Customizations]**。

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>禁用任何Marketo SDK消息传递过程都将导致安装中断！

>[!MORELIKETHIS]
>
>[第2步（共3步）：在 [!DNL Dynamics] 中设置Marketo同步用户（2011年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)
