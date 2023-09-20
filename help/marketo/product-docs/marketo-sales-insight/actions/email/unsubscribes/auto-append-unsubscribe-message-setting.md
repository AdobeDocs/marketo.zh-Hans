---
description: 自动附加取消订阅消息设置 — Marketo文档 — 产品文档
title: 自动附加取消订阅消息设置
hide: true
hidefromtoc: true
feature: Sales Insight Actions
source-git-commit: b0f62abfe04efd8e72ed8e92442d4a46ea118f33
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# 自动附加取消订阅消息设置 {#auto-append-unsubscribe-message-setting}

确保发送的每封销售分析操作电子邮件都包含取消订阅消息，以便收件人可以轻松选择退出通信。 在启用附加取消订阅消息后，您的团队从Marketo Sales发送的所有通信都将包含取消订阅消息，包括从Web应用程序和Salesforce发送的电子邮件。

>[!NOTE]
>
>如果您使用 `{{team_unsubscribe}}` 电子邮件模板中的动态字段并且启用了取消订阅消息附加设置，团队取消订阅动态字段将填充您的取消订阅消息 _而不是_ 正在附加您的取消订阅消息。

## 启用/禁用取消订阅附加 {#enable-disable-unsubscribe-append}

1. 单击齿轮图标并选择 **设置**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. 在管理设置下，单击 **取消订阅**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 在“消息传递”选项卡的“附加取消订阅消息”下，将滑块移动到所需的状态。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>如果禁用附加取消订阅消息设置，我们建议向模板添加取消订阅页脚，以确保您的通信具有选择退出选项。 为此，您可以向每个模板添加自己的自定义消息，或使用 `{{team_unsubscribe}}` 动态字段。
