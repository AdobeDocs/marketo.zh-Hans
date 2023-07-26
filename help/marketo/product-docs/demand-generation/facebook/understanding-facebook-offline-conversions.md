---
unique-page-id: 11383945
description: 了解Facebook离线转化 — Marketo文档 — 产品文档
title: 了解Facebook离线转化
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 了解Facebook离线转化 {#understanding-facebook-offline-conversions}

facebook潜在客户广告营销活动可生成潜在客户并将它们发送到Marketo以用于营销活动。 但是，如果看不到离线转化，Facebook广告商就无法知道哪些广告最有效。 下面是一个示例。

>[!NOTE]
>
>**示例**
>
>facebook潜在客户广告运行三个广告。
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

您可以 [设置Facebook离线转化](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) 将离线广告效果发送到Facebook。

1. 确保 [facebook LaunchPoint集成](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) 是最新的。
1. 将收入周期模型中的阶段映射到Facebook上的离线转化阶段。
1. 当从Facebook Lead广告生成Facebook Lead并到达映射阶段时，Marketo每天都会通过安全、自动的API将离线转化数据发送回Facebook多次。 数据显示在Facebook广告管理器报表中。

>[!MORELIKETHIS]
>
>[设置Facebook离线转化](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
