---
unique-page-id: 3571827
description: 步骤2（共3步）-在Dynamics中设置Marketo Sync用户- Marketo Docs —— 产品文档
title: 第2步（共3步）-在Dynamics中设置Marketo Sync用户
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---


# 第2步，共3步：在Dynamics中设置Marketo同步用户 {#step-of-set-up-marketo-sync-user-in-dynamics}

让我们通过创建用户帐户开始。

>[!PREREQUISITES]
>
>[第1步，共3步：安装Marketo Solution（在线）](step-1-of-3-install.md)

## 创建新用户 {#create-a-new-user}

1. 登录Dynamics。 单击“设置”图标，然后选择“ **高级设置”**。

   ![](assets/one.png)

1. 单击**设置**并选择“安 **全性**”。

   ![](assets/two.png)

1. 单击“ **用户**”。

   ![](assets/three.png)

1. 单击 **新建。**

   ![](assets/four.png)

1. 在新 **窗口中单击** “添加和授权用户”。

   ![](assets/five.png)

1. 此时将打开一个新选项卡。 单 **击页** 面顶部的“管理员”。

   ![](assets/six.png)

1. 将打开另一个新选项卡。 单击 **添加用户**。

   ![](assets/seven.png)

1. 输入您的所有信息。 完成后，单击“添 **加”**。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名称必须是专用的同步用户，而不是现有CRM用户的帐户。 它不必是实际的电子邮件地址。

1. 输入要接收新用户凭据的电子邮件，然后单击“发 **送电子邮件并关闭**”。

   ![](assets/nine.png)

## 分配同步用户角色 {#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo Sync用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户必须具有同步用户角色。 要升级Marketo，请参 [阅Microsoft Dynamics的Upgrade Marketo解决方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 返回“已启用的用户”选项卡并刷新用户列表。

   ![](assets/ten.png)

1. 将鼠标悬停在新创建的Marketo Sync用户旁边，将显示一个复选框。 单击以选择它。

   ![](assets/eleven.png)

1. 单击 **管理角色**。

   ![](assets/twelve.png)

1. 选中 **Marketto Sync User** ，然后单 **击确定**。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都 **不会** 同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快到了！ 我们只剩下向Marketo Solution通知所创建的新用户。

1. 返回“高级设置”部分，单击“设 ![](assets/image2015-5-13-15-3a49-3a19.png)置”旁边的图标，然后选择“ **Marketto配置”**。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果“设置”菜单中 **未显示Marketo** Config，请刷新页面。 如果这不起作用，请尝试再次 [发布Marketo Solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations)[](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) ，或注销并重新登录。

1. 单击 **默认**。

   ![](assets/fifteen.png)

1. 单击Marketo用户字段上 **的搜索按钮** ，然后选择您创建的同步用户。

   ![](assets/sixteen.png)

1. 单击 ![](assets/image2015-3-13-15-3a10-3a11.png)右下角的图标以保存更改。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 单击 **右上** 方的X以关闭屏幕。

   ![](assets/seventeen.png)

1. 单击“设 ![](assets/image2015-5-13-15-3a49-3a19-1.png)置”旁的图标，然后选择“解决 **方案”**。

   ![](assets/eighteen.png)

1. 单击“发 **布所有自定义** ”按钮。

   ![](assets/nineteen.png)

## 在继续执行步骤3之前 {#before-proceeding-to-step}

    *如果要限制同步的记录数，请立即[设置自定义同步过滤器](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *运行[验证Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。 它验证初始设置是否正确完成。
    *在Microsoft Dynamics CRM中登录Marketo Sync用户。

>[!NOTE]
>
>**相关文章**
>
>
>[第3步，共3步：将Microsoft Dynamics与Marketo连接（联机）](step-3-of-3-connect.md)
