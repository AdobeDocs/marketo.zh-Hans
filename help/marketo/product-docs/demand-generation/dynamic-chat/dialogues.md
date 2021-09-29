---
description: 对话框 — Marketo文档 — 产品文档
title: 对话框
hide: true
hidefromtoc: true
source-git-commit: fe4a4b89ee295d8e351587a5ac858806a83f1305
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 对话框 {#dialogues}

对话是单独的聊天对话。 了解如何以可视方式自定义页面、确定页面显示内容，以及决定说什么以及看到内容的人。

## 创建新对话框 {#create-a-new-dialogue}

1. 单击&#x200B;**对话框**。

   ![](assets/dialogues-1.png)

1. 单击&#x200B;**新建**&#x200B;按钮。

   ![](assets/dialogues-2.png)

1. 输入名称（说明是可选的），设置优先级级别，然后单击&#x200B;**Save**。

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>优先级决定了访客同时符合多个对话框的条件时将向其显示哪个对话框。

## 受众标准 {#audience-criteria}

与Marketo智能列表类似，受众标准属性允许您定义目标受众。 您可以使用推断出的、潜在客户或公司属性（或其组合）来定位已知或未知的潜在客户。

**已知潜在客户**

有许多&#x200B;_属性组合可供选择。_&#x200B;在此示例中，我们定位的是加利福尼亚州所有在公司工作且员工超过50名的&#x200B;**已知潜在客户**。

1. 抓取&#x200B;**Lead State**&#x200B;属性并将其拖动到右侧。

   ![](assets/dialogues-4.png)

1. __ 默认设置Isis。在选择值字段中，键入CA（您还可以单击下拉菜单并从列表中选择）。

   ![](assets/dialogues-5.png)

1. 抓取&#x200B;**公司大小**&#x200B;属性，并将其拖动到其显示&#x200B;_的位置，在此处拖放属性_。

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >您还可以通过单击属性的&#x200B;**+**&#x200B;图标来选择属性。

1. 单击运算符下拉列表，然后选择&#x200B;**大于**。

   ![](assets/dialogues-7.png)

1. 键入50，然后单击屏幕上的其他位置进行保存。

   ![](assets/dialogues-8.png)

**匿名潜在客户**

有一种简单的方法可以专门定位尚未在数据库中的潜在客户。 在此示例中，我们定向位于纽约地区的所有&#x200B;**匿名潜在客户**。

1. 获取&#x200B;**潜在客户电子邮件**&#x200B;属性，并将其拖动到右侧。

   ![](assets/dialogues-9.png)

1. 单击运算符下拉列表，然后选择&#x200B;**Is Empty**。

   ![](assets/dialogues-10.png)

1. 抓取&#x200B;**Intercuted State**&#x200B;属性，并将其拖动到其显示&#x200B;_的位置，在此处拖放属性_。

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >当某人访问您的网站时， [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)会将其cookie并放入系统中。 我们在一个特殊的数据库中查找他们的IP，并推断出各种好信息。

1. __ 默认设置Isis。在选择值字段中，键入NY（您也可以单击下拉菜单并从列表中选择）。

   ![](assets/dialogues-12.png)

## 添加群组 {#add-groups}

如果您希望具有所有特定属性以及其他属性的“任意”，则还可以选择对属性进行分组。

完成此操作

## Target {#target}

在这里，您可以输入希望显示特定对话框的URL。

可接受的格式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>使用星号可充当通用通配符。 因此，`https://*.website.com`会在网站的每个页面上都放置对话框，包括子域(例如：`support.website.com`)。 `https://website.com/folder/*`会将对话框置于后续文件夹中的每个HTML页面(例如：在本例中，假设文件夹为“sports”，因此：website.com/sports/baseball.html、website.com/sports/football.html等)。

## 流设计器 {#stream-designer}

流设计器包含您可以添加的不同卡片，以塑造聊天对话。

<table>
 <tr>
  <td><strong>消息</strong></td>
  <td>当您想要做出无需响应的语句时使用(例如：“嗨！ 所有项目现在都优惠25%，代码为SAVE25”)。
</td>
 </tr>
 <tr>
  <td><strong>问题</strong></td>
  <td>当您想要提出多选问题时，可使用该问题提供可用的响应(例如：你对哪种车感兴趣？ 响应= SUV、紧凑型、卡车等)。</td>
 </tr>
 <tr>
  <td><strong>信息捕获</strong></td>
  <td>在要收集信息时使用。 要选择的三个字段是“电子邮件地址”、“电话号码”和“文本”（允许访客自行编写消息）。</td>
 </tr>
 <tr>
  <td><strong>日程安排计划程序</strong></td>
  <td>为访客提供可用日期的日历以安排后续活动。 日历可用性反映[下一个代理在行](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing)。</td>
 </tr>
 <tr>
  <td><strong>意愿</strong></td>
  <td>这是访客看不到的唯一一张卡。 您可以确定在特定聊天中的哪个时间点实现目标(例如：如果您的目标是收集访客的电子邮件，请将目标卡片放在流中信息捕获之后)。</td>
 </tr>
</table>

**创建流**

要创建的流组合有&#x200B;_许多_。 在本例中，我们将提出是或否问题，并准备一些响应。

示例

## 报表 {#reports}

在“报表”选项卡中，查看过去90天的数据。 每个类别在下面进行定义。

<table>
 <tr>
  <td><strong>触发总数</strong></td>
  <td>每当访客符合条件/显示对话框时，都会递增。
</td>
 </tr>
 <tr>
  <td><strong>已参与</strong></td>
  <td>每当访客单击聊天机器人锚点以打开对话框时，都会递增。</td>
 </tr>
 <tr>
  <td><strong>已完成</strong></td>
  <td>访客每次到达对话框中任何分支的结尾时递增。</td>
 </tr>
 <tr>
  <td><strong>捕获的商机</strong></td>
  <td>在对话框中，访客每次提供有效的电子邮件地址时，都会递增。</td>
 </tr>
 <tr>
  <td><strong>已预订的会议</strong></td>
  <td>每次访客通过聊天机器人成功计划约会时，都会递增。</td>
 </tr>
 <tr>
  <td><strong>实现的目标</strong></td>
  <td>在任何对话框流中，当访客达到目标时递增。</td>
 </tr>
</table>
