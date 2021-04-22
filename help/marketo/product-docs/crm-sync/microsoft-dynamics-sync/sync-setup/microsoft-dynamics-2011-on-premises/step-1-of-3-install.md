---
unique-page-id: 3571805
description: 步骤1（共3步） — 安装Marketo解决方案（2011年内部部署） — Marketo文档 — 产品文档
title: 步骤1（共3步） — 安装Marketo解决方案（2011年内部部署）
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 第1步，共3步：安装Marketo解决方案（2011内部部署）{#step-of-install-the-marketo-solution-on-premises}

在同步Microsoft Dynamics On-Premise和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，无法在不替换实例的情况下执行新同步。

>[!PREREQUISITES]
>
>您必须配置[面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)(IFD)，并配置[ Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1或3.0(ADFS)。 **注意**:当您单击该链接时，IFD文档会自动下载。
>
>[在开始之前，请下](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 载Marketo Lead Management解决方案。

>[!NOTE]
>
>**需要Dynamics管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到&#x200B;**Dynamics**，在左下方菜单中选择&#x200B;**设置**。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 在树中选择&#x200B;**解决方案**。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 单击&#x200B;**导入**。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 单击&#x200B;**浏览**。 选择您[已下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)的Marketo潜在客户管理解决方案。 单击&#x200B;**下一步**。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 视图解决方案信息，然后单击&#x200B;**视图解决方案包详细信息**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击&#x200B;**关闭**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页，单击&#x200B;**下一步**。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 确保选中“SDK消息”选项复选框。 单击&#x200B;**下一步**。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

1. 现在，等待导入完成。 起来，拉一拉。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 单击&#x200B;**关闭**。

   >[!NOTE]
   >
   >您可能会看到一条消息，说“Marketo Lead Management已完成，但有警告”。 这完全是预期。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo潜在客户管理现在将显示在&#x200B;**所有解决方案**&#x200B;页面上。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 选择“Marketo潜在客户管理”，然后单击&#x200B;**发布所有自定义。**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

不是太糟吧？ 来吧，我会一直陪着你。

>[!CAUTION]
>
>禁用任何Marketo SDK消息传递进程将导致安装中断！

>[!MORELIKETHIS]
>
>[第2步，共3步：在Dynamics（2011年内部部署）中设置Marketo同步用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
