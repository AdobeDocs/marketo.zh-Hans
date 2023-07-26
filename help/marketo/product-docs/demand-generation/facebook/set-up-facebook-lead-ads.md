---
unique-page-id: 11379622
description: 设置Facebook潜在客户广告 — Marketo文档 — 产品文档
title: 设置Facebook潜在客户广告
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 设置Facebook潜在客户广告 {#set-up-facebook-lead-ads}

使用 [facebook潜在客户广告](https://www.facebook.com/business/a/lead-ads) 在Facebook中运行广告营销活动并为Marketo生成潜在客户。

>[!NOTE]
>
>**需要管理员权限**

>[!AVAILABILITY]
>
>要将Facebook潜在客户广告添加到您的实例，请联系Adobe客户团队（您的客户经理）。

1. 转到Marketo **管理员**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到 **启动点**，单击 **新建，** 并选择 **新建服务**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 输入 **显示名称** 对于您的服务，选择 **facebook潜在客户广告** 服务，然后单击 **创建**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. 在同一浏览器中打开新选项卡，然后转到 [facebook.com](https://www.facebook.com). 使用要用于集成的帐户登录Facebook。

   >[!NOTE]
   >
   >facebook帐户将需要访问您要从中提取潜在广告的所有Facebook业务页面。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录Facebook后，请返回Marketo并单击 **授权**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. 如果出现提示，请单击 **确定** ，以接受将Marketo应用程序安装到Facebook中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您会发现您现在已获得授权。 单击 **下一个**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. 选择您希望Marketo从中提取Facebook潜在客户广告的页面，然后单击 **下一个**.

   >[!TIP]
   >
   >如果您没有看到预期的页面，请确保将用于身份验证的Facebook帐户已添加到Facebook上的该页面，然后重试。

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. 要接受默认的Facebook到Marketo字段映射，只需单击 **创建**.

   >[!TIP]
   >
   >通过修改映射，您可以自定义潜在客户广告数据在Marketo中的存储位置。 您还可以 [从潜在客户广告自定义问题中提取数据](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo不支持将两个Facebook字段映射到单个Marketo字段，仅支持从1到1。 如果将2映射到1，则潜在客户可能无法进入Marketo系统。

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   做得好！ 当您成功开展Marketo潜在客户广告营销活动时，潜在客户将开始流入Facebook。

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [在潜在客户访问管理器(Facebook)中分配/删除权限](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [在智能营销活动中使用潜在客户广告过滤器和触发器](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [将自定义字段映射到Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)
