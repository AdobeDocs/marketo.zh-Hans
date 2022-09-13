---
description: 过滤电子邮件机器人活动 — Marketo文档 — 产品文档
title: 筛选电子邮件机器人活动
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 2fd0856e21c51af6ca29887978d5aa946733405d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 筛选电子邮件机器人活动 {#filtering-email-bot-activity}

有时，电子邮件机器人活动可能会错误地使电子邮件打开数和点击数数据虚增。 请按照以下步骤进行修复。

我们使用三种不同的方法来确认机器人活动：

* 匹配 [交互式广告局机器人列表](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;}:与IAB UA/IP（用户代理/IP地址）列表上的任何内容匹配的活动将标记为机器人。
* 与邻近模式匹配：当同时发生两个以上的活动时（在两秒内），它们将被识别为机器人。

针对电子邮件链接点击和电子邮件打开活动，新属性将填充以下值：

* 被识别为机器人的活动将具有“机器人活动”作为“True”，“机器人活动模式”作为已识别的模式/方法
* 被标识为非机器人的活动将“机器人活动”设置为“False”，“机器人活动模式”设置为“N/A”
* 在我们引入这些属性之前发生的活动将具有“机器人活动”作为“ ”（空），“机器人活动模式”作为“ ”（空）

1. 单击 **管理员**.

   ![](assets/filtering-email-bot-activity-1.png)

1. 单击 **电子邮件**.

   ![](assets/filtering-email-bot-activity-2.png)

1. 单击 **机器人活动** 选项卡。

   ![](assets/filtering-email-bot-activity-3.png)

1. 选择 **与IAB列表匹配**, **与邻近模式匹配**，或两者兼有。 选择是否记录机器人活动 _或_ 过滤机器人活动。

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>如果选择过滤机器人活动，您可能会在电子邮件打开数中看到一个下拉消息，并在删除假活动时单击该消息。

**可选步骤**:要禁用此功能，只需取消选择滑块即可。 如果禁用，则数据不会重置。

>[!TIP]
>
>通过“电子邮件中的点击链接”和“打开电子邮件”过滤器中的“是/否”布尔值（“是”/“否”）和“机器人活动模式”，以及“电子邮件中的点击链接”和“打开电子邮件”触发器，利用智能列表中的机器人活动数据。
