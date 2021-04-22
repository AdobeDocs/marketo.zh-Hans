---
unique-page-id: 7513680
description: 自动发出警报以发现可能的重复— Marketo Docs — 产品文档
title: 自动警报可能的重复
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 自动警报可能的重复{#automate-an-alert-for-possible-duplicate-people}

是否希望在每次可能创建重复人时发出警报？ 下面介绍如何设置智能活动来完成此操作。

1. [创建新的智能活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。定义以下智能列表:

* 触发器：**已创建人**
* 过滤器：**重复字段。** 字段名 **称为全名**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >发挥创意。 用不同的场进行实验，获得更好的滤波效果。

1. 在流步骤中，选择[发送警报](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)流操作。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >使用[发送警报信息令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md)在CRM中包含指向该人员的链接。

   >[!CAUTION]
   >
   >如果导入大列表，您可能会同时获得大量这些警报！
   >
   >另外，两个名字相同的人并不自动意味着他们是同一个人。

1. 在&#x200B;**活动**&#x200B;选项卡中激活计划。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

就这样！ 每次在Marketo中创建具有现有全名的新人时，此智能活动都将触发。

>[!MORELIKETHIS]
>
>[查找并合并重复人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
