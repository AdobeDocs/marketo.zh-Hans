---
description: 第4步（共4步） — 将Marketo解决方案与资源所有者密码控制连接连接 — Marketo文档 — 产品文档
title: 第4步（共4步） — 将Marketo解决方案与资源所有者密码控制连接连接
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 第4步（共4步）：连接Marketo解决方案与资源所有者密码控制连接 {#step-4-of-4-connect-the-marketo-solution-ropc}

这是同步的最后一步。 你快到了！

>[!PREREQUISITES]
>
>* [第1步（共4步）：安装具有资源所有者密码控制连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [第2步（共4步）：使用资源所有者密码控制连接设置Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
>* [第3步（共4步）：在MS Dynamics上设置客户端应用程序](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>如果您正在从基本身份验证升级到OAuth，您可以使用[此文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}来重新配置您的身份验证。

## 输入Dynamics同步用户信息 {#enter-dynamics-sync-user-information}

1. 登录到Marketo并单击&#x200B;**A分钟**。

   ![](assets/login-admin.png)

1. 单击 **[!UICONTROL CRM]**。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 选择 **[!UICONTROL Microsoft]**。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 在&#x200B;**[!UICONTROL Enter Credentials]**&#x200B;中单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >请确保您的组织URL正确，因为提交后我们无法还原后续架构更改。 如果使用的组织URL不正确，您将必须获取新的Marketo订阅。 如果您不知道该URL，[请在此处了解如何查找该URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

   >[!NOTE]
   >
   >在输入新凭据之前，您可以[在此处](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}验证它们。

1. 输入&#x200B;**[!UICONTROL Username]**、**[!UICONTROL Password]**、Microsoft Dynamics **URL**、**[!UICONTROL Client ID]**&#x200B;和&#x200B;**[!UICONTROL Client Secret]**。 完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Marketo中的用户名必须与CRM中同步用户的用户名匹配。 格式可以是`user@domain.com`或DOMAIN\user。

## 选择要同步的字段 {#select-fields-to-sync}

1. 在&#x200B;**[!UICONTROL Select Fields to Sync]**&#x200B;中单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 选择您要同步到Marketo的字段，以便预先选择它们。 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo存储对要同步的字段的引用。 如果删除Dynamics中的字段，我们建议在禁用[同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}的情况下执行此操作。 然后通过编辑并保存[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}来刷新Marketo中的架构。

## 同步自定义筛选器的字段 {#sync-fields-for-a-custom-filter}

如果已创建自定义筛选器，请确保进入并选择要与Marketo同步的新字段。

1. 转到管理员并选择&#x200B;**[!DNL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击字段同步详细信息中的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并选中。 实际名称必须是new_synctomkto ，但“显示名称”可以是任何内容。 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 启用同步 {#enable-sync}

1. 在&#x200B;**[!UICONTROL Enable Sync]**&#x200B;中单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不会针对Microsoft Dynamics同步或手动输入人员或潜在客户时自动执行重复数据删除。

1. 读取弹出窗口中的所有内容，输入您的电子邮件地址，然后单击&#x200B;**[!UICONTROL Start Sync]**。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 根据记录数量，初始同步可能需要几小时到几天时间。 完成后，您将收到电子邮件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

>[!MORELIKETHIS]
>
>[重新配置Dynamics身份验证方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
