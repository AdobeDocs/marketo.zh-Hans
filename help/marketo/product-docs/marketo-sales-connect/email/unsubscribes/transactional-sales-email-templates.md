---
description: 事务性销售电子邮件模板 — Marketo文档 — 产品文档
title: 事务性销售电子邮件模板
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# 事务性销售电子邮件模板 {#transactional-sales-email-templates}

如果您的团队发送事务性或非商业性电子邮件，您可以将电子邮件模板标记为非商业性，这样它就可以绕过取消订阅。

## 注意事项 {#things-to-note}

* 非商业电子邮件将绕过销售取消订阅和 [Marketo Engage取消订阅检查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* 取消订阅消息不会自动附加到非商业电子邮件，即使 [附加取消订阅消息管理员设置](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} 仍会填充您的团队取消订阅消息。

## 配置电子邮件模板用于非商业用途 {#configure-an-email-template-for-non-commercial-use}

1. 在标题中，单击 **模板**.

PICC

1. 搜索要更新的模板。

PICC

1. 选择模板。

PICC

1. 在“模板设置”下启用非商业电子邮件切换。

PICC

## 发送非商业电子邮件 {#send-a-non-commercial-email}

选择取消订阅的人员时，他们将会突出显示为橙色。

1. 在撰写窗口中，选择要查看的非商业模板。

PICC

1. 用户将看到一个横幅，显示他们当前选择了非商业电子邮件模板。

PICC

1. 单击 **发送**.

PICC

即使此人已取消订阅，仍会发送电子邮件。
