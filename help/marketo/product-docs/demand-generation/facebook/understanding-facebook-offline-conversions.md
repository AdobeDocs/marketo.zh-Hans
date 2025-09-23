---
unique-page-id: 11383945
description: 了解Facebook离线转化 — Marketo文档 — 产品文档
title: 了解 Facebook 离线转化
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 2%

---

# 了解[!DNL Facebook]离线转化 {#understanding-facebook-offline-conversions}

Facebook商机广告营销活动会生成商机并将它们发送到Marketo以用于营销活动。 但是，如果看不到离线转化，[!DNL Facebook]广告商将无法知道哪些广告最有效。 下面是一个示例。

>[!NOTE]
>
>**示例**
>
>[!UICONTROL Facebook Lead Ads]运行三个广告。
>
>* 广告1生成20个潜在客户
>* 广告2会产生30个潜在客户
>* 广告3会产生50个潜在客户
>
>仅从这些数字来看，广告3似乎最有效。
>
>但是，从Marketo方面来看，情况则截然不同。
>
>* 广告1产生10个销售额
>* 广告3产生2个销售
>
>这意味着，广告1尽管产生的潜在客户较少，但成功率为50%，而广告3几乎毫无效果。
>
>如果没有离线转化，广告商可能会在Ad 3上投入更多资金。 有了离线转化数据，广告商更有可能投资于广告1。

您可以[设置Facebook离线转化](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)以将离线广告性能发送到[!DNL Facebook]。

1. 确保您的[[!DNL Facebook] [!UICONTROL LaunchPoint]集成](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md)是最新的。
1. 将收入周期模型中的阶段映射到[!DNL Facebook]上的离线转化阶段。
1. 当从[!DNL Facebook]潜在客户广告生成[!DNL Facebook]潜在客户并到达映射阶段时，Marketo每天都会通过安全、自动的API将离线转化数据发送回[!DNL Facebook]多次。 该数据显示在[!DNL Facebook]广告管理器报表中。

>[!MORELIKETHIS]
>
>[设置 [!DNL Facebook] 脱机转换](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
