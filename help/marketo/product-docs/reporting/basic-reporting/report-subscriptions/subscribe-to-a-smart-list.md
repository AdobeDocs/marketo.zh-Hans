---
unique-page-id: 7505310
description: 订阅智能列表 — Marketo文档 — 产品文档
title: 订阅智能列表
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 订阅智能列表 {#subscribe-to-a-smart-list}

订阅智能列表是一种很好的跟踪人员的方法，报表会直接发送到您的收件箱。

您可以在两个不同的位置创建智能列表订阅：

* 营销活动
* 数据库

订阅使用运行订阅时的完整人员列表。

订阅位于智能列表所在的位置，即营销活动或数据库中。

您可以从同一智能列表创建多个订阅。

订阅特定于工作区。 例如，此订阅列表与本文其余部分中显示的工作区不同：

![](assets/one.png)

>[!NOTE]
>
>每个Marketo实例限制为100个订阅，每个订阅最多包含100,000名人员（跨工作区）。 如果智能列表包含超过100,000个名称，Marketo将为前100,000个运行订阅。

## 创建智能列表订阅 {#create-a-smart-list-subscription}

1. 转到 **数据库** 或 **营销活动**.

   ![](assets/db.png)

1. 选择要为其创建订阅的智能列表。 单击 **列出操作** 并选择 **新建智能列表订阅**.

   ![](assets/three.png)

1. 为您的订阅提供 **名称**，然后选择或输入 **收件人**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. 单击 **频率** 列出并选择频率。

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. 设置 **结束投放** 日期。 您可以选择 **从不** 或日历日期。

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. 单击 **格式** 并从列表中选择。

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. 单击&#x200B;**创建**。

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. 您的新智能列表订阅将显示在“订阅”选项卡的列表顶部。 单击 **发送** 如果您希望立即发送，而不是等到计划的电子邮件发送。

   ![](assets/eight.png)

1. 我们建议您清除“活动”复选框，以便在没有人订阅智能列表订阅时将其停用。

   ![](assets/nine.png)

   这很容易，不是吗？

## 电子邮件 {#email-message}

收件人将收到一封包含下载报表选项的电子邮件，以及一个直接指向Marketo实例中列表的链接。 下载链接将在四天后过期。

>[!NOTE]
>
>如果 [安全订阅管理](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) 设置已设置为 **是**，则只有有权访问Marketo实例的用户才能下载报表。

![](assets/image2015-4-17-15-3a46-3a47.png)

如果报表中包含0人，收件人仍会收到电子邮件。 但是，电子邮件仅声明没有人员可报告。

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>修改基于订阅的智能列表筛选器时，也会更新报表。

电子邮件还提供了有关用于创建列表的过滤器的其他信息。

## 删除订阅 {#delete-a-subscription}

要删除预订，请在“预订”选项卡中选择它，然后单击“删除预订”。

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [编辑智能列表订阅](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [保护订阅管理员设置](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
