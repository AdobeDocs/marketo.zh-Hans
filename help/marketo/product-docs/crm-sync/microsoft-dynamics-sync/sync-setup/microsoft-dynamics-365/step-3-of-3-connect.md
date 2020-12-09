---
unique-page-id: 3571830
description: 第3步，共3步——将Microsoft Dynamics与Marketo（在线）连接- Marketo Docs —— 产品文档
title: 第3步（共3步）-将Microsoft Dynamics与Marketo连接（联机）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---


# 第3步，共3步：将Microsoft Dynamics与Marketo连接（联机） {#step-of-connect-microsoft-dynamics-with-marketo-online}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

这是同步的最后一步。 我们快到了！

>[!PREREQUISITES]
>
>* [第1步，共3步：安装Marketo Solution（在线）](step-1-of-3-install.md)
   >
   >
* [第2步，共3步：在Dynamics中设置Marketo同步用户](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**需要管理员权限**

## 输入Dynamics Sync用户信息 {#enter-dynamics-sync-user-information}

1. 登录Marketo并单击“管 **理员**”。

   ![](assets/login-admin.png)

1. 单击 **CRM**。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 选择 **Microsoft**。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 单击 **步骤** 1 **中的编辑：输入凭据**。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确，因为我们无法在提交后还原后续模式更改。 如果保存的凭据不正确，您将必须获得新的Marketo订阅。

1. 输入 **Username**、 **Password**&#x200B;和Microsoft Dynamics **URL** （客户端ID和客户端机密是可选的）。 完成后 **单击** “保存”。

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#bcc9cfd9cefcd8d3d1ddd5d292dfd3d1) 或DOMAIN\user。

## 选择要同步的字段 {#select-fields-to-sync}

1. 单击 **步骤** 2 **中的编辑：选择要同步的字段**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择要同步到Marketo的字段，以便预先选择它们。 单击 **保存**。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请务必进入并选择要与Marketo同步的新字段。

1. 转至“管理员”并选 **择“Microsoft Dynamics**”。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“ **字段同步** ”详细信息上的“编辑”。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并进行检查。 实际名称必须是new_synctomkto，但显示名称可以是任何内容。 单击 **保存**。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 启用同步 {#enable-sync}

1. 单击 **步骤** 3 **中的编辑：启用同步**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动消除重复。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件地址，然后单击“ **开始同步”**。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 第一次同步可能需要几个小时。 完成后，您会收到一封电子邮件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

干得好！
