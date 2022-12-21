---
unique-page-id: 11383945
description: 了解Facebook离线转化 — Marketo文档 — 产品文档
title: 了解Facebook离线转化
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 了解Facebook离线转化 {#understanding-facebook-offline-conversions}

Facebook商机广告促销活动会生成商机，并将它们发送到Marketo，以用于营销活动。 但是，如果无法查看离线转化，Facebook广告商就无法知道哪些广告最有效。 以下是一个示例。

>[!NOTE]
>
>**示例**
>
>Facebook Lead Ads运行三个广告。
>
>* 广告1生成20个潜在客户
>* 广告2生成30个潜在客户
>* 广告3生成50个潜在客户
>
>仅根据这些数字，第3条似乎最有效。
>
>但是，在Marketo一侧查看数据时，情况却有所不同。
>
>* 广告1生成10个销售
>* 广告3生成2个销售
>
>这意味着，广告1尽管产生的线索较少，但其成功率为50%，而广告3根本起不到任何作用。
>
>如果没有离线转化，广告商可能会在广告3上投入更多资金。 有了离线转化数据，广告商更有可能投资于广告1。

您可以 [设置Facebook离线转化](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) 将离线广告效果发送到Facebook。

1. 确保 [Facebook LaunchPoint集成](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) 是最新的。
1. 在Facebook上将收入周期模型中的阶段映射到离线转化阶段。
1. 当从Facebook潜在客户广告生成Facebook潜在客户并到达映射的阶段时，Marketo会通过安全、自动化的API每天多次将离线转化数据发送回Facebook。 数据会显示在Facebook广告管理器报表中。

>[!MORELIKETHIS]
>
>[设置Facebook离线转化](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
