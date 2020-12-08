---
unique-page-id: 3571813
description: 步骤1（共3步）-在Dynamics（2013内部部署）中安装Marketo Solution - Marketo Docs —— 产品文档
title: 步骤1（共3步）-在Dynamics（2013年内部部署）中安装Marketo解决方案
translation-type: tm+mt
source-git-commit: ce8b67b8549d23ff4ddd1d341632c6c5ff33990d
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# 第1步，共3步：在Dynamics（2013内部部署）中安装Marketo解决方案 {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

在同步Microsoft Dynamics On-Promess和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Market同步到CRM后，无法在不替换实例的情况下执行新同步。

>[!NOTE]
>
>**先决条件**
>
>您必须配 [置了Active Directory Federation Services](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) 2.0、 [](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.1或3.0(ADFS)的Internet Packed Deployment(IFD)。 注意：IFD文档在您单击链接时自动下载。
>
>[在开始之前先下载Marketo](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Solution。

>[!NOTE]
>
>**需要动态管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录 **Dynamics**。 单击 **Microsoft Dynamics CRM** 下拉菜单并选择 **SETTINGS**。

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 在“设 **置**”下，选 **择“解决方案**”。

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 单击“ **导入**”。

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 单击“ **浏览** ”并选择已 [下载的解决方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 单击“ **下一步**”。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. 视图解决方案信息，然后单击 **视图解决方案包详细信息**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击“关闭 **”**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页面，单击“下 **一步**”。

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 确保选中SDK选项。 单击“ **导入**”。

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. 等待导入完成。

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 下载日志文件（如果需要），然后单击“关 **闭”**。

   >[!NOTE]
   >
   >您可能会看到一条消息，说明“Marketo Lead Management已完成，但有警告”。 这完全是意料之中的。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management现在将显示在所有解决 **方案页** 。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. 选择Marketo解决方案，然后单击 **发布所有自定义**。

   ![](assets/image2014-12-11-10-3a41-3a32.png)

还不算太糟吧？ 来吧，我会一直带你过去。

>[!CAUTION]
>
>禁用任何Marketo SDK消息传递进程将导致安装中断！

>[!NOTE]
>
>**相关文章**
>
>* [第2步，共3步：为Marketo配置同步用户（2013年本地版）](step-2-of-3-configure.md)

>



