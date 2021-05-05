---
description: 过滤电子邮件活动- Marketo文档 — 产品文档
title: 过滤电子邮件机器人活动
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# 过滤电子邮件活动{#filtering-email-bot-activity}

有时，电子邮件程序活动会错误地夸大电子邮件的打开次数和点击数据。 下面介绍如何解决这个问题。

>[!NOTE]
>
>使用[IAB/ABC International Spiders and Bots列表](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/)，所有与IP或用户代理(与该列表中的任何内容匹配)的打开/单击活动都将标识为bot活动，且不会登录Marketo。

1. 单击&#x200B;**管理员**。

   ![](assets/filtering-email-bot-activity-1.png)

1. 单击&#x200B;**电子邮件**。

   ![](assets/filtering-email-bot-activity-2.png)

1. 单击&#x200B;**机器人活动**&#x200B;选项卡。

   ![](assets/filtering-email-bot-activity-3.png)

1. 选中&#x200B;**启用电子邮件活动筛选**&#x200B;复选框。

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>启用此功能后，您可能会看到打开电子邮件并单击，因为过滤掉了假数。

**可选步骤**:要禁用该功能，只需取消选中该复选框。如果禁用，则“Bot 活动 in last 90 days”数据&#x200B;**不会**&#x200B;重置。
