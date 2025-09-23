---
unique-page-id: 42762519
description: 现有客户的配置 — Marketo文档 — 产品文档
title: 现有客户的配置
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 10%

---

# 现有客户的配置 {#configuration-for-existing-customers}

请设置以下配置以开始使用新的分析仪表板。

>[!PREREQUISITES]
>
>请确保已将[!DNL Salesforce]包升级到最新版本

## 在Marketo中配置[!DNL Sales Insight] {#configure-sales-insight-in-marketo}

1. 在浏览器中打开新选项卡，以从您的Marketo帐户获取[!DNL Marketo Sales Insights]凭据。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/configuration-for-existing-customers-1.png)

1. 单击 **[!UICONTROL Sales Insight]**。

   ![](assets/configuration-for-existing-customers-2.png)

1. 单击&#x200B;**[!UICONTROL View]**&#x200B;以填充Rest API凭据。

   ![](assets/configuration-for-existing-customers-3.png)

1. 您将会看到确认弹出窗口。 单击 **[!UICONTROL OK]**。

## 在[!DNL Sales Insight]中配置[!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击&#x200B;**[!UICONTROL Setup]**。

   ![](assets/configuration-for-existing-customers-4.png)

1. 搜索并选择&#x200B;**[!UICONTROL Remote Site Settings]**。

   ![](assets/configuration-for-existing-customers-5.png)

1. 单击 **[!UICONTROL New Remote Site]**。

   ![](assets/configuration-for-existing-customers-6.png)

1. 输入[!UICONTROL Remote Site Name]（可以是“MarketoRestAPI”之类的内容）和[!UICONTROL Remote Site URL]&#x200B;(Marketo中Rest API配置面板中的API URL)。

   ![](assets/configuration-for-existing-customers-7.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/configuration-for-existing-customers-8.png)

   您现在已为Rest API创建了远程站点设置。

## 访问Marketo Sales Insight {#access-marketo-sales-insight}

1. 从[!DNL Marketo’s Sales Insight]管理页面中的Rest API面板复制凭据。 将它们粘贴到Salesforce [!DNL Sales Insight]配置页面的Rest API部分中。

1. 输入[!UICONTROL API Secret Key]。

   ![](assets/configuration-for-existing-customers-9.png)
