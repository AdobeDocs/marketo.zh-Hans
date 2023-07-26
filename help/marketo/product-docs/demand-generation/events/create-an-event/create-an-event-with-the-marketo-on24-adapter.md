---
unique-page-id: 10096656
description: 使用Marketo ON24适配器创建事件 — Marketo文档 — 产品文档
title: 使用Marketo ON24适配器创建事件
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# 使用Marketo ON24适配器创建事件 {#create-an-event-with-the-marketo-on-adapter}

您应该熟悉构建基块以及在Marketo中创建事件的推荐顺序。 您还应具有以下Marketo概念的工作知识：

* [Marketo项目](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} 以及事件和它们之间的差异
* [渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [本地资产](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [子营销活动](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} and [Program Statuses](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>请参阅 [Marketo API文档](https://developers.marketo.com/documentation/rest/){target="_blank"} 有关Marketo API的更多信息。

## 先决条件 {#prerequisites}

要使用Marketo ON24集成，需要满足以下条件：

* **订购ON24网络广播**  — 如果当前没有订阅，请直接与ON24联系。 **注意**：需要ON24 Hosted Edition。 不需要ON24事件管理。

* **ON24的管理员权限**  — 您需要此连接器才能在ON24系统中使用此连接器并创建来宾。
* **ON24连接凭据**  — 您需要在Marketo中输入以下信息才能启用集成：用户名、密码、客户端ID和客户端密钥。 如果您需要有关凭据的帮助，请联系您的ON24客户经理或ON24支持。
* **注册表单**  — 使用Marketo表单或非Marketo表单以及适当的API，以确保注册数据和注册者信息传递到Marketo。
* **注册子营销活动**  — 必须正确创建和配置Marketo事件中的注册子营销活动，才能使事件合作伙伴集成正常工作。

## 处理流程 {#process-flow}

执行以下步骤，使用Marketo On24适配器创建事件：

1. [在ON24中创建网络研讨会活动](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [配置事件设置并将Marketo与您的网络研讨会同步](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [创建子营销活动和本地资源](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [测试ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [ON24事件集成示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [了解网络研讨会计划状态](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [ON24事件注册更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
