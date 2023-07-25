---
unique-page-id: 37355826
description: 发行说明 — 2020年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年2月
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 发行说明： 2020年2月 {#release-notes-feb}

2020年2月版中包括以下功能。 查看Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号( ![(star)](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_** 以下功能发布于 **2020年2月21日**.

## 核心Marketo Engage {#core-marketo-engage}

* **Microsoft Dynamics“在Microsoft中更改所有者”流程操作**：保持对Microsoft Dynamics CRM数据的控制，并允许直接从Marketo Engage中更改潜在客户/联系所有者。 这是对我们的本机CRM集成功能的增强。
* **用户管理API**：通过外部身份和组织管理系统自动管理用户和角色。 这是对我们API调用功能的增强。
* **自定义对象架构API**：在Marketo Engage的实例间自动管理和配置自定义对象架构，以使您的销售和营销工具中的数据模型保持一致。 通过此API，您可以在沙盒或卓越中心中定义和测试自定义对象，并根据需要为任意数量的实例进行配置。 这是对我们API调用功能的增强。 请联系您的Marketo Engage代表以了解如何访问此增强功能。
* **登陆页面重定向规则API**：自动管理登陆页面重定向规则。 这是对我们API调用功能的增强。
* **表单描述符缓存**：我们通过将表单缓存为资源来缩短嵌入表单的加载时间并增强整体应用程序稳定性。 请注意，对嵌入式表单的批准可能最多需要4分钟才能反映在Web上。 这是对我们的登陆页面和Forms功能的增强。

<br> 

**_整个季度发布_**

以下功能属于非季度周期，将在未来几个月发布。

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **基于帐户的分段**：分析帐户级别的归因，并能够创建区段和过滤器，以根据帐户属性发现展示板。 使用这些区段可深入了解基于帐户的营销绩效。
* **保存筛选器**：保存每个用户特有的功能板特定过滤器，以便快速、一致地分析您的功能板。
* **导出到PDF**：通过将Bizible功能板导出为PDF，可在您的组织中共享有价值的见解。

## Sales Connect {#sales-connect}

* **撰写窗口更新**：我们简化了通过Sales Connect选择模板和发送电子邮件的流程。 在我们的Web客户端和Salesforce中使用“撰写”窗口作为销售人员的一站式商店，可以保存模板类别、计划电子邮件、批量发送电子邮件以及发送包含查看和点击跟踪的电子邮件。
* **命令中心更新**：我们正在重建Sales Connect指挥中心，以便让销售人员深入了解他们从Sales Connect发起的所有电子邮件、致电和任务。 他们还可以从指挥中心查看电子邮件参与度和可投放性等信息。

<br> 

## 公告 {#announcements}

* **Marketo Engage成功中心**：我们将于2020年2月启动Marketo成功中心。 Success Center是一个产品内帮助中心，它允许您搜索产品文档和社区、启动操作指南、访问采用内容(如Marketo University和同事最佳实践视频)等，以及直接从您的Marketo Engage实例中进行搜索。 **注释**：此功能将作为测试版在澳新银行推出，并将在本季度晚些时候推出到北美洲。

## 弃用 {#deprecations}

* **资产API“_method”参数**： 2020年9月之后，Asset API端点将不再接受“_method”在POST正文中传递查询参数以绕过URI长度限制。 为了适应需要此参数的请求，资产API的URI限制将从6KiB增加到65KiB，以便可以提交长请求URI。
* **弃用Internet Explorer支持**：从2020年7月31日发行的7月版本开始，Internet Explorer将不再支持Marketo Engage用户界面。

**_产品发布网络研讨会_** [加入我们](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 3月3日上午11:00（太平洋时间）/下午2:00（东部时间），参加由我们的产品团队主持的直播网络研讨会，并了解有关此版本中包含的功能的更多信息。
