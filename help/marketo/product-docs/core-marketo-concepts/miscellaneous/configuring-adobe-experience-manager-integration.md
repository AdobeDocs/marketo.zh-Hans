---
unique-page-id: 30081815
description: 配置Adobe Experience Manager集成 — Marketo文档 — 产品文档
title: 配置 Adobe Experience Manager 集成
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 7%

---

# 配置 Adobe Experience Manager 集成 {#configuring-adobe-experience-manager-integration}

配置Adobe Experience Manager (AEM)，以便您可以访问、选择AEM资源，并将其导入Marketo Engage Design Studio。

>[!NOTE]
>
>**需要管理员权限**

>[!IMPORTANT]
>
>* 此集成仅适用于AEM的内部部署，AEM Cloud Service实施不支持此集成。
>
>* 目前，仅在Firefox中完全支持此功能。 该功能在Safari中不受支持，并且可能在最新版本的Chrome中不起作用，具体取决于您的SameSite Cookie设置。

1. 导航到Adobe Experience Manager （URL特定于您的公司）。

   ![](assets/one.png)

1. 您可以使用Adobe登录或本地登录。 在本例中，我们将本地登录。

   ![](assets/two.png)

1. 在&#x200B;**[!UICONTROL Tools]**&#x200B;中，单击&#x200B;**[!UICONTROL Operations]**&#x200B;并选择&#x200B;**[!UICONTROL Web Console]**。

   ![](assets/2a.png)

1. 在浏览器中，搜索“[!UICONTROL Adobe Granite Cross-Origin Resource Sharing Policy]”(在Windows上按ctrl+f，在Mac上按cmd+f)。

   ![](assets/three.png)

1. 单击右侧的&#x200B;**+**&#x200B;符号。

   ![](assets/four.png)

1. 在&#x200B;**[!UICONTROL Allowed Origins (Regexp)]**&#x200B;文本框中，键入`https://.*\.marketo\.com`并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/five-psd.png)

1. 在页面顶部的标题中，单击&#x200B;**[!UICONTROL Web Console]**&#x200B;并选择&#x200B;**[!UICONTROL System Information]**。

   ![](assets/six.png)

1. 在“服务器信息”下，单击&#x200B;**[!UICONTROL Restart]**&#x200B;按钮。

   ![](assets/seven.png)

1. 单击&#x200B;**[!UICONTROL OK]**&#x200B;确认。

   ![](assets/eight.png)

1. 在 Marketo Engage 中，单击 **[!UICONTROL Admin]**。

   ![](assets/nine.png)

1. 在集成下，选择&#x200B;**[!UICONTROL Adobe Experience Manager]**。

   ![](assets/ten.png)

1. 单击 **[!UICONTROL Edit]**。

   ![](assets/eleven.png)

1. 输入您的AEM URL并单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/twelve.png)
