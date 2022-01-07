---
unique-page-id: 3571830
description: 第3步（共3步） — 将Marketo解决方案与S2S连接连接 — Marketo文档 — 产品文档
title: 步骤3（共3步） — 将Marketo解决方案与S2S连接连接
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
source-git-commit: 549282b11bcf5fd48d29680f196e4534063b30f6
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 步骤3（共3步）：将Marketo解决方案与S2S连接连接 {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

这是同步的最后一步。 我们快到了！

>[!PREREQUISITES]
>
>* [步骤1（共3步）：安装具有S2S连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [步骤2（共3步）：使用S2S连接设置Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>在输入新凭据之前，您可以 [在此处验证](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

## 输入Dynamics Sync用户信息 {#enter-dynamics-sync-user-information}

1. 登录Marketo并单击 **管理员**.

   ![](assets/login-admin.png)

1. 单击 **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 选择 **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 单击 **编辑** in **步骤1:输入凭据**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >请确保您的组织URL正确，因为我们无法在提交后还原后续架构更改。 如果使用的组织URL不正确，您必须获取新的Marketo订阅。 如果您不知道URL， [了解如何在此处查找](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

1. 输入 **用户名**, **密码**, **客户端ID**, **客户端密钥**&#x200B;和Microsoft Dynamics **URL**. 单击 **保存** 完成时。

   ![](assets/step-3-of-3-s2s-5.png)

   >[!NOTE]
   >
   >Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是 `user@domain.com` 或域\用户。

## 选择要同步的字段 {#select-fields-to-sync}

1. 单击 **编辑** in **步骤2:选择要同步的字段**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择要同步到Marketo的字段，以便预先选择它们。 单击 **保存**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

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

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 启用同步 {#enable-sync}

1. 单击 **编辑** in **步骤3:启用同步**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动消除重复数据。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件地址，然后单击 **开始同步**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 第一次同步可能需要几个小时。 完成后，您将收到一封电子邮件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

干得好！