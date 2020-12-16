---
unique-page-id: 3571819
description: 第3步，共3步-Connect Marketo和Dynamics（2013年内部部署）- Marketo文档——产品文档
title: 第3步（共3步）- Connect Marketo和Dynamics（2013年内部部署）
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---


# 第3步，共3步：Connect Marketo和Dynamics（2013年内部部署） {#step-of-connect-marketo-and-dynamics-on-premises}

好吧！ 我们已安装解决方案并配置了同步用户。 接下来，我们需要将Marketo和Dynamics联系起来。

>[!PREREQUISITES]
>
>* [第1步，共3步：在Dynamics（2013内部部署）中安装Marketo解决方案](step-1-of-3-install.md)
>* [第2步，共3步：为Marketo配置同步用户（2013年本地版）](step-2-of-3-configure.md)

>



>[!NOTE]
>
>**需要管理员权限**

## 输入Dynamics Sync用户信息 {#enter-dynamics-sync-user-information}

1. 登录Marketo并单击“管 **理员**”。

   ![](assets/login-admin.png)

1. 单击 **CRM**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 选择 **Microsoft**。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 在第 **1步** 中单 **击“编辑”:输入凭据**。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确，因为我们无法在提交后还原后续模式更改。 如果保存的凭据不正确，您将必须获得新的Marketo订阅。

1. 输入用 **户名**、 **密码** 和Microsoft Dynamics **URL** ，然后单 ****&#x200B;击保存。

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#631610061123070c0e020a0d4d000c0e) 或DOMAIN\user。

   >[!TIP]
   >
   >不知道URL? 我们将在此处向您展示如何 [找到Dynamics Organization Service](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) URL。

## 选择要同步的字段 {#select-fields-to-sync}

现在，我们需要选择要同步的字段。

1. 在步骤2中，单击** **编辑**:选择要同步的字段**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择要同步到Marketo的字段，以便预先选择它们。 单击 **保存**。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请务必进入并选择要与Marketo同步的新字段。

1. 转至“管理员”并选 **择“Microsoft Dynamics**”。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“ **字段同步** ”详细信息上的“编辑”。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并进行检查。 实际名称必须是new_synctomkto，但显示名称可以是任何内容。 单击 **保存**。

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 启用同步 {#enable-sync}

1. 在步骤3中单击** **编辑**:启用同步**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动消除重复。

1. 阅读弹出窗口中的所有内容，输入电子邮件，然后单击“ **开始同步”**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要几个小时。 完成后，您将收到电子邮件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

干得好！ 您刚刚释放了Marketo和Microsoft Dynamics之间双向同步的强大功能。 如果您已购买Marketo Sales Insight，您会有更多乐趣：

>[!NOTE]
>
>**相关文章**
>
>* [在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight](../../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)

>



