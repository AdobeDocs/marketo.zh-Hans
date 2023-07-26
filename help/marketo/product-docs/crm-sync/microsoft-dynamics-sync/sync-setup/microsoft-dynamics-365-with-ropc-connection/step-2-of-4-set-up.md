---
description: 第2步（共4步） — 使用资源所有者密码控制连接设置Marketo解决方案 — Marketo文档 — 产品文档
title: 第2步（共4步） — 使用资源所有者密码控制连接设置Marketo解决方案
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 第2步（共4步）：使用资源所有者密码控制连接设置Marketo解决方案 {#step-2-of-4-set-up-the-marketo-solution-ropc}

让我们从创建用户帐户开始。

>[!PREREQUISITES]
>
>[第1步（共4步）：安装具有资源所有者密码控制连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)

## 创建新用户 {#create-a-new-user}

1. 登录到Dynamics。 单击设置图标并选择 **高级设置**.

   ![](assets/one.png)

1. 单击 **设置** 并选择 **安全性**.

   ![](assets/two.png)

1. 单击 **用户**.

   ![](assets/three.png)

1. 单击 **新建。**

   ![](assets/four.png)

1. 单击 **添加和许可用户** 在新窗口中打开。

   ![](assets/five.png)

1. 此时将打开一个新选项卡。 单击 **管理员** 页面顶部的。

   ![](assets/six.png)

1. 此时将打开另一个新选项卡。 单击 **添加用户**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >同步用户应具有对Marketo配置的读取权限。

1. 输入您的所有信息。 完成后，单击 **添加**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名称必须是专用同步用户，而不是现有的CRM用户帐户。 它不需要是实际的电子邮件地址。

1. 输入要接收新用户凭据的电子邮件，然后单击 **发送电子邮件并关闭**.

   ![](assets/nine.png)

## 分配同步用户角色 {#assign-sync-user-role}

仅将Marketo同步用户角色分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅 [升级适用于Microsoft Dynamics的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用户的语言设置 [应设置为英语](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 返回启用用户选项卡并刷新用户列表。

   ![](assets/ten.png)

1. 将鼠标悬停在新创建的Marketo同步用户旁边，将会显示一个复选框。 单击以将其选中。

   ![](assets/eleven.png)

1. 单击 **管理角色**.

   ![](assets/twelve.png)

1. Check **Marketo同步用户** 并单击 **确定**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都将 **非** 已同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快到了！ 我们只剩下通知Marketo解决方案所创建的新用户。

1. 返回高级设置部分，然后单击 ![](assets/image2015-5-13-15-3a49-3a19.png) 图标，然后选择 **Marketo配置**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您没有看到 **Marketo配置** 在“设置”菜单中，刷新页面。 如果这样行不通，请尝试 [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) 再次登录或注销并重新登录。

1. 单击 **默认**.

   ![](assets/fifteen.png)

1. 单击 **Marketo用户** 字段并选择您创建的同步用户。

   ![](assets/sixteen.png)

1. 单击 ![](assets/image2015-3-13-15-3a10-3a11.png) 图标以保存更改。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 单击 **X** 以关闭屏幕。

   ![](assets/seventeen.png)

1. 单击 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 图标，然后选择 **解决方案**.

   ![](assets/eighteen.png)

1. 单击 **发布所有自定义项** 按钮。

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[第3步（共4步）：连接Marketo解决方案与资源所有者密码控制连接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)
