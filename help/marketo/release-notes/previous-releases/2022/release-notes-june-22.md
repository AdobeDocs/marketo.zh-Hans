---
description: 发行说明 — 2022年6月 — Marketo文档 — 产品文档
title: 发行说明 - 2022 年 6 月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 6%

---

# 发行说明：2022 年 6 月 {#release-notes-june-22}

在下方，您会找到2022年6月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

以下功能将于&#x200B;**2022年6月24日**&#x200B;开始发布，并在接下来的几周内分阶段推出剩余功能（除非另有说明）。

## 营销数据环境 {#marketing-data-environment}

* **公开自定义对象的CreatedAt/UpdatedAt字段**：让您能够在“人员详细信息”屏幕中检查这些字段，以获取额外的insight。

## 跨渠道编排 {#cross-channel-orchestration}

* **已改进[!DNL Dynamic Chat]**&#x200B;的流Designer可用性：无需拖放，即可直接从Designer流画布添加信息卡。 [!DNL Dynamic Chat]界面也已得到改进，可更好地显示各个信息卡中的内容。

* **的[!DNL Dynamic Chat]**&#x200B;高级约会路由规则： [!DNL Dynamic Chat]为目标约会路由提供了更多选项。 指定应根据Marketo Engage属性路由哪些座席约会，确保将潜在客户路由到适当的座席。

* **适用于[!DNL Dynamic Chat]**&#x200B;的高级对话框报表：使用参与和转化量度的全新数据可视化图表，更详细地查看[!DNL Dynamic Chat]营销活动的性能。

* **取消同步[!DNL Dynamic Chat]**&#x200B;的未使用Marketo Engage属性：取消同步未使用的[!DNL Dynamic Chat]订阅中的Marketo Engage属性，这有助于促进数据清理，并可以根据需要同步替代属性。

## 下一代体验

**新的切换开关视图**：以下视图现在可在下一代体验中使用：

* [电子邮件详细信息视图](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [电子邮件列表视图](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## 体验自动化 {#experience-automation}

* **全局表单字段验证规则排除**：从全局表单验证规则中排除特定表单，以便订阅中心和其他关键业务工作流可以接受所有值。

* **自助流程步骤**：扩展Marketo Engage与栈栈其他部分之间的连接，并能够创作自定义流程步骤以用于Smart Campaigns。 Marketo Engage用户和合作伙伴都可以利用此功能，允许在“触发器”、“批处理”和“可执行”营销活动中使用外部Web服务，而相比之下，Webhook只能在“触发器”营销活动中使用。

* **与Munchkin协议无关的链接跟踪**：通过Munchkin扩展对`tel`和`mailto`链接的跟踪支持，以跟踪扩展的Web行为集。

* **Webhook的其他HTTP方法**：将PUT、PATCH和DELETE指定为请求类型，以便与Web服务交互。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[!DNL Sales Insight]在[!DNL Salesforce]**&#x200B;中设置的权限：管理员可以通过Marketo应用程序权限集向用户级别上的有限用户集合提供[!DNL Sales Insight]访问权限，而不是配置文件级别上的有限用户集合，该权限集是[!DNL Sales Insight] [!DNL Salesforce]包的一部分。

* **我的Marketo拼贴更新 — [!DNL Sales Insight]操作**： Marketo管理员（以及他们指定的用户）现在可以通过位于“我的Marketo”页面上的新[!DNL Sales Insight]操作拼贴快速导航到他们的[!DNL Sales Insight]操作实例。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **[!DNL Salesforce]API更新**：在[!DNL Salesforce]夏季&#39;22版本中，[!DNL Salesforce]将不再支持API旧版本21 -30。 在此Marketo Engage版本中，使用旧版API的所有[!DNL Sales Connect]请求都已更新，以保持在支持的版本中。 有关[!DNL Salesforce] API弃用计划的完整详细信息，请单击[此处](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}。

## API增强功能 {#api-enhancements}

* **批量程序成员提取API的新筛选功能**：按程序成员资格状态、updatedAt、cadence或用完的内容进行筛选，以优化提取的数据集。

* **批量程序成员提取API改进**：在创建作业期间指定最多10个程序以提高吞吐量。

## 公告 {#announcements}

* **Forms弃用 — Forms 1.0、潜在客户捕获/保存端点以及Forms**&#x200B;的无脚本版本：到2022年10月，将从Marketo Engage中完全移除对Forms 1.0资源的支持。 所有现有的Forms 1.0资源都将停止运行。 Marketo Engage表单将要求在登陆页面和网站上加载JavaScript。

**_产品发布网络研讨会_**

[2022年6月和8月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
