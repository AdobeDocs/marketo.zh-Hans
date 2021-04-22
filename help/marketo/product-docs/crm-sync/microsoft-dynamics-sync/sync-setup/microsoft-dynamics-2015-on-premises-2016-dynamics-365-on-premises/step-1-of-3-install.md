---
unique-page-id: 7504736
description: 安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤1（共3步） — Marketo文档 — 产品文档
title: 安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤1（共3步）
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 第1步，共3步：为Marketo配置同步用户（2015 On-Prem和2016 365 On-Prem）{#step-of-configure-sync-user-for-marketo-on-premises-and-365}

在将Microsoft Dynamics 2015本地版或2016(Dynamics 365)与Marketo同步之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，您无法将新CRM同步到现有Marketo实例。

>[!PREREQUISITES]
>
>如果您使用的是Microsoft Dynamics内部部署，则必须配置[Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+(ADFS)的[面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)(IFD)。 注意：当您单击该链接时，IFD文档会自动下载。
>
>[在开始之前，请下](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 载Marketo Lead Management解决方案。

>[!NOTE]
>
>**需要Dynamics管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到&#x200B;**Dynamics。** 单击Microsoft  **Dynamics** CRM下拉菜单并选择 **设置**。

   ![](assets/image2015-3-19-8-33-29.png)

1. 在&#x200B;**设置**&#x200B;下，选择&#x200B;**解决方案**。

   ![](assets/image2015-3-19-8-33-3.png)

1. 单击&#x200B;**导入**。

   ![](assets/image2015-3-19-8-34-8.png)

1. 单击&#x200B;**浏览**&#x200B;并选择您[已下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)的解决方案。 单击&#x200B;**下一步**。

   ![](assets/image2015-3-19-9-20-56.png)

1. 视图解决方案信息，然后单击&#x200B;**视图解决方案包详细信息**。

   ![](assets/image2015-11-18-11-12-8.png)

1. 检查完所有详细信息后，单击&#x200B;**关闭**。

   ![](assets/step6.png)

1. 返回“解决方案信息”页，单击&#x200B;**下一步**。

   ![](assets/image2015-3-19-9-21-50.png)

1. 确保选中“SDK”选项复选框。 单击&#x200B;**导入**。

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待导入完成。

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下载日志文件（如果需要），然后单击&#x200B;**关闭**。

   >[!NOTE]
   >
   >您可能会看到一条消息，说“Marketo Lead Management已完成，但有警告”。 这完全是预期。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo潜在客户管理现在将显示在&#x200B;**所有解决方案**&#x200B;页面上。

   ![](assets/image2015-3-19-8-40-38.png)

1. 选择Marketo解决方案，然后单击&#x200B;**发布所有自定义项**。

   ![](assets/image2015-3-19-8-41-21.png)

   五！ 安装完成。

   >[!CAUTION]
   >
   >禁用任何Marketo SDK消息传递进程将导致安装中断！

   >[!MORELIKETHIS]
   >
   >[安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤2（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
