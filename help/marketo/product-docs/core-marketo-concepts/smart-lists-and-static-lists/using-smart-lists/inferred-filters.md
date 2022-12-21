---
unique-page-id: 2953188
description: 推断性过滤器 — Marketo文档 — 产品文档
title: 推断性过滤器
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
source-git-commit: c045e9008bf0e9d145ac67866a1e0d7cb6e26069
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 推断性过滤器 {#inferred-filters}

当有人访问您的网站时， [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 给他们点饼干，然后放到系统中。 我们在一个特殊的数据库中查找他们的IP信息，并推断出各种好信息。

>[!NOTE]
>
>为确保推断的字段值保持为最新，我们会定期更新用于IP地址查找的数据库。 数据库更新可以引入新的推断字段值，您可能需要将这些值添加到智能列表筛选器定义中。
>
>数据库更新可在 [Marketo Engage产品版本](/help/marketo/release-notes/release-schedule.md){target=&quot;_blank&quot;}。 当发生更新时， [Marketo Engage发行说明](/help/marketo/release-notes/current.md){target=&quot;_blank&quot;}将包含对推断字段值所做任何更改的说明。

![](assets/image2015-4-27-13-3a25-3a46.png)

![](assets/image2015-4-27-16-3a58-3a53.png)

![](assets/image2015-4-27-16-3a59-3a35.png)

![](assets/image2015-4-27-17-3a0-3a12.png)

![](assets/image2015-4-27-13-3a36-3a9.png)

![](assets/image2015-4-27-13-3a30-3a48.png)

当您在智能列表中使用其中任何过滤器时，结果会产生包含此推断信息的用户。

>[!TIP]
>
>在Web活动报表中使用这些过滤器。 使用销售代表的地区，并在过去24小时内与网站访客订阅一份自定义的每日报告。 他们会喜欢的！
>
>* 访问网页 — 最近24小时
>* 推断状态为 [选择其领土]


这些匿名访客在单击电子邮件链接或填写表单时会自动转换为人员。 但是，他们会保留所有推断的信息。

>[!NOTE]
>
>详细了解 [匿名活动和潜在客户](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md).
