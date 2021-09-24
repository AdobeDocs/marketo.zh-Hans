---
unique-page-id: 37355826
description: 发行说明 — 2020年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年2月
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 发行说明：’20年2月 {#release-notes-feb}

’20年2月版中包含以下功能。 查看您的Marketo版本以了解功能的可用性。

>[!AVAILABILITY]
>
>以星形(![(star)](assets/yellow-star.png))表示的功能是付费附加组件。 请联系您的Marketo Engage代表以了解更多信息。

**_季度_** 版本2020年2月21日发 **布了以下功能**。

## 核心Marketo Engage {#core-marketo-engage}

* **Microsoft Dynamics“在Microsoft中更改所有者”流程操作**:维护对Microsoft Dynamics CRM数据的控制，并能够直接从Marketo Engage更改潜在客户/联系所有者。这是对本机CRM集成功能的增强。
* **用户管理API**:通过外部身份和组织管理系统实现用户和角色管理自动化。这是对API调用功能的增强。
* **自定义对象架构API**:在Marketo Engage中跨实例自动管理和配置自定义对象架构，以使数据模型在销售和营销工具中保持一致。利用此API，您可以在沙盒或英才中心定义和测试自定义对象，并根据需要配置到任意数量的实例。 这是对API调用功能的增强。 请联系您的Marketo Engage代表以了解如何访问此增强功能。
* **登陆页面重定向规则API**:自动管理登陆页面重定向规则。这是对API调用功能的增强。
* **表单描述符缓存**:我们正在通过将表单缓存为资源来减少嵌入式表单的加载时间，并增强整体应用程序稳定性。请注意，对嵌入式表单的批准可能最多需要四分钟才能在Web上进行反映。 这是对登陆页面和Forms功能的增强。

<br> 

**_在整个季度发布_**

以下功能处于非季度周期，将在未来几个月内发布。

## Bizible {#bizible}

![（星号）](assets/yellow-star.png)

* **基于帐户的分段**:在帐户级别分析归因，并能够根据帐户属性为Discover展示板创建区段和过滤器。使用这些区段深入了解您基于帐户的营销效果。
* **保存过滤器**:保存每个用户特有的特定于功能板的过滤器，以便快速一致地分析功能板。
* **导出到PDF**:通过将Bizible功能板导出为PDF，在您的组织内共享有价值的分析。

## Sales Connect {#sales-connect}

* **撰写窗口更新**:我们简化了选择模板和通过Sales Connect发送电子邮件的流程。在我们的Web客户端中使用撰写窗口，在Salesforce中作为销售商的一站式商店，能够保存模板类别、计划电子邮件、批量发送电子邮件，以及通过查看和点击跟踪发送电子邮件。
* **命令中心更新**:我们正在重建Sales Connect命令中心，以便让销售者深入了解其从Sales Connect启动的所有电子邮件、呼叫和任务。他们还可以从指挥中心查看电子邮件参与度和投放能力等信息。

<br> 

## 公告 {#announcements}

* **Marketo Engage成功中心**:我们将于2020年2月启动Marketo成功中心。成功中心是一个产品内帮助中心，允许您直接从Marketo Engage实例中搜索产品文档和社区、启动操作指南、访问采用内容(如Marketo大学和同行最佳实践视频)等。 **注意**:此功能将作为测试版在澳新银行推出，并将在本季度晚些时候推出到北美。

## 弃用 {#deprecations}

* **资产API“_method”参数**:2020年9月之后，资产API端点将不再接受“_method”在POST正文中传递查询参数以绕过URI长度限制。为了适应需要此参数的请求，资产API的URI限制将从6KiB增加到65KiB，以便可以提交长请求URI。
* **弃用Internet Explorer支持**:从2020年7月31日发行的7月版开始，Internet Explorer将不再支持Marketo Engage用户界面。

**_产品发_** [行网络](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 研讨会在3月3日上午11:00PT / 2:00PM ET与我们一起参加由我们的产品团队主办的实时网络研讨会，并了解有关此版本中包含的功能的更多信息。
