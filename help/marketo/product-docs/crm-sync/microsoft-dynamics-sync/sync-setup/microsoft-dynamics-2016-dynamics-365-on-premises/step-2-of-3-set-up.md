---
description: 安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署第2步（共3步） — Marketo文档 — 产品文档
title: 安装Marketo for Microsoft Dynamics 2016/Dynamics 365本地步骤2/3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 步骤3中的2设置Marketo for Dynamics（2016内部部署/Dynamics 365内部部署）{#step-of-set-up-for-marketo-on-premises-2016}

出色完成了前面的步骤。 让我们继续讨论这个问题。

>[!PREREQUISITES]
>
>[安装Marketo for Microsoft Dynamics 2016/Dynamics 365本地步骤1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}

## 创建新用户 {#create-a-new-user}

1. 登录到Dynamics。 单击设置图标并选择高级设置。

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. 单击 **[!UICONTROL 设置]** 并选择 **[!UICONTROL 安全性]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. 单击 **[!UICONTROL 用户]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. 单击 **[!UICONTROL 新建]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. 单击 **[!UICONTROL 添加和许可用户]**. 此时应会打开一个新选项卡。

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. 单击 **[!UICONTROL 管理员]** 页面顶部的。 此时应会打开另一个新选项卡。

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. 单击 **[!UICONTROL 添加用户]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. 输入您的所有信息。 完成后，单击 **[!UICONTROL 添加]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >此名称必须是专用同步用户，而不是现有的CRM用户帐户。 它不需要是实际的电子邮件地址。

1. 输入要接收新用户凭据的电子邮件，然后单击发送电子邮件并关闭。

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## 创建新的客户端应用程序 {#create-a-new-client-application}

请按照中的步骤操作 [此Microsoft文章](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later){target="_blank"} 创建新的客户端应用程序并授予权限。 请记下Dynamics客户端应用程序的客户端ID/密码。

## 分配同步用户角色 {#assign-sync-user-role}

仅将Marketo同步用户角色分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅 [升级Marketo Microsoft Dynamics解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>同步用户的语言设置 [应设置为英语](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. 下 **[!UICONTROL 设置]**，单击 **[!UICONTROL 安全性]**.

   ![](assets/assign1.png)

1. 单击 **[!UICONTROL 用户]**.

   ![](assets/assign2.png)

1. 您将在此处看到用户列表。 选择专用的Marketo同步用户或联系您的 [Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS)管理员创建Marketo的专用用户。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击 **[!UICONTROL 管理角色]**.

   ![](assets/assign4.png)

1. 选中Marketo同步用户并单击 **[!UICONTROL 确定]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果您看不到角色，请返回 [第1步（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) 并导入解决方案。

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都将 _非_ 已同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们仅做了最后几段配置。

1. 下 **[!UICONTROL 设置]**，单击 **[!UICONTROL Marketo配置]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，请尝试刷新页面。 如果问题仍然存在， [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} 或者尝试注销并重新登录。

1. 单击 **[!UICONTROL 默认]**.

   ![](assets/configure2.png)

1. 单击 **[!UICONTROL Marketo用户]** 字段并选择同步用户。

   ![](assets/configure3.png)

1. 单击右下角的保存图标。

   ![](assets/configure4.png)

1. 单击 **[!UICONTROL 发布所有自定义项]**.

   ![](assets/publish-all-customizations1.png)

## 在继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数， [设置自定义同步过滤器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} 进程。 它验证初始设置是否正确完成。
* 登录到Microsoft Dynamics CRM中的“Marketo同步用户”。

>[!MORELIKETHIS]
>
>[安装Marketo for Microsoft Dynamics 2016/Dynamics 365本地步骤3/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md){target="_blank"}
