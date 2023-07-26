---
unique-page-id: 42762511
description: 设置Adobe组织映射 — Marketo文档 — 产品文档
title: 设置Adobe组织映射
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# 设置Adobe组织映射 {#set-up-adobe-organization-mapping}

为了与Adobe应用程序同步，例如Audience Manager、B2B CDP Marketo连接器、 [!DNL Dynamic Chat]等，您必须先在Marketo中输入Adobe IMS组织凭据。

>[!NOTE]
>
>Marketo实例的适用于HIPAA的部署无法使用此集成。

>[!CAUTION]
>
>对于已登记到Adobe业务平台和Identity Management System的客户，与订阅关联的组织ID将被填充，并且为只读字段。

1. 在Marketo中，单击 **[!UICONTROL 管理员]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. 在集成下，单击 **[!UICONTROL Adobe组织映射]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. 单击 **[!UICONTROL 编辑]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. 输入您的Adobe IMS组织ID(了解如何查找 [此处](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"})，然后单击 **[!UICONTROL 确定]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. 单击 **[!UICONTROL 确认]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. 单击&#x200B;**[!UICONTROL 关闭]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >出于安全原因，您必须是要映射到的Adobe组织的组织管理员。 否则，操作将失败。 此外，Adobe用户和Marketo用户在登录时必须使用相同的电子邮件地址。

1. 如果您是 _非_ 已登录，新选项卡/窗口中将显示一个弹出窗口。 登录到Adobe组织（此操作验证组织访问权限）。

就是这样！ 您现在可以 [共享受众数据](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} to, or [sync an audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} 来自Adobe Experience Cloud的。
