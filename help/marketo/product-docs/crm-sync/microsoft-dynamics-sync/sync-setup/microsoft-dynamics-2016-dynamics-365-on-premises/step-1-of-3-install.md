---
unique-page-id: 7504736
description: 安装适用于Microsoft Dynamics 2016/Dynamics 365的Marketo本地1（共3个） — Marketo文档 — 产品文档
title: 安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署步骤1（共3步）
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
source-git-commit: 1e20fdd1d3c6bba265ceabe499e0d7a4babf4ef1
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# 步骤1（共3步）：为Marketo配置同步用户(2016 On-Prem /Dynamics 365 On-Premise) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

在将Microsoft Dynamics 2015本地版或2016(Dynamics 365)与Marketo同步之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，无法将新CRM同步到现有的Marketo实例。

>[!PREREQUISITES]
>
>如果您使用的是Microsoft Dynamics On-Premise，则您必须 [面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) [Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 配置了2.0+(ADFS)。 注意：单击链接时，IFD文档会自动下载。
>
>[下载Marketo潜在客户管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 开始之前。

>[!NOTE]
>
>**需要Dynamics管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到 **动态。** 单击 **Microsoft Dynamics CRM** 下拉菜单，然后选择 **设置**.

   ![](assets/image2015-3-19-8-33-29.png)

1. 在 **设置**，选择 **解决方案**.

   ![](assets/image2015-3-19-8-33-3.png)

1. 单击 **导入**.

   ![](assets/image2015-3-19-8-34-8.png)

1. 单击 **浏览** 并选择您的解决方案 [下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 单击 **下一个**.

   ![](assets/image2015-3-19-9-20-56.png)

1. 查看解决方案信息，然后单击 **查看解决方案包详细信息**.

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
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下载日志文件（如果需要）并单击 **关闭**.

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，并出现警告”。 这是完全可以预料的。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management现在将显示在 **所有解决方案** 页面。

   ![](assets/image2015-3-19-8-40-38.png)

1. 选择Marketo解决方案，然后单击 **发布所有自定义设置**.

   ![](assets/image2015-3-19-8-41-21.png)

   五！ 安装完成。

   >[!CAUTION]
   >
   >禁用任何Marketo SDK消息传送流程都会导致安装中断！

   >[!MORELIKETHIS]
   >
   >[安装Marketo for Dynamics 2015内部版和2016 365内部版步骤2（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises/step-2-of-3-set-up.md)
