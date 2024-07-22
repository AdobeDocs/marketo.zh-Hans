---
description: 第2步（共4步） — 使用资源所有者密码控制连接设置Marketo解决方案 — Marketo文档 — 产品文档
title: 第2步（共4步） — 使用资源所有者密码控制连接设置Marketo解决方案
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# 第2步（共4步）：使用资源所有者密码控制连接设置Marketo解决方案 {#step-2-of-4-set-up-the-marketo-solution-ropc}

让我们从创建用户帐户开始。

>[!PREREQUISITES]
>
>[第1步（共4步）：安装具有资源所有者密码控制连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## 创建新用户 {#create-a-new-user}

1. 登录到Dynamics。 单击“设置”图标并选择&#x200B;**[!UICONTROL 高级设置]**。

   ![](assets/one.png)

1. 单击&#x200B;**[!UICONTROL 设置]**&#x200B;并选择&#x200B;**[!UICONTROL 安全性]**。

   ![](assets/two.png)

1. 单击&#x200B;**[!UICONTROL 用户]**。

   ![](assets/three.png)

1. 单击&#x200B;**[!UICONTROL 新建]**。

   ![](assets/four.png)

1. 在新窗口中单击&#x200B;**[!UICONTROL 添加并许可用户]**。

   ![](assets/five.png)

1. 此时将打开一个新选项卡。 单击页面顶部的&#x200B;**[!UICONTROL 管理员]**。

   ![](assets/six.png)

1. 此时将打开另一个新选项卡。 单击&#x200B;**[!UICONTROL 添加用户]**。

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >同步用户应具有对Marketo配置的读取权限。

1. 输入您的所有信息。 完成后，单击&#x200B;**[!UICONTROL 添加]**。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名称必须是专用同步用户，而不是现有的CRM用户帐户。 它不需要是实际的电子邮件地址。

1. 输入接收新用户凭据的电子邮件，然后单击&#x200B;**[!UICONTROL 发送电子邮件并关闭]**。

   ![](assets/nine.png)

## 分配同步用户角色 {#assign-sync-user-role}

仅将Marketo同步用户角色分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅[升级Marketo Microsoft Dynamics解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}。

>[!IMPORTANT]
>
>同步用户[的语言设置应设置为英语](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}。

1. 返回&#x200B;**[!UICONTROL 启用的用户]**&#x200B;选项卡并刷新用户列表。

   ![](assets/ten.png)

1. 将鼠标悬停在新创建的Marketo同步用户旁边，将会显示一个复选框。 单击以将其选中。

   ![](assets/eleven.png)

1. 单击&#x200B;**[!UICONTROL 管理角色]**。

   ![](assets/twelve.png)

1. 检查&#x200B;**[!UICONTROL Marketo同步用户]**&#x200B;并单击&#x200B;**[!UICONTROL 确定]**。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都&#x200B;_不会_&#x200B;同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快到了！ 我们只剩下通知Marketo解决方案所创建的新用户。

1. 返回到“高级设置”部分，单击“设置”旁边的![](assets/image2015-5-13-15-3a49-3a19.png)图标，然后选择&#x200B;**[!UICONTROL Marketo配置]**。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果在“设置”菜单中看不到&#x200B;**[!UICONTROL Marketo配置]**，请刷新页面。 如果仍无效，请尝试[再次发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}，或者注销并重新登录。

1. 单击&#x200B;**[!UICONTROL 默认值]**。

   ![](assets/fifteen.png)

1. 单击&#x200B;**[!UICONTROL Marketo User]**&#x200B;字段上的“搜索”按钮，然后选择您创建的同步用户。

   ![](assets/sixteen.png)

1. 单击右下角的![](assets/image2015-3-13-15-3a10-3a11.png)图标以保存更改。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 单击右上角的&#x200B;**X**&#x200B;以关闭屏幕。

   ![](assets/seventeen.png)

1. 单击“设置”旁边的![](assets/image2015-5-13-15-3a49-3a19-1.png)图标，然后选择&#x200B;**[!UICONTROL 解决方案]**。

   ![](assets/eighteen.png)

1. 单击&#x200B;**[!UICONTROL Publish所有自定义项]**&#x200B;按钮。

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[第3步（共4步）：连接Marketo解决方案与资源所有者密码控制连接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
