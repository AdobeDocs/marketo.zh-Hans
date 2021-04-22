---
unique-page-id: 3571827
description: 第2步（共3步） — 在Dynamics中设置Marketo Sync用户 — Marketo Docs — 产品文档
title: 第2步（共3步） — 在Dynamics中设置Marketo同步用户
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# 第2步，共3步：在Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}中设置Marketo同步用户

让我们通过创建用户帐户开始。

>[!PREREQUISITES]
>
>[第1步，共3步：安装Marketo解决方案（在线）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

## 创建新用户{#create-a-new-user}

1. 登录到Dynamics。 单击“设置”图标，然后选择&#x200B;**高级设置**。

   ![](assets/one.png)

1. 单击&#x200B;**设置**&#x200B;并选择&#x200B;**安全**。

   ![](assets/two.png)

1. 单击&#x200B;**用户**。

   ![](assets/three.png)

1. 单击&#x200B;**新建。**

   ![](assets/four.png)

1. 在新窗口中单击&#x200B;**添加和许可用户**。

   ![](assets/five.png)

1. 此时将打开一个新选项卡。 单击页面顶部的&#x200B;**管理员**。

   ![](assets/six.png)

1. 将打开另一个新选项卡。 单击&#x200B;**添加用户**。

   ![](assets/seven.png)

1. 输入您的所有信息。 完成后，单击&#x200B;**添加**。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名称必须是专用的同步用户，而不是现有CRM用户的帐户。 它不必是实际的电子邮件地址。

1. 输入要接收新用户凭据的电子邮件，然后单击&#x200B;**发送电子邮件并关闭**。

   ![](assets/nine.png)

## 分配同步用户角色{#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo 4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅[升级Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

1. 返回“已启用的用户”选项卡并刷新用户列表。

   ![](assets/ten.png)

1. 将鼠标悬停在新创建的Marketo Sync用户旁边，此时将显示一个复选框。 单击以选择它。

   ![](assets/eleven.png)

1. 单击&#x200B;**管理角色**。

   ![](assets/twelve.png)

1. 选中&#x200B;**Marketo Sync User**&#x200B;并单击&#x200B;**确定**。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步用户在您的CRM中所做的任何更新都将&#x200B;**不会**&#x200B;同步回Marketo。

## 配置Marketo解决方案{#configure-marketo-solution}

快到了！ 我们只剩下了通知Marketo Solution有关新用户创建的信息。

1. 返回“高级设置”部分，单击“设置”旁的![](assets/image2015-5-13-15-3a49-3a19.png)图标，然后选择&#x200B;**Marketo Config**。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果“设置”菜单中未显示&#x200B;**Marketo Config**，请刷新页面。 如果这行不通，请尝试再次[发布Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)或注销并重新登录。

1. 单击&#x200B;**默认**。

   ![](assets/fifteen.png)

1. 单击&#x200B;**Marketo User**&#x200B;字段上的搜索按钮，然后选择您创建的同步用户。

   ![](assets/sixteen.png)

1. 单击右下角的![](assets/image2015-3-13-15-3a10-3a11.png)图标以保存更改。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 单击右上角的&#x200B;**X**&#x200B;以关闭屏幕。

   ![](assets/seventeen.png)

1. 单击“设置”旁边的![](assets/image2015-5-13-15-3a49-3a19-1.png)图标，然后选择“**解决方案**”。

   ![](assets/eighteen.png)

1. 单击&#x200B;**发布所有自定义项**&#x200B;按钮。

   ![](assets/nineteen.png)

## 继续执行步骤3 {#before-proceeding-to-step}之前

    *如果要限制同步的记录数，请立即[设置自定义同步过滤器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *运行[验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。它验证初始设置是否正确。
    *在Microsoft Dynamics CRM中登录Marketo Sync用户。

>[!MORELIKETHIS]
>
>[第3步，共3步：将Microsoft Dynamics与Marketo（联机）连接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
