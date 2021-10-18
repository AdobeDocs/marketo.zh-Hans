---
unique-page-id: 11383953
description: 设置Facebook离线转化 — Marketo文档 — 产品文档
title: 设置Facebook离线转化
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 设置Facebook离线转化 {#set-up-facebook-offline-conversions}

通过将离线转化数据发送回Facebook，以供通过潜在客户广告创建的人员使用，您的广告团队可以比以往任何时候都优化其广告支出。 下面是如何设置它。

>[!PREREQUISITES]
>
>* 您必须 [设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* 您必须在 [收入周期建模器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).


## 管理员配置 {#admin-configuration}

1. 转到Marketo **管理员**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. 转到 **LaunchPoint** 并双击您之前创建的Facebook潜在客户广告服务。

   >[!NOTE]
   >
   >如果你还没做，那就去 [设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)，然后回来。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 如果需要，请编辑 **显示名称** 以包含离线转化。 单击 **下一个**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 检查 **启用离线转化** 单击 **下一个**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 单击 **下一个**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 单击 **保存**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   真贴心！ 启用Facebook离线转化的过程已完成一半。 让我们跳转到收入周期建模器以映射各个阶段。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## 收入周期建模器配置 {#revenue-cycle-modeler-configuration}

1. 转到 **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. 选择模型并单击 **编辑草稿**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >目前，有10个Facebook事件可以将收入周期阶段映射到：
   >
   >* 添加付款信息
   >* 添加到购物车
   >* 添加到愿望列表
   >* 已完成注册
   >* 已启动结帐
   >* 人员
   >* 其他
   >* 购买
   >* 搜索
   >* 内容查看


1. 选择要映射的舞台，然后从 **Facebook转化** 下拉列表，选择要将其映射到的Facebook事件。 重复此步骤，将RCM中的所有阶段映射到Facebook上的离线转化阶段。

   ![](assets/1-1.png)

1. 完成映射后，关闭模型。

   ![](assets/2.png)

1. 批准模型，就完成！

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   现在，当潜在客户到达您映射的阶段时，转化会发送到Facebook以进行报告。

   >[!CAUTION]
   >
   >检查您的Facebook帐户，并确保 [广告关联](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) 到Marketo离线转化事件集。 如果它们不可用，则广告归因可能无法正常工作。

   >[!NOTE]
   >
   >离线转化数据每天从Marketo多次发送到Facebook。

>[!MORELIKETHIS]
>
>[了解Facebook离线转化](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
