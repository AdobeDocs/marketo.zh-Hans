---
unique-page-id: 8783322
description: 验证Microsoft Dynamics同步- Marketo Docs —— 产品文档
title: 验证Microsoft Dynamics同步
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 验证Microsoft Dynamics同步 {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果您为Dynamics同步启用了多因素身份验证(MFA)，则必须禁用它，Dynamics才能与Marketo正确同步。 如需其他信息，请与Marketo [支持部门联系](http://nation.marketo.com/community/support_solutions)。

## 在Marketo中运行验证同步 {#run-validate-sync-in-marketo}

运行“验证同步”工具，确保在它们之间建立最终连接之前正确设置Microsoft Dynamics与Marketo的同步。 该过程生成一个包含七个设置步骤的清单，这些步骤可以找出存在问题的地方。 验证这些操作是否正确，可节省大量时间。

1. 单击“ **Admin** ”选项卡，然 **后单击“Integration** ”（集成）区域中的Microsoft Dynamics链接。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 选择 **Microsoft**。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 单击“验 **证同步设置** ”选项卡。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 输入您的用户名、密码和URL（客户端ID和客户端机密是可选的）。 完成后 **单击** “下一步”。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果您之前已同步， **则左** 树中的CRM将 **读取Microsoft Dynamics**，并且上述表单中的数据可能已预填充。

1. 如果一切正常，验证同步将生成一个包含绿色复选标记的核对 ![清单](assets/check.png)。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到， ![那](assets/delete.png)么该步骤会出现问题。 请参 [阅修复Dynamics验证同步问题](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) ，以识别并修复问题。 然后重新运行同步验证步骤，直到结果与上面的图像类似。

   >[!CAUTION]
   >
   >目前不支持Marketo Dynamics Sync的沙箱刷新。 如果需要刷新Dynamics CRM沙箱，将需要新的Marketo沙箱。 有关更多详细信息，请联系您的客户成功经理。

>[!MORELIKETHIS]
>
>[修复Dynamics验证同步问题](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

