---
description: 过滤电子邮件机器人活动 — Marketo文档 — 产品文档
title: 筛选电子邮件机器人活动
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 筛选电子邮件机器人活动 {#filtering-email-bot-activity}

有时，电子邮件机器人活动可能会错误地使电子邮件打开数和点击数数据虚增。 这是如何解决的。

>[!NOTE]
>
>使用 [IAB/ABC国际蜘蛛程序和机器人列表](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/)，则所有包含IP或用户代理的打开/单击活动（与该列表中的任何内容匹配）都将被标识为机器人活动，且不会登录Marketo。

1. 单击 **管理员**.

   ![](assets/filtering-email-bot-activity-1.png)

1. 单击 **电子邮件**.

   ![](assets/filtering-email-bot-activity-2.png)

1. 单击 **机器人活动** 选项卡。

   ![](assets/filtering-email-bot-activity-3.png)

1. 单击滑块以启用 **过滤机器人活动**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>您可以单独选择是否记录机器人活动。 如果您选择不启用，您可能会看到电子邮件打开数量骤减，并且点击次数会被过滤掉，因为假数字会被过滤掉。

**可选步骤**:要禁用该功能，只需取消选择滑块。 如果禁用，则“过去90天内的机器人活动”数据会禁用 **not** 重置。

>[!TIP]
>
>在智能列表中通过“是机器人活动”布尔值（是/否）或在适用的过滤器/触发器约束中利用机器人活动数据。
