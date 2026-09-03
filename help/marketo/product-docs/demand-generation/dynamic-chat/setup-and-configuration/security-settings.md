---
description: 了解如何使用阻止的或允许的域配置Dynamic Chat安全性。 限制代理查看的电子邮件域以及可以使用聊天脚本的网站。
title: 安全性设置
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 88949407423d12a95bf39470e3c29835d934e2f6
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 3%

---

# 安全性设置 {#security-settings}

在“安全”设置中，您可以向被阻止或允许列表添加域。

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>“阻止和允许电子邮件域”过滤仅适用于访客直接在Dynamic Chat中（在聊天机器人中或对话流中）输入其电子邮件地址的情况。 它不适用于Dynamic Chat从集成产品（如Marketo Engage）收到的电子邮件地址。 有关详细信息，请参阅下表。

| 场景 | 筛选是否适用？ |
|---|---|
| 访客在Dynamic Chat聊天机器人中直接键入其电子邮件 | 是 |
| 访客将电子邮件直接键入到Dynamic Chat对话流中 | 是 |
| 电子邮件是通过Marketo表单提交预填充的（在表单填写之后会显示对话流程） | 否 |
| 电子邮件会从任何其他集成系统传递到Dynamic Chat | 否 |

## 阻止的电子邮件域 {#blocked-email-domains}

如果有任何访客具有您不希望代理与之交互（例如，竞争对手）的电子邮件域，请将其电子邮件域添加到。

1. 选择&#x200B;**启用验证**&#x200B;滑块以激活您的。 最多输入50个域，然后单击&#x200B;**保存**。

   ![](assets/security-settings-2.png)

## 允许的域 {#allowed-domains}

添加允许的域可确保第三方无法从您的站点中刮取Javascript并将其添加到自己的站点中。

1. 选择&#x200B;**启用验证**&#x200B;滑块以激活您的。 输入允许的域，然后单击&#x200B;**保存**。

   ![](assets/security-settings-3.png)
