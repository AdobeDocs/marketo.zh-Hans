---
description: Dynamic Chat概述 — Marketo文档 — 产品文档
title: Dynamic Chat概述
feature: Dynamic Chat
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: be1ca409642fd5d81d341fbadaff38c268fe198f
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 2%

---

# Dynamic Chat概述 {#dynamic-chat-overview}

Dynamic Chat功能允许您利用简单易用的界面来定位访问您网站的用户和帐户。 收集相关内容，如姓名、联系信息和自由文本。 网站访客还可以与现场代理聊天，甚至与您的销售团队预约会议。 Dynamic Chat活动和参与数据可用于将成员添加到Marketo项目并触发跨渠道活动。

>[!TIP]
>
>请访问[此页面](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html?lang=zh-Hans){target="_blank"}查看Dynamic Chat的教程视频。

## 集成 {#integrations}

Dynamic Chat的一个关键组件是，它能够以本机方式与您的Marketo订阅进行交互。 要利用此集成的完整功能，您首先需要启动数据同步。 根据Marketo数据库的大小，完成初始[一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"}最多可能需要24小时的数据。

以下内容已同步：

* 人员字段数据
* 公司字段数据
* 活动数据

## 对话 {#dialogues}

对话框表示单个聊天项目。 将其视为一个容器，其中包含与网站访客进行引人入胜的聊天对话框所需的所有内容。 在每个对话框中，您可以指定希望对话框显示的页面、显示目标对象以及对话框本身的内容和流程。 此外，您还可以查找量度以查看对话框的执行情况。 [了解有关对话框的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}。

## 配置 {#configuration}

在“配置”选项卡中，自定义各种对话框的外观。 更改字体、颜色、响应时间等！ [了解有关配置的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}。

## 日程表 {#calendar}

连接你的Outlook或Gmail日历，以用于聊天机器人中的约会计划。 [了解有关日历的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## 会议 {#meetings}

在这里，您可以看到网站访客通过各种对话框安排的所有约会。 [了解有关会议的详细信息](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## 路由 {#routing}

在这里，您可以查看已连接其日历的所有代理的列表，以及它们向网站访客呈现的顺序，还可以创建自定义路由规则。 [了解有关路由的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## 实时聊天 {#live-chat}

提供符合条件的Web访客，以便通过[实时聊天](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}与销售代表联系。

## 会话流 {#conversational-flow}

[设计可由访客根据您指定的操作（例如，填写表单、单击链接等）触发的对话](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}。

## 生成式 AI {#generative-ai}

Adobe Dynamic Chat中的[生成人工智能](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/overview.md){target="_blank"}实时处理意图信号、用户偏好和过去的行为，以便为聊天访客生成相关的个性化消息。

## 更改语言 {#changing-the-language}

请按照以下步骤更改Dynamic Chat语言。

>[!IMPORTANT]
>
>更改配置文件级别的语言将更改&#x200B;_所有_ Experience Cloud应用程序的语言，而不仅仅是Dynamic Chat。

1. 在您的Experience Cloud帐户中，单击设置图标并选择&#x200B;**首选项**。

   ![](assets/dynamic-chat-overview-1.png)

1. 单击电子邮件地址下的当前语言。

   ![](assets/dynamic-chat-overview-2.png)

1. 选择您的新语言（第二种语言是可选的），然后单击&#x200B;**保存**。

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >有几十种语言可供选择，但是Dynamic Chat语仅支持以下语言：英语、法语、德语、日语、西班牙语、意大利语、巴西葡萄牙语、朝鲜语、简体中文和繁体中文。

当您更新语言时，除了您亲自填充的单词（例如，流响应）之外，应用程序本身中的所有内容都会更改。

## Dynamic Chat数据保留限制 {#dynamic-chat-data-retention-limits}

以下只是Dynamic Chat中的一些限制/参数。 有关完整列表，请参阅Marketo Engage[产品描述页](https://helpx.adobe.com/cn/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}。

<table>
  <th>数据类型</th>
  <th>保留期</th>
 <tr>
  <td>无任何参与的匿名潜在客户</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>目标活动</td>
  <td>24个月</td>
 </tr>
 <tr>
  <td>文档活动</td>
  <td>24个月</td>
 </tr>
 <tr>
  <td>与对话活动交互</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>会议预订活动</td>
  <td>24个月</td>
 </tr>
</table>

## 常见问题 {#faq}

请查看[Dynamic Chat常见问题解答](/help/marketo/product-docs/demand-generation/dynamic-chat/faq.md){target="_blank"}。
