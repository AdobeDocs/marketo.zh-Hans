---
unique-page-id: 3571809
description: 第3步（共3步） — 将Microsoft Dynamics与Marketo（2011年内部部署）连接 — Marketo文档 — 产品文档
title: 第3步（共3步） — 将Microsoft Dynamics与Marketo（2011年内部部署）连接
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# 第3步，共3步：将Microsoft Dynamics与Marketo（2011内部部署）{#step-of-connect-microsoft-dynamics-with-marketo-on-premises}连接

好！ 我们已安装解决方案并配置了同步用户。 接下来，我们需要将Marketo和Dynamics联系起来。

>[!PREREQUISITES]
>
>* [第1步，共3步：安装Marketo解决方案（2011内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)
>* [第2步，共3步：在Dynamics（2011年内部部署）中设置Marketo同步用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理权限**

## 输入Dynamics Sync用户信息{#enter-dynamics-sync-user-information}

1. 登录到Marketo，然后单击&#x200B;**管理**。

   ![](assets/login-admin.png)

1. 单击&#x200B;**CRM**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 单击&#x200B;**Microsoft**。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 单击&#x200B;**步骤1中的**&#x200B;编辑&#x200B;**:输入凭据。**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确无误，因为我们无法在提交后还原后续模式更改。 如果保存的凭据不正确，则必须获得新的Marketo订阅。

1. 输入&#x200B;**Username**、**Password**&#x200B;和CRM **URL**，然后单击&#x200B;**Save**。

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道URL，[将了解如何在此处找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。


## 选择要同步{#select-fields-to-sync}的字段

现在，我们需要选择要同步的字段。

1. 单击&#x200B;**步骤2中的**&#x200B;编辑&#x200B;**:选择要同步的字段。**

   ![](assets/image2015-3-16-9-51-28a.png)

1. 预先选择的字段将同步。 根据需要添加更多内容，然后单击&#x200B;**保存**。

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo存储对要同步的字段的引用。 如果您在Dynamics中删除字段，我们建议在[sync disabled](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情况下执行此操作。 然后，在Marketo中编辑并保存[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)，以刷新模式。

## 自定义筛选器{#sync-fields-for-a-custom-filter}的同步字段

如果已创建自定义过滤器，请务必进入并选择要与Marketo同步的新字段。

1. 转至“管理员”，然后选择&#x200B;**Microsoft Dynamics**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“字段同步详细信息”上的&#x200B;**编辑**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到该字段并检查它。 实际名称必须是new_synctomkto，但“显示名称”可以是任何内容。 单击&#x200B;**保存**。

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 启用同步{#enable-sync}

1. 单击&#x200B;**步骤3中的**&#x200B;编辑&#x200B;**:启用Sync**。

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或在您手动输入人员或潜在客户时自动进行重复数据消除。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件，然后单击&#x200B;**开始同步**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要几个小时。 完成后，您将收到电子邮件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   干得好！
