---
unique-page-id: 3571819
description: 第3步（共3步） — 连接Marketo和Dynamics（2013年内部部署） — Marketo文档 — 产品文档
title: 第3步（共3步） — 连接Marketo和Dynamics（2013内部部署）
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 第3步（共3步）：连接Marketo和Dynamics（2013年内部部署） {#step-of-connect-marketo-and-dynamics-on-premises}

好吧！ 我们安装了解决方案并配置了同步用户。 接下来，我们需要连接Marketo Engage和Dynamics。

>[!PREREQUISITES]
>
>* [第1步（共3步）：在Dynamics（2013内部部署）中安装Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"}
>* [第2步（共3步）：为Marketo配置同步用户（2013内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}

>[!NOTE]
>
>**需要管理员权限**

## 输入Dynamics同步用户信息 {#enter-dynamics-sync-user-information}

1. 登录到Marketo并单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/login-admin.png)

1. 单击&#x200B;**[!UICONTROL CRM]**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 选择 **[!DNL Microsoft]**。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 在&#x200B;**[!UICONTROL Enter Credentials]**&#x200B;中单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >请确保您的凭据正确，因为我们在提交后无法还原后续架构更改。 如果保存了不正确的凭据，您将必须获取新的Marketo订阅。

1. 输入&#x200B;**[!UICONTROL Username]**、**[!UICONTROL Password]**&#x200B;和Microsoft Dynamics **[!UICONTROL URL]**，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道该URL，[请在此处了解如何查找该URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

## 选择要同步的字段 {#select-fields-to-sync}

现在，我们需要选择要同步的字段。

1. 在&#x200B;**[!UICONTROL Select Fields to Sync]**&#x200B;中单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择您要同步到Marketo的字段，以便预先选择它们。 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo存储对要同步的字段的引用。 如果删除Dynamics中的字段，我们建议在禁用[同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}的情况下执行此操作。 然后通过编辑并保存[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}来刷新Marketo中的架构。

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请确保进入并选择要与Marketo同步的新字段。

1. 转到管理员并选择&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击字段同步详细信息中的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并选中。 实际名称必须是new_synctomkto ，但“显示名称”可以是任何内容。 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 启用同步 {#enable-sync}

1. 在&#x200B;**[!UICONTROL Enable Sync]**&#x200B;中单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动执行重复数据删除。

1. 阅读弹出窗口中的所有内容，输入您的电子邮件，然后单击&#x200B;**[!UICONTROL Start Sync]**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 根据记录数量，初始同步可能需要几小时到几天时间。 完成后，您将收到电子邮件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)


>[!MORELIKETHIS]
>
>[在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md){target="_blank"}
