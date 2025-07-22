---
unique-page-id: 11383953
description: 设置Facebook离线转化 — Marketo文档 — 产品文档
title: 设置Facebook离线转化
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# 设置[!DNL Facebook]脱机转换 {#set-up-facebook-offline-conversions}

通过将离线转化数据发送回[!DNL Facebook] （针对通过潜在客户广告创建的人员），您的广告团队可以比以往更好地优化其广告支出。 下面是设置方法。

>[!PREREQUISITES]
>
>* 您必须[设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)。
>* 您在[收入周期Modeler](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)中必须具有已批准的模型。

## 管理员配置 {#admin-configuration}

1. 转到Marketo **[!UICONTROL Admin]**。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. 转到&#x200B;**[!UICONTROL LaunchPoint]**&#x200B;并双击您之前创建的Facebook潜在客户广告服务。

   >[!NOTE]
   >
   >如果您尚未执行该操作，请继续[设置[!UICONTROL Facebook Lead Ads]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)，然后返回此处。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 需要时可编辑&#x200B;**[!UICONTROL Display Name]**&#x200B;以包含离线转化。 单击 **[!UICONTROL Next]**。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 检查&#x200B;**[!UICONTROL Enable Offline Conversions]**&#x200B;并单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   真贴心！ 您已经完成启用[!DNL Facebook]离线转换。 让我们跳转到收入周期Modeler以映射阶段。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Revenue Cycle Modeler配置 {#revenue-cycle-modeler-configuration}

1. 转到&#x200B;**[!UICONTROL Analytics]**。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. 选择您的模型并单击&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >目前，有10个[!DNL Facebook]事件可以将收入周期阶段映射到：
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

1. 选择要映射的阶段，然后从&#x200B;**[!UICONTROL Facebook Conversion]**&#x200B;下拉列表中，选择要将其映射到的[!DNL Facebook]事件。 重复此步骤以将RCM中的所有阶段映射到[!DNL Facebook]上的脱机转换阶段。

   ![](assets/1-1.png)

1. 完成映射后，关闭模型。

   ![](assets/2.png)

1. 批准您的模型即告完成！

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   现在，当潜在客户广告商机达到您映射的阶段时，转化将发送到[!DNL Facebook]进行报告。

   >[!CAUTION]
   >
   >检查您的[!DNL Facebook]帐户，并确保所有[广告都与Marketo离线转化事件集关联](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&cmsid&creative=link&creative_detail=advertiser-help-center&create_type&destination_cms_id&orig_http_referrer)。 如果它们无效，则广告归因可能无效。

   >[!NOTE]
   >
   >离线转化数据每天从Marketo发送至[!DNL Facebook]多次。

>[!MORELIKETHIS]
>
>[了解 [!DNL Facebook] 脱机转换](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
