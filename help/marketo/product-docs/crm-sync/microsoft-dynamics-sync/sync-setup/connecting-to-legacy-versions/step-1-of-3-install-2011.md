---
unique-page-id: 3571805
description: 第1步（共3步） — 安装Marketo解决方案（2011年内部部署） — Marketo文档 — 产品文档
title: 步骤1/3 — 安装Marketo解决方案（2011年内部部署）
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 2%

---

# 第1步（共3步）：安装Marketo解决方案（2011年内部部署） {#step-of-install-the-marketo-solution-on-premises}

在同步Microsoft Dynamics内部部署和Marketo Engage之前，您需要先在Dynamics中安装Marketo解决方案。

>[!NOTE]
>
>将Marketo同步到CRM后，如果不替换该实例，则无法执行新的同步。

>[!PREREQUISITES]
>
>您必须拥有 [面向互联网的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 已配置2.0、2.1或3.0 (ADFS)。 **注意**：单击链接时，会自动下载IFD文档。
>
>[下载Marketo商机管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} 开始之前。

>[!NOTE]
>
>**需要Dynamics管理员权限**.
>
>您需要CRM管理员权限才能执行此同步。

1. 登录到Dynamics并选择 **[!UICONTROL 设置]** ，位于左下角菜单中。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 选择 **[!UICONTROL 解决方案]** 在树上。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 单击 **[!UICONTROL 导入]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 单击 **[!UICONTROL 浏览]**. 选择适合您的Marketo潜在客户管理解决方案 [已下载](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. 单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 查看解决方案信息并单击 **[!UICONTROL 查看解决方案包详细信息]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 检查完所有详细信息后，单击 **[!UICONTROL 关闭]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回“解决方案信息”页面，单击 **[!UICONTROL 下一个]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 确保选中SDK消息选项复选框。 单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您需要启用浏览器上的弹出窗口才能完成安装过程。

1. 现在等待导入完成。 起床做些伸展运动。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 单击&#x200B;**[!UICONTROL 关闭]**。

   >[!NOTE]
   >
   >您可能会看到一条消息，显示“Marketo潜在客户管理已完成，但有警告”。 这是完全符合预期的。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management现在将显示在 **所有解决方案** 页面。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 选择Marketo Lead Management ，然后单击 **[!UICONTROL 发布所有自定义项]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>禁用任何Marketo SDK消息传递过程都将导致安装中断！

>[!MORELIKETHIS]
>
>[步骤2（共3步）：在Dynamics中设置Marketo同步用户（2011内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}
