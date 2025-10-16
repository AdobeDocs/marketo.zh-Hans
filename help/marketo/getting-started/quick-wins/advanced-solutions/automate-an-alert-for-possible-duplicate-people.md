---
unique-page-id: 7513680
description: 自动提醒可能重复的人员 — Marketo文档 — 产品文档
title: 自动提醒可能的重复人员
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 10%

---

# 自动提醒可能的重复人员 {#automate-an-alert-for-possible-duplicate-people}

是否希望每次创建可能的重复人员时都显示警报？ 下面是如何设置Smart Campaign来执行此操作。

1. [创建新的智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}。 定义以下智能列表：

* 触发器： **[!UICONTROL Person is Created]**
* 筛选器： **[!UICONTROL Duplicate Fields]**。 字段名称&#x200B;**[!UICONTROL is]&#x200B;[!UICONTROL Full Name]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >发挥创造力。 对不同字段进行实验，获得更好的过滤效果。

1. 在流程步骤中，选择[[!UICONTROL Send Alert]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"}流程操作。

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >使用[发送警报信息令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}在CRM中包含指向此人的链接。

   >[!CAUTION]
   >
   >如果导入一个大列表，您可能会一次收到一栈此类警报！
   >
   >此外，两个同名的人并不自动意味着他们是同一个人。

1. 在&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡中激活该营销活动。

   ![](assets/automate-an-alert-3.png)

操作完成！每次在Marketo中创建具有现有全名的新人员时，此智能营销活动都会触发。

>[!MORELIKETHIS]
>
>[查找并合并重复的人员](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
