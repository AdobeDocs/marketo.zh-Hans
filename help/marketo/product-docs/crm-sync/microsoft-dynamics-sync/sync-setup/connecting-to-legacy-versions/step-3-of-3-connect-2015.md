---
unique-page-id: 7504744
description: 安装适用于Microsoft Dynamics 2015的Marketo本地步骤3/3 - Marketo文档 — 产品文档
title: 安装适用于Microsoft Dynamics 2015的Marketo本地步骤3（共3步）
exl-id: 054bf725-7a80-4114-8360-2d86e2e33dd7
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

# 第3步（共3步）：连接Marketo [!DNL Dynamics]（2015年内部部署） {#step-of-connect-marketo-dynamics-on-premises-2015}

>[!PREREQUISITES]
>
>* [安装Marketo for [!DNL Microsoft Dynamics] 2015本地步骤1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)
>* [为 [!DNL Microsoft Dynamics] 2015年内部部署安装Marketo第2步（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)

>[!NOTE]
>
>**需要管理员权限**

## 输入[!DNL Dynamics]同步用户信息 {#enter-dynamics-sync-user-information}

1. 登录到Marketo并单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/login-admin.png)

1. 单击 **[!UICONTROL CRM]**。

   ![](assets/image2015-3-16-9-47-34.png)

1. 选择 **[!UICONTROL Microsoft]**。

   ![](assets/image2015-3-16-9-50-6.png)

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中单击&#x200B;**[!UICONTROL Step 1: Enter Credentials]**。

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确，因为我们在提交后无法还原后续架构更改。 如果保存了不正确的凭据，您将必须获取新的Marketo订阅。

1. 输入&#x200B;**[!UICONTROL Username]**、**[!UICONTROL Password]** [!DNL Microsoft Dynamics] **URL**&#x200B;和&#x200B;**[!UICONTROL Client Id]/[!UICONTROL Client Secret]**。 完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 如果您的Marketo是在2020年10月之前配置的，则客户端ID和密码是可选字段。 否则，它们是强制性的。 此信息的获取将取决于您使用的MSD版本。
   >* Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道该URL，[请在此处了解如何查找该URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

   >[!TIP]
   >
   >不知道URL？ 我们将在此处说明如何查找您的[Dynamics组织服务URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

## 选择要同步的字段 {#select-fields-to-sync}

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中单击&#x200B;**[!UICONTROL Step 2: Select Fields to Sync]**。

   ![](assets/image2015-3-16-9-51-28.png)

1. 选择您要同步到Marketo的字段，以便预先选择它们。 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo存储对要同步的字段的引用。 如果删除[!DNL Dynamics]中的字段，我们建议在禁用[同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情况下执行此操作。 然后通过编辑和保存[[!UICONTROL Select Fields to Sync]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)在Marketo中刷新架构。

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请确保进入并选择要与Marketo同步的新字段。

1. 转到[!UICONTROL Admin]并选择&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击&#x200B;**[!UICONTROL Edit]**&#x200B;上的[!UICONTROL Field Sync Details]。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并选中。 实际名称必须是new_synctomkto ，但“显示名称”可以是任何内容。 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 启用同步 {#enable-sync}

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中单击&#x200B;**[!UICONTROL Step 3: Enable Sync]**。

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo不会针对[!DNL Microsoft Dynamics]同步或手动输入人员自动执行重复数据删除。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件，然后单击&#x200B;**[!UICONTROL Start Sync]**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 根据记录数量，初始同步可能需要几小时到几天时间。 完成后，您将收到电子邮件通知。

   ![](assets/image2015-3-16-9-59-51.png)
