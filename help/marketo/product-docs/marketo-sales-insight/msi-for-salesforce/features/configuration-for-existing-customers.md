---
unique-page-id: 42762519
description: 现有客户的配置 — Marketo Docs — 产品文档
title: 现有客户的配置
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---


# 现有客户{#configuration-for-existing-customers}的配置

请设置以下配置，以开始使用新的“分析”仪表板。

>[!PREREQUISITES]
>
>请确保已将您的Salesforce包升级到最新版本

## 在Marketo {#configure-sales-insight-in-marketo}中配置Sales Insight

1. 在您的浏览器中打开新选项卡，从您的Marketo帐户获取Marketo Sales Insights凭据。

1. 转至&#x200B;**Admin**&#x200B;区域。

   ![](assets/configure-1.png)

1. 单击&#x200B;**Sales Insight**。

   ![](assets/configure-2.png)

1. 单击&#x200B;**视图**&#x200B;以填充Rest API凭据。

   ![](assets/configure-3.png)

1. 您将看到确认弹出窗口。 单击&#x200B;**确定**。

## 在Salesforce中配置Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击&#x200B;**Setup**。

   ![](assets/sfdc-1.png)

1. 搜索并选择&#x200B;**远程站点设置**。

   ![](assets/sfdc-2.png)

1. 单击&#x200B;**新建远程站点**。

   ![](assets/sfdc-3.png)

1. 输入远程站点名称（可以是类似“MarketoRestAPI”）和远程站点URL（Marketo中“Rest API配置”面板中的API URL）。

   ![](assets/sfdc-4.png)

1. 单击&#x200B;**保存**。

   ![](assets/sfdc-5.png)

   您现在已为Rest API创建远程站点设置。

## 访问Marketo Sales Insight {#access-marketo-sales-insight}

1. 从Marketo的Sales Insight Admin页面的Rest API面板复制凭据。 将它们粘贴到Salesforce的“Sales Insight配置”页面的Rest API部分。

1. 输入API密钥。

   ![](assets/config.png)
