---
unique-page-id: 3571830
description: 第3步（共3步） — 将Marketo解决方案与服务器连接到服务器 — Marketo文档 — 产品文档
title: 第3步（共3步） — 将Marketo解决方案与服务器连接到服务器
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 第3步（共3步）：将Marketo解决方案与服务器连接到服务器 {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

这是同步的最后一步。 我们快到了！

>[!PREREQUISITES]
>
>* [第1步（共3步）：安装具有服务器到服务器连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [第2步（共3步）：设置具有服务器到服务器连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)

>[!NOTE]
>
>**需要管理员权限**

>[!IMPORTANT]
>
>如果您要从基本身份验证升级到OAuth，您需要联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support) 以获取有关更新附加参数的帮助。 启用此功能将暂时停止同步，直到输入新凭据并重新启用同步。 如果要恢复到旧的身份验证模式，可以禁用该功能（直到2022年4月）。

>[!NOTE]
>
>在输入新凭据之前，您可以 [在此处验证它们](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

## 输入Dynamics同步用户信息 {#enter-dynamics-sync-user-information}

1. 登录到Marketo并单击 **管理员**.

   ![](assets/login-admin.png)

1. 单击 **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 选择 **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 单击 **编辑** 在 **步骤1：输入凭据**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >请确保您的组织URL正确，因为我们在提交后无法还原后续架构更改。 如果使用不正确的组织URL，您将必须获取新的Marketo订阅。 如果您不知道该URL， [在此处了解如何查找它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

1. 输入Dynamics同步用户信息并单击 **保存** 完成时。

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >Marketo中的用户名必须匹配 [电子邮件地址](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) CRM中应用程序用户的名称。 格式可以是 `user@domain.com` 或DOMAIN\user。

## 选择要同步的字段 {#select-fields-to-sync}

1. 单击 **编辑** 在 **步骤2：选择要同步的字段**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择要同步到Marketo的字段，以便预先选择它们。 单击 **保存**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo存储对要同步的字段的引用。 如果您删除Dynamics中的字段，我们建议您使用 [同步已禁用](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Marketo然后，通过编辑并保存 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请确保进入并选择要与Marketo同步的新字段。

1. 转到管理员并选择 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击 **编辑** 在字段同步详细信息上。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并选中它。 实际名称必须是new_synctomkto ，但“显示名称”可以是任何内容。 单击 **保存**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 启用同步 {#enable-sync}

1. 单击 **编辑** 在 **步骤3：启用同步**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动执行重复数据删除。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件地址，然后单击 **开始同步**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 首次同步可能需要几个小时。 完成后，您将收到电子邮件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

干得好！
