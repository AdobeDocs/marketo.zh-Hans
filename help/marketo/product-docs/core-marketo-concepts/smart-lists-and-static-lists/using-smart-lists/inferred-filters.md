---
unique-page-id: 2953188
description: 推断的过滤器 — Marketo文档 — 产品文档
title: 推断的筛选器
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 推断的筛选器 {#inferred-filters}

当有人访问您的网站时， [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 把它们饼干放进系统中。 我们在一个专门的数据库里查询他们的IP，并推断出各种好的信息。

>[!NOTE]
>
>为确保推断的字段值保持最新，我们定期更新用于IP地址查找的数据库。 数据库更新可能会引入新的推断字段值，您可能需要将这些值添加到智能列表筛选器定义中。
>
>数据库更新可能发生在以下期间 [Marketo Engage产品版本](/help/marketo/release-notes/release-schedule.md){target="_blank"}. When an update does occur, the [Marketo Engage release notes](/help/marketo/release-notes/current.md){target="_blank"} 将包含对推断字段值所做任何更改的解释。

![](assets/image2015-4-27-13-3a25-3a46.png)

![](assets/image2015-4-27-16-3a58-3a53.png)

![](assets/image2015-4-27-16-3a59-3a35.png)

![](assets/image2015-4-27-17-3a0-3a12.png)

![](assets/image2015-4-27-13-3a36-3a9.png)

![](assets/image2015-4-27-13-3a30-3a48.png)

当您在智能列表中使用这些过滤器时，结果将产生具有此推断信息的用户。

>[!TIP]
>
>在Web活动报表中使用这些筛选器。 使用销售代表的区域，并向他们订阅过去24小时内的网站访客自定义每日报表。 他们会喜欢的！
>
>* 已访问网页 — 过去24小时
>* 推断的状态为 [选择他们的地区]

这些匿名访客在单击电子邮件链接或填写表单时，会自动转换为人员。 但是，他们保留所有推断出的信息。

>[!NOTE]
>
>详细了解 [匿名活动和潜在客户](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md).
