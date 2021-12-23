---
unique-page-id: 3571805
description: 第1步（共3步） — 安装Marketo解决方案（2011年本地版） — Marketo文档 — 产品文档
title: 步骤1（共3步） — 安装Marketo解决方案（2011年内部部署）
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
source-git-commit: eac7e219f1babc22dce30717fea4cecb93e1cce7
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 步骤1（共3步）：安装Marketo解决方案（2011年内部部署版） {#step-of-install-the-marketo-solution-on-premises}

在同步Microsoft Dynamics本地版和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，如果不替换实例，将无法执行新同步。

>[!PREREQUISITES]
>
>您必须 [面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) [Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 配置了2.0、2.1或3.0(ADFS)。 **注意**:单击链接时，IFD文档会自动下载。
>
>[下载Marketo潜在客户管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 开始之前。

>[!NOTE]
>
>**需要Dynamics管理员权限。**
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到 **动态**，选择 **设置** 菜单。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 选择 **解决方案** 在树上。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 单击 **导入**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 单击 **浏览**. 选择您的Marketo Lead Management解决方案 [下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 单击 **下一个**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 查看解决方案信息，然后单击 **查看解决方案包详细信息**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击 **关闭**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页面，单击 **下一个**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 确保选中SDK消息选项复选框。 单击 **下一个**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

1. 现在，等待导入完成。 起来，做些铺垫。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 单击 **关闭**.

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，并出现警告”。 这是完全可以预料的。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management现在将显示在 **所有解决方案** 页面。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 选择Marketo潜在客户管理并单击 **发布所有自定义设置。**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

不是太糟吧？ 来吧，我会继续带你过去。

>[!CAUTION]
>
>禁用任何Marketo SDK消息传送流程都会导致安装中断！

>[!MORELIKETHIS]
>
>[步骤2（共3步）：在Dynamics（2011本地版）中设置Marketo同步用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)