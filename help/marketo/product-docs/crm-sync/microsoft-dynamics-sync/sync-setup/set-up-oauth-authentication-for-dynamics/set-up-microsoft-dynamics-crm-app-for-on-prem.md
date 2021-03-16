---
description: 设置Microsoft Dynamics CRM应用程序，用于On-Marketo Docs — 产品文档
title: 为On-prem设置Microsoft Dynamics CRM应用程序
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# 为On-prem {#set-up-microsoft-dynamics-crm-app-for-on-prem}设置Microsoft Dynamics CRM应用程序

Marketo中基于客户端ID/客户端机密的设置可针对AD FS(ver)进行预设。 或更高版本)。 对于旧版本的On-prem，请联系[Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support)，以使验证方法更改为仅基于用户ID和密码。

## 设置Microsoft Dynamics CRM应用程序{#set-up-microsoft-dynamics-crm-app}

按照[此Microsoft文章](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later)中的步骤操作。

完成后，下一步是&#x200B;**将Dynamics CRM生成的客户端Id和机密输入Marketo**。

## 在Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}中输入Dynamics CRM生成的客户端Id和密码

以下步骤适用于联机和预先版本。

1. 在Marketo中，单击&#x200B;**管理员**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. 单击&#x200B;**Microsoft Dynamics**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. 单击&#x200B;**禁用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. 在凭据旁，单击&#x200B;**编辑**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. 输入您之前检索到的&#x200B;**客户端ID**&#x200B;和&#x200B;**客户端机密**，然后按&#x200B;**保存**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. 单击&#x200B;**验证同步设置**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. 单击&#x200B;**下一步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. 您应当看到所有绿色复选标记。 单击&#x200B;**关闭**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >如果绿色复选标记中显示红色X，请参阅[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以了解修复选项。

1. 单击&#x200B;**启用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

就这样！
