---
description: 了解Veeva CRM同步 — Marketo文档 — 产品文档
title: 了解Veeva CRM同步
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 了解Veeva CRM同步 {#understanding-the-veeva-crm-sync}

通过几个简单的步骤，可以轻松地在Adobe Marketo Engage和Veeva CRM之间运行同步。

## 同步的工作方式 {#how-the-sync-works}

Marketo Engage每天与Veeva CRM进行全天候同步。 每次同步都需要一些时间，暂停5分钟，然后重新开始。

>[!NOTE]
>
>由于Marketo Engage正在从Veeva复制整个数据库，因此首次同步可能需要几个小时甚至几天。 之后，每次同步通常需要几分钟（有时几秒），并且只同步已更改的数据。

![](assets/understanding-the-veeva-sync-1.png)

Veeva和Marketo Engage之间的同步仅针对Person帐户对象上的Contact字段是双向的。 在这些情况下，无论您在Veeva还是Marketo Engage中进行更改，您的更新都会反映在这两个系统中。 所有其他同步仅从Veeva到Marketo Engage。 单击下面的链接以了解每个报表的详细信息。

## Marketo Engage和Veeva之间同步的内容 {#what-is-synced-between-marketo-engage-and-veeva}

* [人员帐户](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* 用户
* [调用和调用关键对象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [自定义对象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## 注意事项 {#things-to-know}

* 此 [您在Marketo Engage中为Veeva输入的凭据](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} 用于同步数据。 仅包含这些凭据有权访问的数据。

* Veeva CRM基于force.com ，此同步中继承了平台所具有的丰富体验Marketo Engage。

* Veeva CRM显示：潜在客户、联系人、客户（业务帐户、机会、营销活动和活动）。 但是，“与Marketo Engage同步”中不支持这两个参数。
