---
unique-page-id: 42762519
description: 现有客户的配置 — Marketo文档 — 产品文档
title: 现有客户的配置
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 现有客户的配置 {#configuration-for-existing-customers}

请设置以下配置以开始使用新的分析仪表板。

>[!PREREQUISITES]
>
>请确保已将Salesforce包升级到最新版本

## 在Marketo中配置Sales Insight {#configure-sales-insight-in-marketo}

1. 在浏览器中打开新选项卡，以从您的Marketo帐户获取Marketo销售分析凭据。

1. 转到 **管理员** 区域。

   ![](assets/configuration-for-existing-customers-1.png)

1. 单击 **销售分析**.

   ![](assets/configuration-for-existing-customers-2.png)

1. 单击 **视图** 以填充Rest API凭据。

   ![](assets/configuration-for-existing-customers-3.png)

1. 您将会看到确认弹出窗口。 单击 **确定**.

## 在Salesforce中配置Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击 **设置**.

   ![](assets/configuration-for-existing-customers-4.png)

1. 搜索并选择 **远程站点设置**.

   ![](assets/configuration-for-existing-customers-5.png)

1. 单击 **新建远程站点**.

   ![](assets/configuration-for-existing-customers-6.png)

1. 输入远程站点名称（可以类似于“MarketoRestAPI”）和远程站点URL(您在Marketo的“Rest API配置”面板中的API URL)。

   ![](assets/configuration-for-existing-customers-7.png)

1. 单击 **保存**.

   ![](assets/configuration-for-existing-customers-8.png)

   您现在已为Rest API创建了远程站点设置。

## 访问Marketo Sales Insight {#access-marketo-sales-insight}

1. 从Marketo的“Sales Insight管理”页面的“Rest API”面板中复制凭据。 将它们粘贴到Salesforce的Sales Insight配置页面的Rest API部分中。

1. 输入API密钥。

   ![](assets/configuration-for-existing-customers-9.png)
