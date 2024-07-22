---
unique-page-id: 11383953
description: 设置Facebook离线转化 — Marketo文档 — 产品文档
title: 设置Facebook离线转化
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 1%

---

# 设置Facebook离线转化 {#set-up-facebook-offline-conversions}

通过将离线转化数据发送回Facebook以吸引通过潜在客户广告创建的用户，您的广告团队可以比以往更好地优化其广告支出。 下面是设置方法。

>[!PREREQUISITES]
>
>* 您必须[设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)。
>* 您在[收入周期Modeler](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)中必须具有已批准的模型。

## 管理员配置 {#admin-configuration}

1. 转到Marketo **管理员**。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. 转到&#x200B;**LaunchPoint**&#x200B;并双击您之前创建的Facebook潜在客户广告服务。

   >[!NOTE]
   >
   >如果您尚未这样做，请继续[设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)，然后返回此处。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 如果需要，请编辑&#x200B;**显示名称**&#x200B;以包含离线转化。 单击&#x200B;**下一步**。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 选中&#x200B;**启用脱机转换**，然后单击&#x200B;**下一步**。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 单击&#x200B;**下一步**。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   真贴心！ 您已经完成了启用Facebook离线转换的步骤。 让我们跳转到收入周期Modeler以映射阶段。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Revenue Cycle Modeler配置 {#revenue-cycle-modeler-configuration}

1. 转到&#x200B;**Analytics**。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. 选择您的模型并单击&#x200B;**编辑草稿**。

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >目前，有10个Facebook事件可将收入周期阶段映射到：
   >
   >* 添加付款信息
   >* 添加到购物车
   >* 添加到愿望清单
   >* 注册已完成
   >* 已启动结帐
   >* 人员
   >* 其他
   >* 购买
   >* 搜索
   >* 内容查看

1. 选择要映射的阶段，然后从&#x200B;**Facebook转化**&#x200B;下拉列表中，选择要将其映射到的Facebook事件。 重复此步骤以将RCM中的所有阶段映射到Facebook上的离线转化阶段。

   ![](assets/1-1.png)

1. 完成映射后，关闭模型。

   ![](assets/2.png)

1. 批准您的模型即告完成！

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   现在，当潜在客户广告商机达到您映射的阶段时，转化率将发送到Facebook进行报告。

   >[!CAUTION]
   >
   >检查您的Facebook帐户，并确保所有[广告均已关联](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer)到Marketo离线转化事件集。 如果它们无效，则广告归因可能无效。

   >[!NOTE]
   >
   >离线转化数据每天会从Marketo发送到Facebook多次。

>[!MORELIKETHIS]
>
>[了解Facebook脱机转换](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
