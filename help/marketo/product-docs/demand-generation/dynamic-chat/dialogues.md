---
description: 对话框 — Marketo文档 — 产品文档
title: 对话框
exl-id: 5ec17ad0-6d56-4c06-a6ac-4c5771b2d91d
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 对话框 {#dialogues}

对话是单独的聊天对话。 了解如何以可视方式自定义页面、确定页面显示内容，以及决定说什么以及看到内容的人。

## 创建新对话框 {#create-a-new-dialogue}

1. 单击 **对话框**.

   ![](assets/dialogues-1.png)

1. 单击 **新建** 按钮。

   ![](assets/dialogues-2.png)

1. 输入名称（说明是可选的），设置优先级级别，然后单击 **保存**.

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>优先级决定了访客同时符合多个对话框的条件时将向其显示哪个对话框。

## 受众标准 {#audience-criteria}

与Marketo智能列表类似，受众标准属性允许您定义目标受众。 您可以使用推断出的、人员或公司属性（或其组合）来定位已知或未知的人员。

**已知人员**

有 _许多_ 属性组合进行选择。 在本例中，我们定位了所有 **已知人员** 在一家员工超过50人的公司工作。

1. 抓住 **人员状态** 属性并将其拖动到右侧。

   ![](assets/dialogues-4.png)

1. _是_ 设置。 在选择值字段中，键入CA（您还可以单击下拉菜单并从列表中选择）。

   ![](assets/dialogues-5.png)

1. 抓住 **公司规模** 属性并将其拖动到其中显示的位置 _在此处拖放属性_.

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >您还可以通过单击 **+** 图标。

1. 单击运算符下拉列表，然后选择 **大于**.

   ![](assets/dialogues-7.png)

1. 键入50，然后单击屏幕上的其他位置进行保存。

   ![](assets/dialogues-8.png)

就这样！

**匿名人员**

有一种简单的方法可以专门定位尚未在数据库中的人员。 在本例中，我们定位了所有 **匿名人员** 在纽约地区。

1. 抓住 **人员电子邮件** 属性并将其拖动到右侧。

   ![](assets/dialogues-9.png)

1. 单击运算符下拉列表，然后选择 **为空**.

   ![](assets/dialogues-10.png)

1. 抓住 **推断状态** 属性并将其拖动到其中显示的位置 _在此处拖放属性_.

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >当有人访问您的网站时， [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 给他们点饼干，然后放到系统中。 我们在一个特殊的数据库中查找他们的IP信息，并推断出各种好信息。

1. _是_ 设置。 在选择值字段中，键入NY（您也可以单击下拉菜单并从列表中选择）。

   ![](assets/dialogues-12.png)

## 添加群组 {#add-groups}

如果您希望具有所有特定属性以及“全部或任意”其他属性，则还可以选择对属性进行分组。 您可以添加多个群组。

![](assets/dialogues-13.png)

![](assets/dialogues-14.png)

## Target {#target}

在这里，您可以输入希望显示特定对话框的URL。

可接受的格式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>使用星号可充当通用通配符。 所以 `https://*.website.com` 会在网站的每个页面上都放置对话框，包括子域(例如： `support.website.com`)。 和 `https://website.com/folder/*` 会将对话框置于后续文件夹中的每个HTML页面(例如：在本例中，假设文件夹为“sports”，因此：website.com/sports/baseball.html、website.com/sports/football.html等)。

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
  <td>为访客提供可用日期的日历以安排后续活动。 日历可用性反映 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">下一位代理排队</a>.</td>
 </tr>
 <tr>
  <td><strong>意愿</strong></td>
  <td>这是访客看不到的唯一一张卡。 您可以确定在特定聊天中的哪个时间点实现目标(例如：如果您的目标是收集访客的电子邮件，请将目标卡片放在流中信息捕获之后立即放置。)</td>
 </tr>
</table>

**创建流**

有 _许多_ 可能的流组合。 让我们看一个示例 [在本文中](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md).

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
  <td><strong>已捕获人员</strong></td>
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

>[!MORELIKETHIS]
>
>[创建流](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md)
