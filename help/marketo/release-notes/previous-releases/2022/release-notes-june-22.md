---
description: 发行说明 — 2022年6月 — Marketo文档 — 产品文档
title: 发行说明 — 2022年6月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# 发行说明： 2022年6月 {#release-notes-june-22}

在下方，您会找到2022年6月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

以下功能将于&#x200B;**2022年6月24日**&#x200B;开始发布，并在接下来的几周内分阶段推出剩余功能（除非另有说明）。

## 营销数据环境 {#marketing-data-environment}

* **公开自定义对象的CreatedAt/UpdatedAt字段**：让您能够在“人员详细信息”屏幕中检查这些字段，以获得更多见解。

## 跨渠道编排 {#cross-channel-orchestration}

* **已改进Dynamic Chat的流Designer可用性**：无需拖放，即可直接从Designer流画布添加信息卡。 Dynamic Chat界面也得到了改进，可更好地显示各个信息卡中的内容。

* **Dynamic Chat的高级约会路由规则**：Dynamic Chat为目标约会路由提供了更多选项。 指定应根据Marketo Engage属性路由哪些座席约会，确保将潜在客户路由到适当的座席。

* **Dynamic Chat的高级对话框报表**：使用参与和转化指标的全新数据可视化图表，更详细地查看Dynamic Chat促销活动的性能。

* **取消同步Dynamic Chat的未使用Marketo Engage属性**：取消同步未使用的Dynamic Chat订阅中的Marketo Engage属性，这有助于提高数据清洁度并允许根据需要同步替代属性。

## 下一代体验

**新的切换开关视图**：以下视图现在可在下一代体验中使用：

* [电子邮件详细信息视图](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [电子邮件列表视图](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## 体验自动化 {#experience-automation}

* **全局表单字段验证规则排除**：从全局表单验证规则中排除特定表单，以便订阅中心和其他关键业务工作流可以接受所有值。

* **自助流程步骤**：扩展Marketo Engage与栈栈其余部分之间的连接，能够创作自定义流程步骤以用于Smart Campaigns。 Marketo Engage用户和合作伙伴都可以利用此功能，允许在“触发器”、“批处理”和“可执行”营销活动中使用外部Web服务，而相比之下，Webhook只能在“触发器”营销活动中使用。

* **Munchkin协议无关链接跟踪**：扩展对使用Munchkin跟踪`tel`和`mailto`链接的支持，以跟踪扩展的Web行为集。

* **Webhook的其他HTTP方法**：将PUT、PATCH和DELETE指定为与Web服务交互的请求类型。

## 销售分析 {#sales-insight}

![（星形）](assets/yellow-star.png)

* **在Salesforce中设置了Sales Insight权限**：管理员可以通过作为Sales Insight Salesforce包一部分的Marketo应用程序权限集，向用户级别上有限的一组人员提供Sales Insight访问权限，而不是个人资料级别上的权限。

* **我的Marketo图块更新 — Sales Insight操作**： Marketo管理员（以及他们指定的用户）现在可以通过位于“我的Marketo”页面上的新Sales Insight Actions图块，快速导航到他们的Sales Insight Actions实例。

## Sales Connect {#sales-connect}

![（星形）](assets/yellow-star.png)

* **Salesforce API更新**：随着Salesforce 22年夏季版的发布，Salesforce将不再支持API旧版本21 -30。 在此Marketo Engage版本中，所有使用旧版API的Sales Connect请求都已更新，以保持在一个受支持的版本中。 有关Salesforce API弃用计划的完整详细信息，请单击[此处](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}。

## API增强功能 {#api-enhancements}

* **批量程序成员提取API的新筛选功能**：按程序成员资格状态、updatedAt、cadence或用完的内容进行筛选，以优化提取的数据集。

* **批量程序成员提取API改进**：在创建作业期间指定最多10个程序以提高吞吐量。

## 公告 {#announcements}

* **Forms弃用 — Forms 1.0、潜在客户捕获/保存端点以及forms**&#x200B;的无脚本版本：到2022年10月，对Forms 1.0资源的支持将从Marketo Engage中完全删除。 所有现有的Forms 1.0资源都将停止运行。 Marketo Engage表单将要求在登陆页面和网站上加载JavaScript。

**_产品发布网络研讨会_**

[2022年6月和8月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
