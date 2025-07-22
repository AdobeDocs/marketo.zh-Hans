---
unique-page-id: 2953373
description: 在Marketo Sales Insight - Marketo文档中配置取消订阅页脚 — 产品文档
title: 在Marketo Sales Insight中配置取消订阅页脚
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 在[!DNL Marketo Sales Insight]中配置取消订阅页脚 {#configure-unsubscribe-footers-in-marketo-sales-insight}

销售电子邮件会自动将取消订阅页脚放在底部。 但是，您可以根据自己的需要调整设置。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>**定义**
>
>**销售电子邮件**&#x200B;是从[!DNL Sales Insight]发送的电子邮件(不包括从Marketo Outlook插件发送的电子邮件)。

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;区域。

   ![](assets/one-1.png)

1. 单击&#x200B;**[!UICONTROL Sales Insight]**，然后单击&#x200B;**[!UICONTROL Edit Settings]**。

   ![](assets/two-1.png)

   有几个选项。 首先，我们看一下您可以更改其设置的电子邮件类型。

   ![](assets/three-1.png)

   * **[!UICONTROL No Template]** — 由销售用户手动撰写。
   * **[!UICONTROL Standard Email]** — 基于模板的电子邮件。
   * **[!UICONTROL Operational Email]** — 忽略已取消订阅、营销已暂停和通信限制的电子邮件（无论发送什么邮件）。

   您可以选择为每个类型设置不同的行为。

   >[!CAUTION]
   >
   >**[!UICONTROL Respect Unsubscribe Settings]**：即使发布的电子邮件是“可操作的”，取消订阅的潜在客户也不会收到电子邮件
   >
   >**[!UICONTROL Ignore Unsubscribe Settings]**：取消订阅的潜在客户将收到电子邮件

1. 进行所需的更改，然后单击&#x200B;**[!UICONTROL Save]**。

   >[!TIP]
   >
   >最后两个选项允许您根据收件人数量（大于1或大于5）动态包含/排除取消订阅页脚。

   ![](assets/four-1.png)

哇！ 有点复杂，但很灵活，对吧？
