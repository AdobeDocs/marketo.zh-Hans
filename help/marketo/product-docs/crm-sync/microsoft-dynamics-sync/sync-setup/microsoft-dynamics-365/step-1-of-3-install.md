---
unique-page-id: 3571822
description: 步骤1（共3步） — 安装Marketo解决方案（在线） — Marketo文档 — 产品文档
title: 步骤1（共3步） — 安装Marketo解决方案（在线）
exl-id: 593fc014-db38-42cc-8f9f-0dd8307751e8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 第1步，共3步：安装Marketo解决方案（在线）{#step-of-install-the-marketo-solution-online}

在同步Microsoft Dynamics 365和Marketo之前，您需要先在Dynamics中安装Marketo解决方案。 **需要Dynamics管理员权限。**

>[!CAUTION]
>
>* 在完成初始同步之前，请勿启用自定义实体同步。 完成初始同步后，您将通过电子邮件收到通知。
>* 如果您为Dynamics同步启用了多因素身份验证(MFA)，则必须禁用它，Dynamics才能与Marketo正确同步。 如需其他信息，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。


>[!NOTE]
>
>将Marketo同步到CRM后，无法在不替换实例的情况下执行新同步。

>[!PREREQUISITES]
>
>[下载Marketo Lead Management解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. 登录到&#x200B;**[Microsoft Office 365](https://login.microsoftonline.com/)**。

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. 单击![](assets/image2015-3-16-16-3a1-3a13.png)菜单并选择&#x200B;**CRM**。

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. 单击![](assets/image2015-5-13-10-3a5-3a8.png)菜单。 在下拉菜单中，选择&#x200B;**设置**，然后选择&#x200B;**解决方案**。

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 单击&#x200B;**导入。**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. 单击&#x200B;**选择文件。** 选择您下载的Marketo潜在客户管理解 [决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。单击&#x200B;**下一步**。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. 视图解决方案信息，然后单击&#x200B;**视图解决方案包详细信息**。

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. 检查完所有详细信息后，单击&#x200B;**关闭**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 现在，返回“解决方案信息”页，单击&#x200B;**下一步**。

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 确保选中“SDK”选项复选框。 单击&#x200B;**导入**。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

1. 现在，等待导入完成。 起来，拉一拉。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 单击&#x200B;**关闭。**

   >[!NOTE]
   >
   >您可能会看到一条消息，说“Marketo Lead Management已完成，但有警告”。 这完全是预期。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo潜在客户管理现在将出现在解决方案列表中。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 选择&#x200B;**Marketo潜在客户管理**&#x200B;并单击&#x200B;**发布所有自定义。**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   五！ 安装完成。

   >[!MORELIKETHIS]
   >
   >[第2步，共3步：在Dynamics中设置Marketo Sync用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)
