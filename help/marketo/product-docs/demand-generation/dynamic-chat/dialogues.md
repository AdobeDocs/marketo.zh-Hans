---
description: 对话框 — Marketo文档 — 产品文档
title: 对话框
hide: true
hidefromtoc: true
source-git-commit: 1a1d4cb7e013253ce7189150486ba03ea02d877d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 对话框 {#dialogues}

对话框是您设置的特定聊天对话。 它们可以按外观以及说的内容和看到者进行定制。

## 创建新对话框 {#create-a-new-dialogue}

1. 单击&#x200B;**对话框**。

PICC

1. 单击&#x200B;**新建**&#x200B;按钮。

PICC

1. 输入名称（说明是可选的），设置优先级级别，然后单击&#x200B;**Save**。

PICC

>[!NOTE]
>
>说明优先级

## 受众标准 {#audience-criteria}

与Marketo智能列表类似，受众标准属性允许您定义目标受众。

有多个属性可供选择。 在此示例中，我们定位的是加利福尼亚州所有在公司工作且员工超过50名的已知潜在客户。

1. 抓取“潜在客户状态”属性并将其拖动到右侧。

PICC

1. __ 默认设置Isis。在选择值字段中，键入CA（您还可以单击下拉菜单并从列表中选择）。

PICC

1. 抓取“公司规模”属性并将其拖动到右侧。

PICC

1. 单击运算符下拉列表，然后选择大于。

PICC

1. 键入50，然后单击屏幕上的其他位置进行保存。

PICC

如何捕获ANON潜在客户

注意 — 可能提到推断为何使用/显示用例时，潜在客户电子邮件为空

## 添加群组 {#add-groups}

如果您希望具有所有特定属性以及其他属性的“任意”，则还可以选择对属性进行分组。

完成此操作

## Target {#target}

在这里，您可以输入希望显示特定对话框的特定URL。

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

表

消息：当您想要做出无需响应的语句时使用(例如：“嗨！ 所有项目现在都优惠25%，代码为SAVE25。”)

问题：当您想要提出多选问题时，可使用该问题提供可用的响应(例如：你对哪种车感兴趣？ 响应= SUV、紧凑型、卡车等)

信息捕获：在要收集信息时使用。 要选择的三个字段是“电子邮件地址”、“电话号码”和“文本”（允许访客自行编写消息）。

日程安排计划程序：为访客提供可用日期的日历以安排后续活动。 日历可用性反映了[行](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing)中的下一个代理。

目标：这是访客看不到的唯一一张卡。 您可以确定在特定聊天中的哪个时间点实现目标(例如：如果您的目标是收集访客的电子邮件，请将目标卡放在流中信息捕获之后。)

可能属于自己的部分

显示下面的示例