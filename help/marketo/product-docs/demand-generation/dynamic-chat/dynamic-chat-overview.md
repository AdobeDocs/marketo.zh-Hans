---
description: 了解用于定位访客和收集潜在客户的Dynamic Chat。 设置实时聊天、预约会议，并通过聊天参与触发Marketo程序。
title: Dynamic Chat 概述
feature: Dynamic Chat
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 74%

---

# [!DNL Dynamic Chat] 概述 {#dynamic-chat-overview}

Dynamic Chat允许您利用直观的界面来定位访问您网站的人和帐户。 收集相关信息，例如姓名、联系信息以及自由文本内容。 网站访客还可以与实时客服人员聊天，甚至直接与销售团队预约会议。 Dynamic Chat 的活动和参与数据可用于将成员添加到 Marketo 项目中，并触发跨渠道活动。

>[!TIP]
>
>访问[此页面](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html){target="_blank"}可查看 Dynamic Chat 的教程视频。

## 集成 {#integrations}

Dynamic Chat 的一个关键组成部分是其与 Marketo 订阅的原生集成能力。 要利用此集成的完整功能，您首先需要启动数据同步。 根据您的 Marketo 数据库规模，首次[一次性数据同步](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"}可能需要长达 24 小时才能完成。

以下数据将会同步：

* 人员字段数据
* 公司字段数据
* 活动数据

## 对话 {#dialogues}

对话表示一次单独的聊天互动。 可以将其理解为一个容器，包含了与网站访客进行有效聊天所需的全部内容。 在每个对话中，您都可以指定对话出现的页面、展示给哪些受众，以及对话本身的内容和流程。 此外，您还可以查看相关量度，以评估对话的表现效果。 [了解有关对话的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}。

## 配置 {#configuration}

在“配置”选项卡中，您可以自定义各个对话的外观和体验。 更改字体、颜色、响应时间等设置！ [了解有关配置的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}。

## 日程表 {#calendar}

连接您的 Outlook 或 Gmail 日程表，以便在聊天机器人中用于预约安排。 [了解有关日程表的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## 会议 {#meetings}

在这里，您将看到网站访客通过各种对话框安排的所有约会。 [了解有关会议的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## 路由 {#routing}

在这里，您可以查看已连接其日历的所有代理的列表、它们向网站访客呈现的顺序以及创建自定义路由规则。 [了解有关路由的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## 实时聊天 {#live-chat}

通过[实时聊天](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}为符合条件的网站访客提供与销售代表直接沟通的方式。

## 会话流 {#conversational-flow}

[设计一个](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}可由访客根据您指定的操作（例如填写表单、点击链接等）触发的会话流程。

## 生成式 AI {#generative-ai}

Adobe Dynamic Chat 中的[生成式 AI ](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/overview.md){target="_blank"}会实时处理意图信号、用户偏好和历史行为，为聊天访客生成相关且个性化的消息。

## 更改语言 {#changing-the-language}

按照以下步骤更改您的 Dynamic Chat 语言。

>[!IMPORTANT]
>
>在轮廓级别更改语言将影响&#x200B;_所有_ Experience Cloud 应用，而不仅仅是 [!DNL Dynamic Chat]。

1. 在您的 Experience Cloud 帐户中，点击设置图标并选择 **[!UICONTROL Preferences]**。

   ![](assets/dynamic-chat-overview-1.png)

1. 点击电子邮件地址下方显示的当前语言。

   ![](assets/dynamic-chat-overview-2.png)

1. 选择新的语言（第二语言为可选），然后点击 **[!UICONTROL Save]**。

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >可供选择的语言有数十种，但 [!DNL Dynamic Chat] 仅支持以下语言：英语、法语、德语、日语、西班牙语、意大利语、巴西葡萄牙语、韩语、简体中文和繁体中文。

当您更新语言时，除了您亲自填充的单词（例如，流响应）之外，应用程序本身中的所有内容都会更改。

## Dynamic Chat 数据保留限制 {#dynamic-chat-data-retention-limits}

以下是Dynamic Chat中的一些限制/参数。 有关完整列表，请参阅Marketo Engage [产品描述页](https://helpx.adobe.com/cn/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}。

<table>
  <th>数据类型</th>
  <th>保留期限</th>
 <tr>
  <td>无任何互动的匿名潜在客户</td>
  <td>90 天</td>
 </tr>
 <tr>
  <td>目标活动</td>
  <td>24 个月</td>
 </tr>
 <tr>
  <td>文档活动</td>
  <td>24 个月</td>
 </tr>
 <tr>
  <td>与对话交互的活动</td>
  <td>90 天</td>
 </tr>
 <tr>
  <td>会议预约活动</td>
  <td>24 个月</td>
 </tr>
</table>

## 常见问题解答 {#faq}

请参阅[Dynamic Chat常见问题解答](/help/marketo/product-docs/demand-generation/dynamic-chat/faq.md){target="_blank"}。
