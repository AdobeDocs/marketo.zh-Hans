---
unique-page-id: 10096656
description: 使用Marketo ON24适配器创建事件 — Marketo文档 — 产品文档
title: 使用Marketo ON24适配器创建事件
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 使用Marketo ON24适配器创建事件 {#create-an-event-with-the-marketo-on-adapter}

>[!IMPORTANT]
>
>自2022年8月起，ON24不再支持新的Marketo集成。 本文中的信息仅适用于现有用户。

您应该熟悉在Marketo中创建事件的构建基块和推荐的顺序。 您还应了解以下Marketo概念：

* [Marketo计划](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) 以及事件，以及它们之间的差异
* [渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [本地资产](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [子营销活动](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) 和 [项目状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>请参阅 [Marketo API文档](https://developers.marketo.com/documentation/rest/) 有关Marketo API的更多信息。

## 先决条件 {#prerequisites}

使用Marketo ON24集成需要满足以下条件：

* **订购ON24网络广播**  — 如果您当前没有订阅，请直接与ON24联系。 **注意**:需要ON24托管版。 ON24事件管理不是必需的。

* **ON24的管理员权限**  — 使用此连接器并在ON24系统中创建来宾时需要此连接器。
* **ON24连接凭据**  — 您需要在Marketo中输入以下信息才能启用集成：用户名、密码、客户端ID和客户端密钥。 如果您需要凭据方面的帮助，请联系您的ON24客户经理或ON24支持。
* **注册表**  — 使用Marketo表单或非Marketo表单以及适当的API，以确保将注册数据和注册信息传递到Marketo。
* **注册子营销活动**  — 必须正确创建和配置Marketo事件中的注册子营销活动，以便事件合作伙伴集成正常工作。

## 流程 {#process-flow}

按照以下步骤使用Marketo On24适配器创建事件：

1. [在ON24中创建网络研讨会活动](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [配置事件设置并将Marketo与网络研讨会同步](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [创建子营销活动和本地资产](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [测试ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [ON24事件集成示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [了解网络研讨会计划状态](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [ON24事件注册更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
