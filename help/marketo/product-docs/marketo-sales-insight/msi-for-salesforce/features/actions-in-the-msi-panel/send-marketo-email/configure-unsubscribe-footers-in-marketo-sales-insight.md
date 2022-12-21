---
unique-page-id: 2953373
description: 在Marketo Sales Insight - Marketo文档 — 产品文档中配置取消订阅页脚
title: 在Marketo Sales Insight中配置取消订阅页脚
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 在Marketo Sales Insight中配置取消订阅页脚 {#configure-unsubscribe-footers-in-marketo-sales-insight}

销售电子邮件会自动将取消订阅页脚放在底部。 但是，您可以根据需要调整设置。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>**条件**
>
>**销售电子邮件** 是从Sales Insight发送的变量(不包括从Marketo Outlook插件发送的变量)。

1. 转到 **管理员** 的上界。

   ![](assets/one-1.png)

1. 单击 **销售分析**，则 **编辑设置**.

   ![](assets/two-1.png)

   有几个选项。 首先，让我们看一看您可以更改其设置的电子邮件类型。

   ![](assets/three-1.png)

   * **无模板**  — 由销售用户手动合成。
   * **标准电子邮件**  — 基于模板的电子邮件。
   * **操作电子邮件**  — 忽略未订阅、暂停营销和通信限制的电子邮件（无论如何发送）。

   您可以选择为每个类型设置不同的行为。

   >[!CAUTION]
   >
   >**遵循取消订阅设置**:即使已发布的电子邮件“可操作”，未订阅的潜在客户也不会收到电子邮件
   >
   >**忽略取消订阅设置**:未订阅的潜在客户将收到电子邮件

1. 进行所需的更改，然后单击 **保存**.

   >[!TIP]
   >
   >最后两个选项允许您根据收件人的数量（大于1或大于5）动态包含/排除取消订阅的页脚。

   ![](assets/four-1.png)

哇！ 有点复杂，但很灵活，对吧？
