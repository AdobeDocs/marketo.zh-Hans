---
unique-page-id: 3571809
description: 第3步（共3步） — 将Microsoft Dynamics与Marketo连接（2011年本地版） — Marketo文档 — 产品文档
title: 步骤3（共3步） — 将Microsoft Dynamics与Marketo连接（2011年内部部署）
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# 步骤3（共3步）：将Microsoft Dynamics与Marketo连接（2011年内部部署版） {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

好吧！ 我们安装了解决方案并配置了同步用户。 接下来，我们需要将Marketo和Dynamics连接起来。

>[!PREREQUISITES]
>
>* [步骤1（共3步）：安装Marketo解决方案（2011年内部部署版）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)
>* [步骤2（共3步）：在Dynamics（2011本地版）中设置Marketo同步用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理员权限**

## 输入Dynamics同步用户信息 {#enter-dynamics-sync-user-information}

1. 登录Marketo并单击 **管理员**.

   ![](assets/login-admin.png)

1. 单击 **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 单击 **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 单击 **编辑** in **步骤1:输入凭据。**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确无误，因为我们无法在提交后还原后续架构更改。 如果保存的凭据不正确，则必须获取新的Marketo订阅。

1. 输入 **用户名**, **密码** 和CRM **URL** 然后单击 **保存**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是 `user@domain.com` 或域\用户。
   >* 如果您不知道URL， [了解如何在此处查找](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## 选择要同步的字段 {#select-fields-to-sync}

现在，我们需要选择要同步的字段。

1. 单击 **编辑** in **步骤2:选择要同步的字段。**

   ![](assets/image2015-3-16-9-51-28a.png)

1. 有一些预先选择的字段将会同步。 如果需要，可添加更多，然后单击 **保存**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo存储对要同步的字段的引用。 如果删除Dynamics中的字段，我们建议使用 [已禁用](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). 然后，通过编辑和保存 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## 自定义过滤器的同步字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义过滤器，请务必进入并选择要与Marketo同步的新字段。

1. 转到“管理员”并选择 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击 **编辑** 在字段同步详细信息中。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并对其进行检查。 实际名称必须是new_synctomkto，但“显示名称”可以是任何内容。 单击 **保存**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 启用同步 {#enable-sync}

1. 单击 **编辑** in **步骤3:启用同步**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动消除重复数据。

1. 阅读弹出窗口中的所有内容，输入电子邮件，然后单击 **开始同步**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要几个小时。 完成后，您将收到一封电子邮件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   干得好！
