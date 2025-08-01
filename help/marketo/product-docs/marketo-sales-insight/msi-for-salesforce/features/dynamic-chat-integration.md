---
description: Dynamic Chat集成 — Marketo文档 — 产品文档
title: Dynamic Chat集成
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 4%

---

# Dynamic Chat集成 {#dynamic-chat-integration}

详细了解Dynamic Chat与Sales Insight的集成。

>[!PREREQUISITES]
>
>* 您的Sales Insight SFDC程序包必须为[2.4.0或更高版本](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* 您必须设置[Dynamic Chat集成](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* 确保在您的Sales Insight [操作设置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"}中填充“API密钥”字段。 否则，请在[此处](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}了解如何检索它。

## [!DNL Marketo Sales Insight]配置选项卡 {#marketo-sales-insight-configuration-tab}

请按照以下步骤启用[!DNL Dynamic Chat]集成。

1. 登录到您的[!DNL Salesforce]帐户，单击选项卡栏末尾的+并单击&#x200B;**[!DNL Marketo Sales Insight Config]**。

1. 单击以展开“[!UICONTROL Visualforce Panel]”。

   ![](assets/dynamic-chat-integration-1.png)

1. 选中&#x200B;**[!UICONTROL Enable Dynamic Chat Data]**&#x200B;复选框。

   ![](assets/dynamic-chat-integration-2.png)

## 功能概述 {#feature-overview}

以下[!DNL Dynamic Chat]活动可由[!DNL Sales Insight]个用户利用……

参与对话框：已登录Marketo并在访客单击聊天机器人并参与对话框时在[!DNL Sales Insight]中填充。

* 对话名称
* Page URL
* 状态（已启动/已删除/已完成）

计划的约会：登录Marketo并在访客通过聊天机器人成功计划约会时在[!DNL Sales Insight]中填充。

* 对话名称
* 代理
* Page URL
* 计划日期（插入日期和时间戳）
* 状态（已计划、已重新计划、已取消）

已实现目标：访客在任何对话框流中实现目标时登录Marketo并在[!DNL Sales Insight]中填充。

* 对话名称
* 目标名称
* Page URL

与文档交互：已登录Marketo并在访客与通过聊天机器人共享的文档交互时[!DNL Sales Insight]中填充。

* 对话名称
* 文档
* 状态

可在分析功能板中查看聊天活动。

![](assets/dynamic-chat-integration-3.png)

Lead和Contact面板中提供了“聊天”选项卡。 它包括[!UICONTROL Activity Type]、[!UICONTROL Dialogue Name]和[!UICONTROL Date]列。

![](assets/dynamic-chat-integration-4.png)

您可以通过单击某个活动类型来详细了解该活动类型。

![](assets/dynamic-chat-integration-5.png)

同样，“帐户”和“机会”面板包括[!UICONTROL Name]、[!UICONTROL Activity Type]、[!UICONTROL Dialogue Name]和[!UICONTROL Date]列。

![](assets/dynamic-chat-integration-6.png)

“聊天”选项卡也包含在您的全局Marketo选项卡中。 它包括三种活动类型([!UICONTROL Engaged Dialogue]、[!UICONTROL Scheduled Appointment]、[!UICONTROL Reached Goal])，以及以下列：

* [!UICONTROL Person]
* [!UICONTROL Account]
* [!UICONTROL Activity type] ([!UICONTROL Engaged Dialogue]，[!UICONTROL Scheduled Appointment]，[!UICONTROL Reached Goal])
* [!UICONTROL Dialogue Name]
* [!UICONTROL Date]

同样地，您可以通过单击某个活动类型来了解关于该活动类型的更多信息。

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>如果“[!UICONTROL Enable Dynamic Chat data]”复选框已禁用，则将禁用以下功能：
>
>* 分析功能板（智能网格和每周列表视图）中包含聊天活动的行
>* Lead 、 Contact 、 Account和Opportunity面板中的Chat选项卡
>* “全局Marketo”选项卡中的“聊天”选项卡
>
>不能只禁用其中一项功能。
