---
unique-page-id: 4719283
description: 了解 Salesforce 同步 — Marketo 文档 — 产品文档
title: 了解 Salesforce 同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '212'
ht-degree: 100%

---

# 了解 [!DNL Salesforce] 同步 {#understanding-the-salesforce-sync}

Marketo Engage 与 Salesforce 密不可分、相辅相成。我们会保持您的销售数据与营销数据始终同步。

## 同步机制如何运作 {#how-sync-works}

Marketo 全天候与 [!DNL Salesforce] 进行同步。每次同步都会运行一段时间，然后暂停 5 分钟，再重新开始。

>[!NOTE]
>
>您订阅中的首次同步可能需要数小时，甚至数天时间，因为 Marketo 需要从 [!DNL Salesforce] 复制整个数据库。此后，每次同步通常只需几秒到几分钟，并且只会同步发生变化的数据。

![](assets/sync-illustration.png)

在潜在客户、联系人以及 [!DNL Salesforce] 营销活动方面，[!DNL Salesforce] 与 Marketo 之间的同步是双向的。在这些情况下，无论您是在 [!DNL Salesforce] 还是 Marketo 中进行更改，更新都会同步反映到两个系统中。其余同步均仅从 [!DNL Salesforce] 单向同步到 Marketo。请点击下方链接，查看各项同步的详细信息。

## Marketo 与 [!DNL Salesforce] 之间会同步哪些内容？ {#what-is-synced-between-marketo-and-salesforce}

* [潜在客户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [联系人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [帐户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [用户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [商机](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce 营销活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [自定义对象](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>您[在 Marketo 中为 Salesforce 输入的凭据](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}将用于执行数据同步。只有这些凭据有权限访问的数据才会得到同步。

Marketo 与 [!DNL Salesforce] 之间的同步是同类解决方案中功能最强大的之一。这种体验就像魔法一样：在一个系统中完成更改，另一个系统很快就会同步更新。
