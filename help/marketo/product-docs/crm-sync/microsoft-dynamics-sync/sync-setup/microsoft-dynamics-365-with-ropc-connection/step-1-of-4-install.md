---
description: 第1步（共4步） — 安装具有资源所有者密码控制连接的Marketo解决方案 — Marketo文档 — 产品文档
title: 步骤4之1 — 安装具有资源所有者密码控制连接的Marketo解决方案
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 第1步（共4步）：安装具有资源所有者密码控制连接的Marketo解决方案 {#step-1-of-4-install-the-marketo-solution-ropc}

在同步Microsoft Dynamics 365和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。 **需要Dynamics管理员权限。**

>[!CAUTION]
>
>* 在初始同步完成之前，请勿启用自定义实体同步。 初始同步完成后，您将收到电子邮件通知。
>* 如果您为Dynamics Sync启用了多重身份验证(MFA)，则必须禁用它以便Dynamics能够与Marketo正确同步。 欲知更多信息，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>将Marketo同步到CRM后，如果不替换该实例，则无法执行新的同步。

>[!PREREQUISITES]
>
>[下载Marketo商机管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. 登录 **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. 单击 ![](assets/image2015-3-16-16-3a1-3a13.png) 菜单并选择 **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. 单击 ![](assets/image2015-5-13-10-3a5-3a8.png) 菜单。 在下拉菜单中，选择 **设置** 然后选择 **解决方案**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 单击 **导入。**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. 单击 **选择“文件”。** 选择适合您的Marketo潜在客户管理解决方案 [已下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 单击 **下一个**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. 查看解决方案信息并单击 **查看解决方案包详细信息**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. 检查完所有详细信息后，单击 **关闭**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 现在，返回“解决方案信息”页面，单击 **下一个**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 确保选中SDK选项复选框。 单击 **导入**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >您需要启用浏览器上的弹出窗口才能完成安装过程。

1. 现在等待导入完成。 起床做些伸展运动。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 单击 **关闭。**

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，但有警告”。 这是完全符合预期的。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo潜在客户管理现在将显示在解决方案列表中。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 选择 **Marketo潜在客户管理** 并单击 **发布所有自定义项。**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   击掌！ 安装完成。

   >[!MORELIKETHIS]
   >
   >[第2步（共4步）：使用资源所有者密码控制连接设置Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
