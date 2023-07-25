---
unique-page-id: 8783322
description: 验证Microsoft Dynamics同步 — Marketo文档 — 产品文档
title: 验证Microsoft Dynamics同步
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 验证Microsoft Dynamics同步 {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果您为Dynamics同步启用了多重身份验证(MFA)，则必须禁用它以便Dynamics能够与Marketo正确同步。 欲知更多信息，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

## 在Marketo中运行验证同步 {#run-validate-sync-in-marketo}

运行验证同步工具是非常重要的，以确保在它们之间建立最终连接之前，您的Microsoft Dynamics与Marketo同步设置正确。 该流程会生成一个包含七个设置步骤的核对表，以查明存在问题的地方。 验证这些操作是否正确完成可以节省大量时间。

1. 单击 **管理员** 选项卡，然后 **Microsoft Dynamics** 集成区域中的链接。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 选择 **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 单击 **验证同步设置** 选项卡。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 输入用户名、密码和URL（客户端ID和客户端密钥是可选的）。 单击 **下一个** 完成时。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果您之前已同步， **CRM** 在左侧树中将显示 **Microsoft Dynamics**，并且可以预填充上述表单中的数据。

1. 如果一切正常，验证同步会生成一个充满绿色复选标记的核对清单 ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到 ![—](assets/delete.png)，则该步骤有一个问题。 参见 [修复Dynamics验证同步问题](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) 识别并修复问题。 然后，重新运行同步验证步骤，直到结果类似于上图。

   >[!CAUTION]
   >
   >我们当前不支持Marketo Dynamics同步的沙盒刷新。 如果您需要刷新Dynamics CRM沙盒，则需要新的Marketo沙盒。 有关其他详细信息，请联系Adobe客户团队（您的客户经理）。

>[!MORELIKETHIS]
>
>[修复Dynamics验证同步问题](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
