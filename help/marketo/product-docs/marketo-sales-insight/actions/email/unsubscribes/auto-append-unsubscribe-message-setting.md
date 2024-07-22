---
description: 自动附加取消订阅消息设置 — Marketo文档 — 产品文档
title: 自动附加取消订阅消息设置
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# 自动附加取消订阅消息设置 {#auto-append-unsubscribe-message-setting}

确保发送的每封销售分析操作电子邮件都包含取消订阅消息，以便收件人可以轻松选择退出通信。 在启用附加取消订阅消息后，您的团队从Marketo Sales发送的所有通信都将包含取消订阅消息，包括从Web应用程序和Salesforce发送的电子邮件。

>[!NOTE]
>
>如果您在电子邮件模板中使用`{{team_unsubscribe}}`动态字段并且启用了取消订阅消息附加设置，则团队取消订阅动态字段将填充您的取消订阅消息&#x200B;_，而不是_&#x200B;附加您的取消订阅消息。

## 启用/禁用取消订阅附加 {#enable-disable-unsubscribe-append}

1. 单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. 在“管理员设置”下，单击&#x200B;**取消订阅**。

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 在“消息传递”选项卡的“附加取消订阅消息”下，将滑块移动到所需的状态。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>如果禁用附加取消订阅消息设置，我们建议向模板添加取消订阅页脚，以确保您的通信具有选择退出选项。 您可通过向每个模板添加自己的自定义消息或使用`{{team_unsubscribe}}` [动态字段](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}来执行此操作。
