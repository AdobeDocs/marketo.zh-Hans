---
description: 受众标准 — Marketo文档 — 产品文档
title: 受众标准
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
source-git-commit: f71ac0398b3a93d2c46201a696dd41e6ccd89000
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# 受众标准 {#audience-criteria}

与Marketo智能列表类似，受众标准属性允许您定义目标受众。 您可以使用推断出的、人员或公司属性（或其组合）来定位已知或未知的人员。

## 优先级 {#priority}

优先级决定潜在客户在符合多个对话框资格时收到的对话框。 它是在你第一次 [创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}。 您可以通过打开现有对话框并转到 **对话框详细信息** （在受众标准选项卡中）。

![](assets/audience-criteria-1.png)

## 事件 {#events}

![](assets/audience-criteria-2.png)

利用事件，可根据访客的滚动量或页面/网站上的时长来定位访客。 在以下示例中，我们定位的是在特定页面上停留超过20秒的访客。

1. 抓住 **页面逗留时间** 事件并将其拖动到右侧。

   ![](assets/audience-criteria-3.png)

1. 将“大于”时间设置为20秒。

   ![](assets/audience-criteria-4.png)

1. 在 [Target](#target) 中。

   ![](assets/audience-criteria-5.png)

## 属性 {#attributes}

![](assets/audience-criteria-6.png)

**已知人员**

有 _许多_ 属性组合进行选择。 在以下示例中，我们定位了所有 **已知人员** 在一家员工超过50人的公司工作。

1. 抓住 **人员状态** 属性并将其拖动到右侧。

   ![](assets/audience-criteria-7.png)

1. _是_ 设置。 在选择值字段中，键入CA（您还可以单击下拉菜单并从列表中选择）。

   ![](assets/audience-criteria-8.png)

1. 抓住 **公司规模** 属性并将其拖动到其中显示的位置 _在此处拖放属性_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >您还可以通过单击 **+** 图标。

1. 单击运算符下拉列表，然后选择 **大于**.

   ![](assets/audience-criteria-10.png)

1. 键入50，然后单击屏幕上的其他位置进行保存。

   ![](assets/audience-criteria-11.png)

就这样！

**匿名人员**

有一种简单的方法可以专门定位尚未在数据库中的人员。 在本例中，我们定位了所有 **匿名人员** 在纽约地区。

1. 抓住 **人员电子邮件** 属性并将其拖动到右侧。

   ![](assets/audience-criteria-12.png)

1. 单击运算符下拉列表，然后选择 **为空**.

   ![](assets/audience-criteria-13.png)

1. 抓住 **推断状态** 属性并将其拖动到其中显示的位置 _在此处拖放属性_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >当有人访问您的网站时， [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 给他们点饼干，然后放到系统中。 我们在一个特殊的数据库中查找他们的IP信息，并推断出各种好信息。

1. _是_ 设置。 在选择值字段中，键入NY（您也可以单击下拉菜单并从列表中选择）。

   ![](assets/audience-criteria-15.png)

## 添加群组 {#add-groups}

如果您希望具有所有特定属性以及“全部或任意”其他属性，则还可以选择对属性进行分组。 您可以添加多个群组。

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## 目标 {#target}

在这里，您可以输入希望显示特定对话框的URL。 您还可以选择添加排除项。

可接受的格式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>使用星号可充当通用通配符。 所以 `https://*.website.com` 会在网站的每个页面上都放置对话框，包括子域(例如： `support.website.com`)。 和 `https://website.com/folder/*` 会将对话框置于后续文件夹中的每个HTML页面(例如：在本例中，假设文件夹为“sports”，因此：website.com/sports/baseball.html、website.com/sports/football.html等)。

**排除项**

使用排除项确保对话框已执行 **not** 显示在网站的特定页面/区域上。 排除项与包含项的格式相同。

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [流设计器](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [报表](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

