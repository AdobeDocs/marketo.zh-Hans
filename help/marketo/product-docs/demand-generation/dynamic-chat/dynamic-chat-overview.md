---
description: 动态聊天概述 — Marketo文档 — 产品文档
title: 动态聊天概述
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: adf3a9f156ec5ed823a0647affb87f6c0686d35f
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# 动态聊天概述 {#dynamic-chat-overview}

通过动态聊天，您可以利用易于使用的界面来定位访问您网站的人员和帐户。 收集相关内容，如姓名、联系信息和自由文本。 网站访客还可以预订与销售团队的会议。 动态聊天活动和参与数据可用于向Marketo项目添加成员并触发跨渠道活动。

>[!NOTE]
>
>动态聊天正在逐步推出，目前的可用性有限。 此页面将在正式发布(GA)详细信息之后进行更新。

>[!TIP]
>
>访问 [本页](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) 查看动态聊天的教程视频。

## 集成 {#integrations}

动态聊天的一个关键组件是其与Marketo订阅本机接口的功能。 为了利用此集成的全部功能，您首先需要启动数据同步。 根据Marketo数据库的大小，初始数据可能最多需要24小时， [一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) 完成。

会同步以下内容：

* 人员字段数据
* 公司字段数据
* 活动数据

## 对话框 {#dialogues}

对话表示单个聊天项目。 将其视为一个容器，其中包含与网站访客进行引人入胜的聊天对话所需的所有内容。 在每个对话框中，您可以指定希望对话框显示在哪些页面上、希望将其显示给哪些对象，以及对话框本身的内容和流程。 此外，您还可以找到量度来查看对话框的效果。 [了解有关对话框的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target=&quot;_blank&quot;}。

## 配置 {#configuration}

在“配置”选项卡中，自定义各种对话框的外观。 更改字体、颜色、响应时间等！ [了解有关配置的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## 日历 {#calendar}

在“日历”选项卡中，连接您的（Outlook或Gmail）日历，以用于聊天机器人中的约会计划。 用户的日历连接到动态聊天后，该用户将被添加到队列，其日历将可供网站访客安排约会时间。

您还可以自定义在用户日历上安排约会时发送给访客的邀请正文。

## 会议 {#meetings}

在这里，您将看到网站访客通过各种对话安排的所有约会。 在此，您将找到预订约会的人的电子邮件地址、他们与哪位座席预订了约会、预定何时进行约会以及会议是否已发生。

## 路由 {#routing}

在这里，您可以看到已连接其日历的所有座席的列表，以及将向网站访客显示的顺序。 会议是循规蹈矩的，所以如果你有五个特工和三号探员参加最后一次会议，四号探员会得到下一次会议，接着是五号探员，然后是一号探员。

## 常见问题解答 {#faq}

**数据会存储多长时间以便进行报告？**

90天(请参阅 [下面](#limits-in-dynamic-chat))。

**动态聊天是否允许进行实时聊天？**

不会，它仅使用预先确定的响应。

**如何定位匿名用户？**

在对话框中，您需要使用 _人员电子邮件为空_ 属性。

**是否支持AI/NLP功能？**

我们不支持AI/NLP功能。

**动态聊天除英语以外，还提供任何语言吗？**

现在不行。

## 动态聊天中的限制 {#limits-in-dynamic-chat}

<table>
  <th>参数</th>
  <th>描述</th>
  <th>限制</th>
 <tr>
  <td>对话框总数</td>
  <td>对话总数（已发布和草稿）</td>
  <td>500</td>
 </tr>
 <tr>
  <td>已发布的对话框</td>
  <td>保存的已发布对话框数</td>
  <td>100</td>
 </tr>
 <tr>
  <td>每个对话框的目标URL</td>
  <td>可添加到单个对话框的Target URL数量</td>
  <td>20</td>
 </tr>
 <tr>
  <td>每个对话框的属性</td>
  <td>可添加到单个对话框的受众标准的属性数量</td>
  <td>100</td>
 </tr>
 <tr>
  <td>群组</td>
  <td>可添加到单个对话框的组数</td>
  <td>10</td>
 </tr>
 <tr>
  <td>每组属性</td>
  <td>可添加到群组的属性数</td>
  <td>10</td>
 </tr>
 <tr>
  <td>卡片</td>
  <td>每个对话框可添加到画布的卡片数</td>
  <td>500</td>
 </tr>
 <tr>
  <td>匿名潜在客户数据保留期</td>
  <td>匿名潜在客户信息在没有任何参与的情况下将保留多长时间</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>目标活动保留期</td>
  <td>保留目标活动数据的时长</td>
  <td>24个月</td>
 </tr>
 <tr>
  <td>记录活动保留期</td>
  <td>保留文档活动数据的时间</td>
  <td>24个月</td>
 </tr>
 <tr>
  <td>与对话活动保留期进行交互</td>
  <td>与Dialog活动数据交互的时长将保留</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>会议预订活动保留期</td>
  <td>会议预订活动将存储在动态聊天中的时长</td>
  <td>24个月</td>
 </tr>
</table>
