---
description: 安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署1/3 - Marketo文档 — 产品文档
title: 安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署步骤1/3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# 步骤1/3：为Marketo配置同步用户（2016内部部署/Dynamics 365内部部署） {#step-of-configure-sync-user-for-marketo-on-premises-2016}

在将Microsoft Dynamics 2016内部部署/Dynamics 365与Marketo同步之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，无法将新的CRM同步到现有Marketo实例。

>[!PREREQUISITES]
>
>如果您使用的是Microsoft Dynamics On-Premise，则必须具有 [面向互联网的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)替换为 [Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS)已配置。 注意：单击该链接时，会自动下载IFD文档。
>
>[下载Marketo潜在客户管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 开始之前。

>[!NOTE]
>
>**需要Dynamics管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录 **动态。** 单击 **Microsoft Dynamics CRM** 下拉菜单并选择 **设置**.

   ![](assets/image2015-3-19-8-33-29.png)

1. 下 **设置**，选择 **解决方案**.

   ![](assets/image2015-3-19-8-33-3.png)

1. 单击 **导入**.

   ![](assets/image2015-3-19-8-34-8.png)

1. 单击 **浏览** 并选择您的解决方案 [已下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 单击 **下一个**.

   ![](assets/image2015-3-19-9-20-56.png)

1. 查看解决方案信息并单击 **查看解决方案包详细信息**.

   ![](assets/image2015-11-18-11-12-8.png)

1. 检查完所有详细信息后，单击 **关闭**.

   ![](assets/step6.png)

1. 返回“解决方案信息”页面，单击 **下一个**.

   ![](assets/image2015-3-19-9-21-50.png)

1. 确保选中SDK选项复选框。 单击 **导入**.

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待导入完成。

   >[!TIP]
   >
   >您需要启用浏览器上的弹出窗口才能完成安装过程。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下载日志文件（如果需要），然后单击 **关闭**.

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，但有警告”。 这完全符合预期。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management现在将显示在 **所有解决方案** 页面。

   ![](assets/image2015-3-19-8-40-38.png)

1. 选择Marketo解决方案，然后单击 **发布所有自定义项**.

   ![](assets/image2015-3-19-8-41-21.png)

   击掌！ 安装完成。

   >[!CAUTION]
   >
   >禁用任何Marketo SDK消息传递进程都将导致安装中断！

   >[!MORELIKETHIS]
   >
   >[安装Marketo for Dynamics 2015内部部署和2016 365内部部署步骤2/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
