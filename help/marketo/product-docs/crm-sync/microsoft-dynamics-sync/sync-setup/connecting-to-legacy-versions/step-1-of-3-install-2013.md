---
unique-page-id: 3571813
description: 第1步（共3步） — 在Dynamics（2013年本地版）中安装Marketo解决方案 — Marketo文档 — 产品文档
title: 步骤1（共3步） — 在Dynamics中安装Marketo解决方案（2013年本地版）
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
source-git-commit: 64c5f03bd2320bfbffd257684d1482e995def83a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 步骤1（共3步）：在Dynamics（2013本地版）中安装Marketo解决方案 {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

在同步Microsoft Dynamics本地版和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，如果不替换实例，将无法执行新同步。

>[!PREREQUISITES]
>
>您必须 [面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) [Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 配置了2.0、2.1或3.0(ADFS)。 注意：单击链接时，IFD文档会自动下载。
>
>[下载Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 开始之前。

>[!NOTE]
>
>**需要Dynamics管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录 **动态**. 单击 **Microsoft Dynamics CRM** 下拉菜单，然后选择 **设置**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 在 **设置**，选择 **解决方案**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 单击 **导入**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 单击 **浏览** ，然后选择 [下载解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 单击 **下一个**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. 查看解决方案信息，然后单击 **查看解决方案包详细信息**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击 **关闭**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页面，单击 **下一个**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 确保选中SDK选项。 单击 **导入**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. 等待导入完成。

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 下载日志文件（如果需要）并单击 **关闭**.

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，并出现警告”。 这是完全可以预料的。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management现在将显示在 **所有解决方案** 页面。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. 选择Marketo解决方案，然后单击 **发布所有自定义设置**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

不是太糟吧？ 来吧，我会继续带你过去。

>[!CAUTION]
>
>禁用任何Marketo SDK消息传送流程都会导致安装中断！

>[!MORELIKETHIS]
>
>[步骤2（共3步）：为Marketo配置同步用户（2013本地版）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
