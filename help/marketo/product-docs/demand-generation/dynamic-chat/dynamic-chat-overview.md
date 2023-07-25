---
description: Dynamic Chat概述 — Marketo文档 — 产品文档
title: Dynamic Chat概述
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
feature: Dynamic Chat
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Dynamic Chat概述 {#dynamic-chat-overview}

Dynamic Chat允许您利用易于使用的界面来定位访问您网站的人和帐户。 收集相关内容，如姓名、联系信息和自由文本。 网站访客还可以预订与您的销售团队的会议。 Dynamic Chat活动和参与数据可用于将成员添加到Marketo项目群并触发跨渠道活动。

>[!NOTE]
>
>Dynamic Chat正在逐步推出，目前可用性有限。 此页面将在正式发布时进行更新，并提供正式发布版(GA)详细信息。

>[!TIP]
>
>访问 [此页面](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) 查看Dynamic Chat的教程视频。

## 集成 {#integrations}

Dynamic Chat的一个关键组件是，它能够以本机方式与您的Marketo订阅进行交互。 要利用此集成的完整功能，您首先需要启动数据同步。 根据Marketo数据库的大小，初始数据可能需要长达24小时， [一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) 完成。

以下内容已同步：

* 人员字段数据
* 公司字段数据
* 活动数据

## 对话 {#dialogues}

对话框表示单个聊天参与。 将其视为一个容器，其中包含与网站访客进行引人入胜的聊天对话框所需的所有内容。 在每个对话框中，您可以指定您希望对话框显示的页面、显示给哪个页面，以及对话框本身的内容和流程。 此外，您还可以找到一些量度以查看您的对话框的运行情况。 [了解有关对话框的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## 配置 {#configuration}

在“配置”选项卡中，自定义各种对话框的外观。 更改字体、颜色、响应时间等！ [了解有关配置的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}.

## 日程表 {#calendar}

连接你的Outlook或Gmail日历，以便在聊天机器人中的约会计划中使用。 [了解有关日历的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## 会议 {#meetings}

在这里，您可以看到网站访客通过各种对话框安排的所有约会。 [了解有关会议的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## 路由 {#routing}

在这里，您可以查看已连接其日历的所有代理的列表、它们向网站访客呈现的顺序以及创建自定义路由规则。 [了解有关路由的更多信息](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## 常见问题解答 {#faq}

**我是否可以在公司网站上的任何位置安装Dynamic Chat，或者它是否只能在Marketo登陆页面上工作？**

Dynamic ChatJavaScript代码片段可以安装在任何网站以及Marketo登陆页面上。

**数据会存储多长时间以用于报告？**

90天（参见完整的限制列表） [以下](#limits-in-dynamic-chat))。

**Dynamic Chat是否允许实时聊天？**

否，它仅利用预先确定的响应。

**Dynamic Chat支持英语以外的任何语言吗？**

是. Dynamic Chat支持以下语言：法语、德语、日语、西班牙语、意大利语、巴西葡萄牙语、朝鲜语、简体中文和繁体中文。 了解详情，请参阅 [以下部分](#changing-the-language).

**是否支持AI/NLP功能？**

我们不支持AI/NLP功能。

**我该如何定位匿名用户？**

在对话框中，您将需要使用 _人员电子邮件为空_ 属性。

## 更改语言 {#changing-the-language}

按照以下步骤更改Dynamic Chat语言。

>[!IMPORTANT]
>
>在配置文件级别更改您的语言将更改 _所有_ Experience Cloud应用程序，而不仅仅是Dynamic Chat。

1. 在您的Experience Cloud帐户中，单击设置图标，然后选择 **首选项**.

   ![](assets/dynamic-chat-overview-1.png)

1. 单击电子邮件地址下的当前语言。

   ![](assets/dynamic-chat-overview-2.png)

1. 选择您的新语言（第二种语言是可选的），然后单击 **保存**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >有几十种语言可供选择，但是，Dynamic Chat语仅支持以下语言：英语、法语、德语、日语、西班牙语、意大利语、巴西葡萄牙语、朝鲜语、简体中文和繁体中文。

当您更新语言时，除了您亲自填充的单词（例如，流响应）之外，应用程序本身中的所有内容都会更改。

## Dynamic Chat限制 {#limits-in-dynamic-chat}

<table>
  <th>参数</th>
  <th>描述</th>
  <th>限制</th>
 <tr>
  <td>对话框总数</td>
  <td>对话次数（已发布和草稿）</td>
  <td>500</td>
 </tr>
 <tr>
  <td>日历总数</td>
  <td>连接的日历数</td>
  <td>25</td>
 </tr>
 <tr>
  <td>用户总数（管理员和营销用户）</td>
  <td>每个Dynamic Chat实例允许的组合用户数</td>
  <td>50</td>
 </tr>
 <tr>
  <td>已发布对话框</td>
  <td>已保存的已发布对话框数</td>
  <td>100</td>
 </tr>
 <tr>
  <td>每个对话框的目标URL</td>
  <td>可添加到单个对话框的目标URL数量</td>
  <td>20</td>
 </tr>
 <tr>
  <td>每个对话框的属性</td>
  <td>可添加到单个对话框的受众条件的属性数量</td>
  <td>100</td>
 </tr>
 <tr>
  <td>组</td>
  <td>可添加到单个对话框的组数</td>
  <td>10</td>
 </tr>
 <tr>
  <td>每个组的属性</td>
  <td>可添加到组的属性数量</td>
  <td>10</td>
 </tr>
 <tr>
  <td>卡片</td>
  <td>每个对话框可以添加到画布的卡片数量</td>
  <td>500</td>
 </tr>
 <tr>
  <td>匿名潜在客户数据保留期</td>
  <td>未参与的任何匿名潜在客户的信息将保留多长时间</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>目标活动保留期</td>
  <td>目标活动数据的保留时间</td>
  <td>24个月</td>
 </tr>
 <tr>
  <td>文档活动保留期</td>
  <td>文档活动数据保留的时间</td>
  <td>24个月</td>
 </tr>
 <tr>
  <td>与对话框活动保留期交互</td>
  <td>与Dialog活动数据交互的保留时间</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>会议预订活动保留期</td>
  <td>会议预订活动将存储在Dynamic Chat中的时间</td>
  <td>24个月</td>
 </tr>
 <tr>
  <td>已参与的对话</td>
  <td>Web访客每月可参与的聊天会话数</td>
  <td>250</td>
 </tr>
 <tr>
  <td>已触发对话</td>
  <td>每月可向Web访客显示的聊天对话数</td>
  <td>25,000</td>
 </tr>
</table>
