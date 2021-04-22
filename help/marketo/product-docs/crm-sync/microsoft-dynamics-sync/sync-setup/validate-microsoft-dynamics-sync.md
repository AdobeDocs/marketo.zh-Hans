---
unique-page-id: 8783322
description: 验证Microsoft Dynamics同步 — Marketo Docs — 产品文档
title: 验证Microsoft Dynamics同步
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# 验证Microsoft Dynamics同步{#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果您为Dynamics同步启用了多因素身份验证(MFA)，则必须禁用它，Dynamics才能与Marketo正确同步。 如需其他信息，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。

## 在Marketo {#run-validate-sync-in-marketo}中运行验证同步

运行“验证同步”工具非常重要，这样，在进行最终连接之前，必须确保与Marketo的Microsoft Dynamics同步设置正确。 该过程生成一个包含七个设置步骤的清单，这些步骤可以找出存在问题的地方。 验证这些操作是否正确，可节省很多时间。

1. 单击“Integration（集成）”区域中的&#x200B;**Admin**&#x200B;选项卡，然后单击&#x200B;**Microsoft Dynamics**&#x200B;链接。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 选择&#x200B;**Microsoft**。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 单击&#x200B;**验证同步设置**&#x200B;选项卡。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 输入您的用户名、密码和URL（客户端ID和客户端机密是可选的）。 完成后，单击&#x200B;**下一步**。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果您之前已同步，则左树中的&#x200B;**CRM**&#x200B;将读取&#x200B;**Microsoft Dynamics**，并且可能会预填充上述表单中的数据。

1. 如果一切正常，验证同步将生成一个包含绿色复选标记![—](assets/check.png)的核对清单。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到![—](assets/delete.png)，则该步骤存在问题。 请参阅[修复Dynamics验证同步问题](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以识别并修复问题。 然后重新运行同步验证步骤，直到结果与上面的图像类似。

   >[!CAUTION]
   >
   >我们当前不支持Marketo Dynamics Sync的沙箱刷新。 如果需要刷新Dynamics CRM沙箱，则需要新的Marketo沙箱。 有关更多详细信息，请联系您的客户成功经理。

>[!MORELIKETHIS]
>
>[修复Dynamics验证同步问题](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
