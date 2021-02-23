---
unique-page-id: 7505310
description: 订阅智能列表- Marketo Docs — 产品文档
title: 订阅智能列表
translation-type: tm+mt
source-git-commit: 03ee7b69f691efce12825aa708c81dffa23cecd9
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---


# 订阅智能列表{#subscribe-to-a-smart-list}

订阅智能列表是跟踪人员、将报告直接发送到收件箱的绝佳方式。

您可以在两个不同的位置创建智能列表订阅:

* 营销活动
* 数据库

订阅在运行订阅时使用完整的列表。

订阅可以在营销活动或数据库中使用智能列表所处的位置。

您可以从同一智能订阅创建多个列表。

订阅特定于工作区。 例如，此列表的订阅与本文其余部分中显示的工作区不同：

![](assets/one.png)

>[!NOTE]
>
>每个Marketo实例在不同工作区内限制为100个订阅，每个订阅最多限制为100,000人。 如果智能列表包含的名称超过100,000个，Marketo将为前100,000个运行订阅。

## 创建智能列表订阅{#create-a-smart-list-subscription}

1. 转到&#x200B;**Database**&#x200B;或&#x200B;**营销活动**。

   ![](assets/db.png)

1. 选择要为其创建列表的智能订阅。 单击&#x200B;**列表操作**&#x200B;并选择&#x200B;**新建智能列表订阅**。

   ![](assets/three.png)

1. 为您的订阅提供&#x200B;**名称**，然后选择或输入&#x200B;**收件人**&#x200B;的电子邮件地址。

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. 单击&#x200B;**Frequency**&#x200B;列表并选择一个频率。

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. 设置&#x200B;**结束投放**&#x200B;日期。 您可以选择&#x200B;**从不**&#x200B;或日历日期。

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. 单击&#x200B;**格式**&#x200B;并从列表中进行选择。

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. 单击&#x200B;**创建**。

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. 您的新智能列表订阅将显示在列表顶部的“订阅”选项卡中。 如果要立即发送，请单击&#x200B;**发送**，并且等到预定的电子邮件投放。

   ![](assets/eight.png)

1. 我们建议您清除“活动”复选框，以在没有订阅智能列表订阅时停用该智能订阅。

   ![](assets/nine.png)

   那很容易，不是吗？

## 电子邮件{#email-message}

收件人将收到一封电子邮件，其中包含下载报告的选项，以及指向Marketo实例中列表的直接链接。 下载链接将在四天后过期。

>[!NOTE]
>
>如果将[安全订阅管理员](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)设置设置为&#x200B;**是**，则只有有权访问Marketo实例的人员才能下载报告。

![](assets/image2015-4-17-15-3a46-3a47.png)

如果报表包含0个人，收件人仍会收到电子邮件。 但是，该电子邮件只是说，没有人可以报告。

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>修改基于列表的智能订阅过滤器时，也会更新报表。

该电子邮件还提供了有关用于创建列表的过滤器的其他信息。

## 删除订阅{#delete-a-subscription}

要删除订阅，请在“订阅”选项卡中选择该订阅，然后单击“删除”。

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [编辑智能列表订阅](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [保护订阅管理设置](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)

