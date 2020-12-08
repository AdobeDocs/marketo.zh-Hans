---
unique-page-id: 3571805
description: 步骤1（共3步）-安装Marketo解决方案（2011年内部部署）- Marketo文档——产品文档
title: 步骤1（共3步）-安装Marketo解决方案（2011年内部部署）
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# 第1步，共3步：安装Marketo解决方案（2011内部部署） {#step-of-install-the-marketo-solution-on-premises}

在同步Microsoft Dynamics On-Promess和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Market同步到CRM后，无法在不替换实例的情况下执行新同步。

>[!NOTE]
>
>**先决条件**
>
>您必须配 [置了Active Directory Federation Services](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) 2.0、 [](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.1或3.0(ADFS)的Internet Packed Deployment(IFD)。 **注意**:IFD文档在您单击链接时自动下载。
>
>[在开始之前，先下载Marketo](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Lead Management Solution。

>[!NOTE]
>
>**需要动态管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录 **到Dynamics**，在左 **下** 方的菜单中，选择“设置”。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 在树 **中选** 择解决方案。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 单击“ **导入**”。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 单击“ **浏览**”。 选择您下载的Marketo Lead Management解决 [方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 单击“ **下一步**”。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 视图解决方案信息，然后单击 **视图解决方案包详细信息**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击“关闭 **”**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页面，单击“下 **一步**”。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 确保选中SDK消息选项复选框。 单击“ **下一步**”。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

1. 现在，请等待导入完成。 起来，好好休息一下。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 单击 **关闭**。

   >[!NOTE]
   >
   >您可能会看到一条消息，说明“Marketo Lead Management已完成，但有警告”。 这完全是意料之中的。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management现在将显示在所有解决 **方案页** 。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 选择“Marketto Lead Management”，然后单击“ **发布所有自定义”。**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

还不算太糟吧？ 来吧，我会一直带你过去。

>[!CAUTION]
>
>禁用任何Marketo SDK消息传递进程将导致安装中断！

>[!NOTE]
>
>**相关文章**
>
>[第2步，共3步：在Dynamics（2011年内部部署）中设置Marketo Sync用户](step-2-of-3-set-up.md)
