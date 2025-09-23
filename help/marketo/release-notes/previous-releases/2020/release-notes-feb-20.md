---
unique-page-id: 37355826
description: 发行说明 — 2020年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年2月
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 2%

---

# 发行说明：2020 年 2 月 {#release-notes-feb}

2020年2月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![（星号）](assets/yellow-star.png))表示的功能是付费加载项。 请联系您的 Marketo Engage 代表了解更多信息。

**_季度发布_**&#x200B;以下功能发布于&#x200B;**2020年2月21日**。

## 核心Marketo Engage {#core-marketo-engage}

* **[!DNL Microsoft Dynamics]“在Microsoft中更改所有者”流程操作**：保持对[!DNL Microsoft Dynamics] CRM数据的控制，并能够直接从Marketo Engage更改潜在客户/联系所有者。 这是对我们的本机CRM集成功能的增强。
* **用户管理API**：通过外部标识和组织管理系统自动管理用户和角色。 这是对我们API调用功能的增强。
* **自定义对象架构API**：在Marketo Engage中跨实例自动管理和预配自定义对象架构，以保持销售和营销工具中的数据模型一致。 利用此API，您可以在沙盒或卓越中心中定义和测试自定义对象，并根据需要为任意数量的实例进行配置。 这是对我们API调用功能的增强。 请联系您的Marketo Engage代表以了解如何访问此增强功能。
* **登陆页面重定向规则API**：自动管理登陆页面重定向规则。 这是对我们API调用功能的增强。
* **表单描述符缓存**：我们将通过缓存表单作为资源来减少嵌入表单的加载时间并提高整体应用程序稳定性。 请注意，对嵌入式表单的批准可能最多需要4分钟才能反映在Web上。 这是对我们的登陆页面和Forms功能的增强。

<br> 

**_在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## [!DNL Bizible] {#bizible}

![（星形）](assets/yellow-star.png)

* **基于帐户的分段**：在帐户级别分析归因，能够根据帐户属性创建区段和筛选器以发现展示板。 使用这些区段可深入分析基于帐户的营销绩效。
* **保存筛选器**：保存每个用户特有的仪表板特定筛选器，以便快速一致地分析您的仪表板。
* **导出到PDF**：通过将Bizible功能板导出为PDF，可在您的组织内共享有价值的见解。

## [!DNL Sales Connect] {#sales-connect}

* **撰写窗口更新**：我们已简化通过[!DNL Sales Connect]选择模板和发送电子邮件的流程。 使用我们的Web客户端和Salesforce中的“撰写”窗口，可一站式查找销售者，并保存模板类别、计划电子邮件、批量发送电子邮件以及发送包含查看和点击跟踪的电子邮件。
* **命令中心更新**：我们正在重建[!DNL Sales Connect]命令中心，以便向销售商insight提供其从[!DNL Sales Connect]启动的所有电子邮件、呼叫和任务。 他们还可以从指挥中心查看电子邮件参与度和可投放性等信息。

<br> 

## 公告 {#announcements}

* **Marketo Engage成功中心**：我们将在2020年2月启动Marketo成功中心。 成功中心是一个产品内帮助中心，它允许您搜索产品文档和社区、启动操作指南、访问采用内容(如Marketo University和同事最佳实践视频)等，并直接从您的Marketo Engage实例中进行搜索。 **注意**：此功能将作为测试版在澳新银行推出，并将在本季度晚些时候推出到北美。

## 弃用 {#deprecations}

* **Asset API“_method”参数**： 2020年9月之后，Asset API端点将不再接受在POST正文中传递“_method”以绕过URI长度限制。 为了适应需要此参数的请求，资产API的URI限制将从6KiB增加到65KiB，以便可以提交较长的请求URI。
* **弃用Internet Explorer支持**：从2020年7月31日发行的7月版本开始，Internet Explorer将不再支持Marketo Engage用户界面。

**_产品发布网络研讨会_** [于3月3日（太平洋时间11](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) / 2:00AM ET）加入我们:00PM，参加我们产品团队举办的实时网络研讨会，并了解有关此版本中包含的功能的更多信息。
