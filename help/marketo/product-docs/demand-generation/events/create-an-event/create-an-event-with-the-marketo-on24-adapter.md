---
unique-page-id: 10096656
description: 使用Marketo ON24适配器创建事件- Marketo文档——产品文档
title: 使用Marketo ON24适配器创建事件
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# 使用Marketo ON24适配器{#create-an-event-with-the-marketo-on-adapter}创建事件

## 开始前{#before-you-begin}

您应该熟悉构建基块以及在Marketo中创建事件的推荐顺序。 您还应具备以下Marketo概念的工作知识：

* [Marketo Programs](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) 和事件，以及它们之间的区别
* [渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [本地资产](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [子营销](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) 活动和 [项目状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>有关Marketo API的详细信息，请参阅[Marketo API文档](https://developers.marketo.com/documentation/rest/)。

## 先决条件{#prerequisites}

使用Marketo ON24集成需要以下各项：

* **订阅到ON24 Webcast**  —— 如果您没有当前订阅，请直接与ON24联系。**注意**:需要ON24 Hosted Edition。无需ON24事件管理。

* **对ON24的管理员权** 限——您需要此权限才能使用此连接器并在ON24系统中创建客人。
* **ON24连接凭据** -您需要在Market中输入此信息才能启用集成：用户名、密码、客户端ID和客户端密钥。如果您需要有关凭据的帮助，请与您的ON24客户经理或ON24支持联系。
* **注册表单** -使用Marketo表单或非Marketo表单以及正确的API，确保注册数据和注册者信息被传递到Marketo。
* **注册子活动** -必须正确创建和配置Marketo事件中的注册子活动，以使事件合作伙伴集成正常工作。

## 进程流{#process-flow}

按照以下步骤使用Marketo On24适配器创建事件:

1. [在Marketo中输入您的ON24凭据](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [在ON24中创建网络研讨会事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [配置事件设置并将营销人员同步到网络研讨会](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [创建子活动和本地资产](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [测试ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [示例ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [了解网络研讨会项目状态](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [ON24事件注册更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
