---
description: 事务性销售电子邮件模板 — Marketo文档 — 产品文档
title: 事务性销售电子邮件模板
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# 事务性销售电子邮件模板 {#transactional-sales-email-templates}

如果您的团队发送事务性或非商业性电子邮件，您可以将电子邮件模板标记为非商业性，这样它就可以绕过取消订阅。

## 注意事项 {#things-to-note}

* 非商业电子邮件将绕过销售取消订阅和[Marketo Engage取消订阅检查](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}，但不会绕过[阻止的域](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md){target="_blank"}。

* 即使启用了[附加取消订阅消息管理员设置](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"}，取消订阅消息也不会自动附加到非商业电子邮件。 但是，`{{team_unsubscribe}}` [动态字段](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}仍将填充您的团队取消订阅消息。

## 配置电子邮件模板用于非商业用途 {#configure-an-email-template-for-non-commercial-use}

1. 在标题中，单击&#x200B;**模板**。

   ![](assets/transactional-sales-email-templates-1.png)

1. 查找并选择要更新的模板。

   ![](assets/transactional-sales-email-templates-2.png)

1. 在“模板设置”下启用非商业电子邮件切换。

   ![](assets/transactional-sales-email-templates-3.png)

## 发送非商业电子邮件 {#send-a-non-commercial-email}

>[!NOTE]
>
>选择取消订阅的人员时，他们将会突出显示为橙色。

1. 在标题中，单击&#x200B;**撰写**。 查找并选择所需的非商业模板。

   ![](assets/transactional-sales-email-templates-4.png)

1. 用户将看到一个横幅，显示他们已选择非商业电子邮件模板。

   ![](assets/transactional-sales-email-templates-5.png)

1. 单击&#x200B;**发送**。

   ![](assets/transactional-sales-email-templates-6.png)

即使此人已取消订阅，仍会发送电子邮件。
