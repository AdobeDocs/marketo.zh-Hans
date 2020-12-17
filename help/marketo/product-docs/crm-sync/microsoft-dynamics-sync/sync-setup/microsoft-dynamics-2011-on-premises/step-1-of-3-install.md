---
unique-page-id: 3571805
description: 步骤1（共3步）-安装Marketo解决方案（2011年内部部署）- Marketo文档——产品文档
title: 步骤1（共3步）-安装Marketo解决方案（2011年内部部署）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# 第1步，共3步：安装Marketo解决方案（2011内部部署）{#step-of-install-the-marketo-solution-on-premises}

在同步Microsoft Dynamics On-Promess和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Market同步到CRM后，无法在不替换实例的情况下执行新同步。

>[!PREREQUISITES]
>
>必须配置[面向Internet的部署](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)(IFD)，并配置[Active Directory联合服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1或3.0(ADFS)。 **注意**:IFD文档在您单击链接时自动下载。
>
>[在开始之前，请先下](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 载Marketo Lead Management Solution。

>[!NOTE]
>
>**需要动态管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录&#x200B;**Dynamics**，在左下方菜单中选择&#x200B;**设置**。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 在树中选择&#x200B;**解决方案**。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 单击&#x200B;**导入**。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 单击&#x200B;**浏览**。 选择您[已下载的](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)的Marketo Lead Management解决方案。 单击&#x200B;**下一步**。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 视图解决方案信息，然后单击&#x200B;**视图解决方案包详细信息**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击&#x200B;**关闭**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页，单击&#x200B;**下一步**。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 确保选中SDK消息选项复选框。 单击&#x200B;**下一步**。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

1. 现在，请等待导入完成。 起来，好好休息一下。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 单击&#x200B;**关闭**。

   >[!NOTE]
   >
   >您可能会看到一条消息，说明“Marketo Lead Management已完成，但有警告”。 这完全是意料之中的。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management现在将显示在&#x200B;**所有解决方案**&#x200B;页面上。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 选择“Marketto Lead Management”，然后单击“**发布所有自定义项”。**

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
