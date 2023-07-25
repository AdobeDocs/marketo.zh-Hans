---
unique-page-id: 7513680
description: 自动提醒可能存在的重复人员 — Marketo文档 — 产品文档
title: 针对可能存在的重复人员自动发出警报
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 针对可能存在的重复人员自动发出警报 {#automate-an-alert-for-possible-duplicate-people}

是否希望每次创建可能的重复人员时都显示警报？ 以下是如何设置Smart Campaign来执行此操作。

1. [创建新的智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. 定义以下智能列表：

* 触发器： **[!UICONTROL 人员已创建]**
* 筛选条件： **[!UICONTROL 重复字段]**. 字段名称 **[!UICONTROL 是] [!UICONTROL 全名]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >发挥创造力。 对不同字段进行实验以获得更好的过滤结果。

1. 在流程步骤中，选择 [[!UICONTROL 发送警报]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} flow操作。

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >使用 [发送警报信息令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} 以包含指向您的CRM中的人员的链接。

   >[!CAUTION]
   >
   >如果导入一个大列表，您可能会一次收到大量此类警报！
   >
   >此外，两个同名人员不会自动表示他们是同一个人。

1. 在中激活营销活动 **[!UICONTROL 计划]** 选项卡。

   ![](assets/automate-an-alert-3.png)

就是这样！ 每次在Marketo中创建具有现有全名的新人员时，都会触发此智能营销活动。

>[!MORELIKETHIS]
>
>[查找并合并重复的人员](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
