---
unique-page-id: 3571809
description: 步骤3（共3步）-将Microsoft Dynamics与Marketo（2011年内部部署）连接- Marketo文档——产品文档
title: 第3步（共3步）-将Microsoft Dynamics与Marketo连接（2011年内部部署）
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# 第3步，共3步：将Microsoft Dynamics与Marketo连接（2011年内部部署） {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

好吧！ 我们已安装解决方案并配置了同步用户。 接下来，我们需要将Marketo和Dynamics联系起来。

>[!PREREQUISITES]
>
>* [第1步，共3步：安装Marketo解决方案（2011内部部署）](step-1-of-3-install.md)
>* [第2步，共3步：在Dynamics（2011年内部部署）中设置Marketo Sync用户](step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理员权限**

## 输入Dynamics Sync用户信息 {#enter-dynamics-sync-user-information}

1. 登录到Marketo并单击“管 **理员**”。

   ![](assets/login-admin.png)

1. 单击 **CRM**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 单击 **Microsoft**。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 单击 **步骤** 1 **中的编辑：输入凭据。**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确，因为我们无法在提交后还原后续模式更改。 如果保存的凭据不正确，您将必须获得新的Marketo订阅。

1. 输入用 **户名**、 **密码** 和CRM **URL** ，然 **后单击**&#x200B;保存。

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) 或DOMAIN\user。

   >[!TIP]
   >
   >不知道URL? 我们将在此处向您展示如何 [找到Dynamics Organization Service](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) URL。

## 选择要同步的字段 {#select-fields-to-sync}

现在，我们需要选择要同步的字段。

1. 单击 **步骤****2中的编辑：选择要同步的字段。**

   ![](assets/image2015-3-16-9-51-28a.png)

1. 预先选择的字段将同步。 根据需要添加更多内容，然后单击“ **保存**”。

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请务必进入并选择要与Marketo同步的新字段。

1. 转至“管理员”并选 **择“Microsoft Dynamics**”。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“ **字段同步** ”详细信息上的“编辑”。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并进行检查。 实际名称必须是new_synctomkto，但显示名称可以是任何内容。 单击 **保存**。

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 启用同步 {#enable-sync}

1. 单击 **步骤** 3 **中的编辑：启用同步**。

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动消除重复。

1. 阅读弹出窗口中的所有内容，输入电子邮件，然后单击“ **开始同步”**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要几个小时。 完成后，您将收到电子邮件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   干得好！
