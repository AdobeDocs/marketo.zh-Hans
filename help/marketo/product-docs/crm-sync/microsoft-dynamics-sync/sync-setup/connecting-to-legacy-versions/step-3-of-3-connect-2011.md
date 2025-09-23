---
unique-page-id: 3571809
description: 第3步（共3步） — 使用Marketo连接 [!DNL Microsoft Dynamics] （2011年内部部署） — Marketo文档 — 产品文档
title: 第3步（共3步） — 使用Marketo连接 [!DNL Microsoft Dynamics] （2011年内部部署）
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 第3步（共3步）：将[!DNL Microsoft Dynamics]与Marketo连接（2011年内部部署） {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

好吧！ 我们安装了解决方案并配置了同步用户。 接下来，我们需要连接Marketo和[!DNL Dynamics]。

>[!PREREQUISITES]
>
>* [第1步（共3步）：安装Marketo解决方案（2011年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)
>* [第2步（共3步）：在 [!DNL Dynamics] 中设置Marketo同步用户（2011年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)

>[!NOTE]
>
>**需要管理员权限**

## 输入[!DNL Dynamics]同步用户信息 {#enter-dynamics-sync-user-information}

1. 登录到Marketo并单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/login-admin.png)

1. 单击&#x200B;**[!UICONTROL CRM]**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 单击 **[!UICONTROL Microsoft]**。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中单击&#x200B;**[!UICONTROL Step 1: Enter credentials]**。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确，因为我们在提交后无法还原后续架构更改。 如果保存了不正确的凭据，您将必须获取新的Marketo订阅。

1. 输入&#x200B;**[!UICONTROL Username]**、**[!UICONTROL Password]**&#x200B;和CRM **[!UICONTROL URL]**，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Marketo中的[!UICONTROL Username]必须与CRM中同步用户的用户名匹配。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道该URL，[请在此处了解如何查找该URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。

## 选择要同步的字段 {#select-fields-to-sync}

现在，我们需要选择要同步的字段。

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中单击&#x200B;**[!UICONTROL Step 2: Select Fields to Sync]**。

   ![](assets/image2015-3-16-9-51-28a.png)

1. 存在将同步的预先选定的字段。 根据需要添加更多内容，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo存储对要同步的字段的引用。 如果删除[!DNL Dynamics]中的字段，我们建议在禁用[同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情况下执行此操作。 然后通过编辑并保存[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)来刷新Marketo中的架构。

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请确保进入并选择要与Marketo同步的新字段。

1. 转到管理员并选择&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击&#x200B;**[!UICONTROL Edit]**&#x200B;上的[!UICONTROL Field Sync Details]。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并选中。 实际名称必须是new_synctomkto ，但“显示名称”可以是任何内容。 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 启用同步 {#enable-sync}

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中单击&#x200B;**[!UICONTROL Step 3: Enable Sync]**。

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo不会针对[!DNL Microsoft Dynamics]同步或手动输入人员或潜在客户时自动执行重复数据删除。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件，然后单击&#x200B;**[!UICONTROL Start Sync]**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 根据记录数量，初始同步可能需要几小时到几天时间。 完成后，您将收到电子邮件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)
