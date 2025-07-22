---
unique-page-id: 8783322
description: 验证 [!DNL Microsoft Dynamics] 同步 — Marketo文档 — 产品文档
title: 验证 [!DNL Microsoft Dynamics] 同步
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 验证[!DNL Microsoft Dynamics]同步 {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果您为[!DNL Dynamics]同步启用了多重身份验证(MFA)，则必须禁用它才能使[!DNL Dynamics]与Marketo正确同步。 有关详细信息，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。

## 在Marketo中运行验证同步 {#run-validate-sync-in-marketo}

运行验证同步工具是非常重要的，以确保在它们之间建立最终连接之前，您的[!DNL Microsoft Dynamics]与Marketo的同步设置正确。 该流程会生成一个包含七个设置步骤的核对表，以查明存在哪些问题。 验证这些操作是否正确可节省大量时间。

1. 单击集成区域中的&#x200B;**[!UICONTROL Admin]**&#x200B;选项卡，然后单击&#x200B;**[!DNL Microsoft Dynamics]**&#x200B;链接。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 选择 **[!DNL Microsoft]**。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 单击&#x200B;**[!UICONTROL Validate Sync Setup]**&#x200B;选项卡。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 输入用户名、密码和URL（客户端ID和客户端密钥是可选的）。 完成后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果您之前已同步，则左侧树中的&#x200B;**CRM**&#x200B;将读取&#x200B;**[!DNL Microsoft Dynamics]**，并且可能会预填充上述表单中的数据。

1. 如果一切正常，验证同步将生成一个充满绿色复选标记![—](assets/check.png)的核对清单。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到![—](assets/delete.png)，则该步骤存在问题。 请参阅[修复 [!DNL Dynamics] 验证同步问题](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以识别和修复问题。 然后，重新运行同步验证步骤，直到结果类似于上图。

   >[!CAUTION]
   >
   >我们当前不支持[!DNL Marketo Dynamics]同步的沙盒刷新。 如果您需要刷新[!DNL Dynamics] CRM沙盒，则需要新的Marketo沙盒。 请联系您的客户成功经理以了解更多详细信息。

>[!MORELIKETHIS]
>
>[修复 [!DNL Dynamics] 验证同步问题](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
