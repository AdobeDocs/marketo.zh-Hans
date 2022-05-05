---
description: 了解Veva CRM同步 — Marketo文档 — 产品文档
title: 了解Veeva CRM同步
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
source-git-commit: 884c9a27f3876ec3036f2f7187db30565cdd49a7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 了解Veeva CRM同步 {#understanding-the-veeva-crm-sync}

在几个简单的步骤中，可以轻松地在Adobe Marketo Engage和Veeva CRM之间同步。

## 同步的工作原理 {#how-the-sync-works}

Marketo Engage每天与Veeva CRM进行同步。 每次同步都需要一段时间，暂停5分钟，然后再次开始。

>[!NOTE]
>
>第一次同步可能需要数小时甚至数天，因为Marketo Engage正在从Veeva中复制整个数据库。 之后，每次同步通常需要几分钟（有时是几秒），并且只同步已更改的数据。

![](assets/understanding-the-veeva-sync-1.png)

Veva和Marketo Engage之间的同步仅对Person帐户对象上的“联系人”字段是双向的。 在这些情况下，无论您何时在Veva或Marketo Engage中进行更改，您的更新都将反映在这两个系统中。 所有其他同步仅从Veeva到Marketo Engage。 有关每个链接的详细信息，请单击以下链接。

## Marketo Engage与Veeva之间同步的内容 {#what-is-synced-between-marketo-engage-and-veeva}

* [人员帐户](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target=&quot;_blank&quot;}
* 用户
* [调用和调用关键对象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
* [自定义对象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}

## 注意事项 {#things-to-know}

* 的 [您在VeevaMarketo Engage中输入的凭据](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target=&quot;_blank&quot;}用于同步数据。 将只包含这些凭据有权访问的数据。

* Veeva CRM基于force.com，且与该平台一起使用的丰富体验Marketo Engage会继承到此同步中。

* Veeva CRM显示：潜在客户、联系人、帐户（业务帐户、机会、营销活动和活动）。 但是，在与Marketo Engage同步时不支持这些参数。
