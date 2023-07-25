---
unique-page-id: 3571819
description: 第3步（共3步） — 连接Marketo和Dynamics（2013年内部部署） — Marketo文档 — 产品文档
title: 第3步（共3步） — 连接Marketo和Dynamics（2013内部部署）
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 步骤3/3：连接Marketo和Dynamics（2013年内部部署） {#step-of-connect-marketo-and-dynamics-on-premises}

好吧！ 我们安装了解决方案并配置了同步用户。 接下来，我们需要连接Marketo和Dynamics。

>[!PREREQUISITES]
>
>* [步骤1/3：在Dynamics中安装Marketo解决方案（2013内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [第2步（共3步）：为Marketo配置同步用户（2013年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)

>[!NOTE]
>
>**需要管理员权限**

## 输入Dynamics同步用户信息 {#enter-dynamics-sync-user-information}

1. 登录到Marketo并单击 **管理员**.

   ![](assets/login-admin.png)

1. 单击 **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 选择 **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 单击 **编辑** 在 **步骤1：输入凭据**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确，因为我们在提交后无法还原后续架构更改。 如果保存了不正确的凭据，您必须获取新的Marketo订阅。

1. 输入 **用户名**， **密码** 和Microsoft Dynamics **URL** 然后单击 **保存**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是user@domain.com或DOMAIN\user。
   >* 如果您不知道该URL， [在此处了解如何查找它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## 选择要同步的字段 {#select-fields-to-sync}

现在，我们需要选择要同步的字段。

1. 单击 **编辑** 在 **步骤2：选择要同步的字段**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择要同步到Marketo的字段，以便预先选择它们。 单击 **保存**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

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

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 启用同步 {#enable-sync}

1. 单击 **编辑** 在 **步骤3：启用同步**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动执行重复数据删除。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件，然后单击 **开始同步**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 首次同步可能需要几个小时。 完成后，您将收到电子邮件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

干得好！ 您刚刚释放了Marketo和Microsoft Dynamics之间的双向同步功能。 如果您购买了Marketo Sales Insight，您会得到更多乐趣：

>[!MORELIKETHIS]
>
>[在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
