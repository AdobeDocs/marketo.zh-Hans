---
description: 受众标准 — Marketo文档 — 产品文档
title: 受众标准
feature: Dynamic Chat
exl-id: 95c4558e-0c0c-4623-bb7d-b6ac2f455c01
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 1%

---

# 受众标准 {#audience-criteria}

与Marketo Engage智能列表类似，受众标准属性允许您定义目标受众。 您可以使用推断的、人员或公司属性（或它们的组合）定位已知或未知人员。

## 优先级 {#priority}

优先级确定在符合多个对话框资格的情况下，潜在客户将收到哪个对话框。 它是您首次[创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}时创建的。 您可以通过打开现有对话框并转到“受众条件”选项卡中的&#x200B;**[!UICONTROL Dialogue Details]**&#x200B;来更改其优先级。

![](assets/audience-criteria-1.png)

## 事件 {#events}

事件允许您根据访客滚动多少或他们在您的页面/网站上的时间长短来定位访客。 在以下示例中，我们的定位是在特定页面上停留超过20秒的访客。

1. 抓取&#x200B;**[!UICONTROL Time on Page]**&#x200B;事件并将其拖动到右侧。

   ![](assets/audience-criteria-3.png)

1. 将“[!UICONTROL Greater Than]”时间设置为20秒。

   ![](assets/audience-criteria-4.png)

1. 在[[!UICONTROL Target]](#target)部分中添加所需页面的URL。

   ![](assets/audience-criteria-5.png)

## 属性 {#attributes}

**已知人员**

有&#x200B;_多个_&#x200B;属性组合可供选择。 在下面的示例中，我们定位了在加利福尼亚州一家拥有50名以上员工的公司工作的所有已知人员。

1. 获取&#x200B;**[!UICONTROL Person State]**&#x200B;属性并将其拖动到右侧。

   ![](assets/audience-criteria-7.png)

1. 默认情况下已设置&#x200B;_[!UICONTROL Is]_。 在选择值字段中，键入CA（您还可以单击下拉菜单并从列表中选择）。

   ![](assets/audience-criteria-8.png)

1. 获取&#x200B;**[!UICONTROL Company Size]**&#x200B;属性并将其拖到显示&#x200B;_将属性拖放到此处_&#x200B;的位置。

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >您还可以通过单击属性的&#x200B;**+**&#x200B;图标来选择属性。

1. 单击运算符下拉列表并选择&#x200B;**[!UICONTROL Greater Than]**。

   ![](assets/audience-criteria-10.png)

1. 键入50并单击屏幕上的其他位置进行保存。

   ![](assets/audience-criteria-11.png)

就是这样！

**匿名人员**

有一种简便的方法可以专门定向尚未出现在数据库中的用户。 在此示例中，我们定位了位于纽约区域的所有匿名人员。

1. 获取&#x200B;**[!UICONTROL Person Email]**&#x200B;属性并将其拖动到右侧。

   ![](assets/audience-criteria-12.png)

1. 单击运算符下拉列表并选择&#x200B;**[!UICONTROL Is Empty]**。

   ![](assets/audience-criteria-13.png)

1. 获取&#x200B;**[!UICONTROL Inferred State]**&#x200B;属性并将其拖到显示&#x200B;_将属性拖放到此处_&#x200B;的位置。

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >当有人访问您的网站时，[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}会对其进行Cookie并将其放入系统中。 我们在一个特殊的数据库中查找他们的IP，并推断出各种好的信息。

1. 默认情况下已设置&#x200B;_[!UICONTROL Is]_。 在选择值字段中，键入NY （您还可以单击下拉菜单并从列表中选择）。

   ![](assets/audience-criteria-15.png)

## 会员资格 {#membership}

将Marketo Engage智能列表用于对话框的目标受众。

>[!AVAILABILITY]
>
>“智能列表成员”或“列表成员”条件需要Dynamic Chat Prime。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

1. 在成员身份下，获取&#x200B;**[!UICONTROL Member of Smart List]**&#x200B;并将其放到画布上。

   ![](assets/audience-criteria-15a.png)

1. 选择所需的智能列表。

   ![](assets/audience-criteria-15b.png)

## 添加组 {#add-groups}

如果您希望具有所有特定属性以及其他的“所有或任何”属性，也可以选择对属性进行分组。 您可以添加多个组。

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Target {#target}

您可以在此处输入希望特定对话框显示的URL。 您还可以选择添加排除项。

可接受的格式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>* 使用星号就像一个全面的通配符。 因此，`https://*.website.com`将对话框置于网站的每个页面上，包括子域（例如： `support.website.com`）。 `https://website.com/folder/*`会将对话框放置到后续文件夹中的每个HTML页面上(例如：在此示例中，假设文件夹为“sports”，如：website.com/sports/baseball.html、website.com/sports/football.html等)。
>
>* 目前不支持URL参数。

**排除项**

使用排除项确保您的对话框&#x200B;_不_&#x200B;出现在网站的特定页面/区域。 排除项遵循与包含项相同的格式。

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Designer流](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}
