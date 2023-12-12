---
description: 在智能列表触发器和过滤器中使用Vibes SMS消息 — Marketo文档 — 产品文档
title: 在智能列表触发器和过滤器中使用Vibes SMS消息
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 6b8c54dbe95c7bc6e2f68a48de11306f3f678cb6
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 在智能列表触发器和过滤器中使用Vibes SMS消息 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

新建文档

在您之后 [创建短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}，您将需要在Smart Campaign中使用智能列表触发器和过滤器以获取好处。 具体方法如下。

1. 在“我的Marketo”中，单击 **营销活动**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. 选择您要使用短信资产的智能营销活动。 拖动到触发器上。 在此示例中，我们使用 **填写表单**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS触发器 {#sms-triggers}

还有其他可用的短信触发器。 仅当启用了Vibes服务时，才会显示SMS触发器。

发送短信消息：

* 营销活动>选择新建智能营销活动
   * 智能列表>选择受众列表过滤器和正确逻辑>受众列表：从下拉列表（从Vibes平台同步的移动设备数据库列表）中选择列表
      * 可以优化分段并利用短信和电子邮件过滤器以及同一营销活动中的触发器
      * Vibes Filters： Subscribed to Vibes List vs. Member of Vibes List — 逻辑与电子邮件一致
         * 已订阅的Vibes列表 — 已订阅该Vibes列表的参与者，即使现在已取消订阅。   — 主要用于跨渠道营销工作
            * 注意：如果任何未订阅的用户不在Vibes移动数据库列表中，则不会向其发送短信消息
         * Vibes列表的成员 — 已确认的活动订阅者
         * 已添加到列表 — 访客列表不会填充此过滤器；这适用于Marketo列表

![](assets/new-sms-search2.png)

下面是一些示例：

此 **短信消息退回** 当短信消息退回时，触发器会启动流程，例如发送电子邮件。

![](assets/sms-message-bounces-real.jpg)

此 **Vibes列表的订阅次数** 触发器会在人员订阅时启动流。

![](assets/subscribes-to-vibes-list-real.jpg)

此 **点击短信消息中的链接** 当人员单击短信消息中的链接时，触发器将启动流程。

![](assets/clicks-link-in-sms-message.jpg)

## 短信过滤器 {#sms-filters}

您还可以在智能列表中使用维贝过滤器。 此 **订阅的访客列表** 筛选器查找具有 *从不* 订阅了Vibes。 这包括已取消订阅和已删除的人员，即使流程中会忽略已删除的人员。 此过滤器最适合报表。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

相比之下， **Vibes列表的成员** 筛选器查找 _任何人_ 当前订阅了访客，最适合在智能营销活动或列表中使用。

![](assets/image001.png)

>[!NOTE]
>
>所有短信过滤器都包含 **活动日期** 缺省情况下受约束。

在智能列表中设置Vibes触发器和过滤器后，您可以 [定义流](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [为Smart Campaign定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [查找筛选器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
