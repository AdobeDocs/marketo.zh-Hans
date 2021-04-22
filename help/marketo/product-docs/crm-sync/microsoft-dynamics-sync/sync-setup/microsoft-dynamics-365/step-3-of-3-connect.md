---
unique-page-id: 3571830
description: 第3步（共3步） — 将Microsoft Dynamics与Marketo（在线）连接 — Marketo文档 — 产品文档
title: 第3步（共3步） — 将Microsoft Dynamics与Marketo（联机）连接
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 第3步，共3步：将Microsoft Dynamics与Marketo（联机）{#step-of-connect-microsoft-dynamics-with-marketo-online}

这是同步的最后一步。 快到了！

>[!PREREQUISITES]
>
>* [第1步，共3步：安装Marketo解决方案（在线）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
>* [第2步，共3步：在Dynamics中设置Marketo Sync用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理权限**

## 输入Dynamics Sync用户信息{#enter-dynamics-sync-user-information}

1. 登录Marketo并单击&#x200B;**Admin**。

   ![](assets/login-admin.png)

1. 单击&#x200B;**CRM**。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 选择&#x200B;**Microsoft**。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 单击&#x200B;**步骤1中的**&#x200B;编辑&#x200B;**:输入凭据**。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确无误，因为我们无法在提交后还原后续模式更改。 如果保存的凭据不正确，则必须获得新的Marketo订阅。

1. 输入&#x200B;**Username**、**Password**&#x200B;和Microsoft Dynamics **URL**。 完成后，单击&#x200B;**保存**。

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >* 如果您的Marketo是在2020年10月之前设置的，则客户端ID和机密是可选字段。 否则，它们是强制性的。 获取此信息取决于您使用的MSD版本。
   >* Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道URL，[将了解如何在此处找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。


## 选择要同步{#select-fields-to-sync}的字段

1. 单击&#x200B;**步骤2中的**&#x200B;编辑&#x200B;**:选择要同步的字段**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择要同步到Marketo的字段，以预先选择它们。 单击&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

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

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 启用同步{#enable-sync}

1. 单击&#x200B;**步骤3中的**&#x200B;编辑&#x200B;**:启用Sync**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或在您手动输入人员或潜在客户时自动进行重复数据消除。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件地址，然后单击&#x200B;**开始同步**。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 第一次同步可能需要几个小时。 完成后，您将收到电子邮件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

干得好！
