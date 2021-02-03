---
unique-page-id: 11383953
description: 设置Facebook脱机转换- Marketo Docs —— 产品文档
title: 设置Facebook脱机转换
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# 设置Facebook脱机转换{#set-up-facebook-offline-conversions}

通过向Facebook发送线下转化数据，让通过Lead Ads创建的人群使用，您的广告团队可以比以往更好地优化其广告支出。 下面介绍如何设置。

>[!PREREQUISITES]
>
>* 您必须[设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)。
>* 您必须在[收入周期建模器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)中拥有已批准的模型。


## 管理员配置{#admin-configuration}

1. 转到Marketo **Admin**。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. 转至&#x200B;**LaunchPoint**&#x200B;并多次单击您之前创建的Facebook潜在客户广告服务。

   >[!NOTE]
   >
   >如果您还没有这样做，请继续[设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)，然后返回此处。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 如果需要，请编辑&#x200B;**显示名称**&#x200B;以包含脱机转换。 单击&#x200B;**下一步**。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 选中&#x200B;**启用脱机转换**，然后单击&#x200B;**下一步**。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 单击&#x200B;**下一步**。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   真贴心！ 您完成了启用Facebook脱机转换的一半。 让我们跳到收入周期建模器来映射各个阶段。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## 收入周期建模器配置{#revenue-cycle-modeler-configuration}

1. 转至&#x200B;**Analytics**。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. 选择您的模型，然后单击“编辑草稿”**。**

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >目前，有10个Facebook事件可以将收入周期阶段映射到：
   >
   >* 添加付款信息
   >* 添加到购物车
   >* 添加到愿望列表
   >* 注册已完成
   >* 已启动结帐
   >* 人物
   >* 其他
   >* 购买
   >* 搜索
   >* 内容视图


1. 选择要映射的阶段，然后从&#x200B;**Facebook Conversion**&#x200B;下拉框中，选择要将其映射到的Facebook事件。 重复此步骤，将RCM中的所有阶段映射到Facebook上的脱机转换阶段。

   ![](assets/1-1.png)

1. 完成映射后，关闭模型。

   ![](assets/2.png)

1. 批准您的模型，您就完成！

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   现在，当潜在客户广告潜在客户到达您映射的阶段时，转化会发送到Facebook以供报告。

   >[!CAUTION]
   >
   >检查您的Facebook帐户，并确保所有[广告都关联](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer)到“Marketo Offline Conversions”事件集。 如果不是，广告归因可能不起作用。

   >[!NOTE]
   >
   >脱机转换数据每天从Market发送多次到Facebook。

>[!MORELIKETHIS]
>
>[了解Facebook脱机转换](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
