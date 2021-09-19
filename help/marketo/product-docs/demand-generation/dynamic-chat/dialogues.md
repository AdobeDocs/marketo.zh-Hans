---
description: 对话框 — Marketo文档 — 产品文档
title: 对话框
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
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

有多个属性可供选择。 在本例中，我们选择的是“潜在客户州&#x200B;_是_&#x200B;加利福尼亚，而公司规模&#x200B;_大于_ 50。

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
>使用星号可充当通用通配符。 因此，`https://*.website.com`会在网站的每个页面上都放置对话框，包括子域(例如：support.website.com)。 `https://website.com/folder/*`会将对话框置于后续文件夹中的每个HTML页面(例如：在本例中，假设文件夹为“sports”，因此：website.com/sports/baseball.html、website.com/sports/football.html等)。
