---
unique-page-id: 4720275
description: 在Facebook中创建自定义受众 — Marketo文档 — 产品文档
title: 在Facebook中创建自定义受众
exl-id: a2c8d89c-16b3-44f6-a2c6-c52fe78ab39c
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 在Facebook中创建自定义受众 {#create-a-custom-audience-in-facebook}

>[!PREREQUISITES]
>
>* [将Facebook自定义受众添加为LaunchPoint服务](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md){target="_blank"} 在“管理员”部分中。
>* [接受Facebook的自定义受众术语](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} 在您的Facebook帐户中。

>[!TIP]
>
>详细了解 [facebook中的自定义受众](https://www.facebook.com/help/341425252616329){target="_blank"}.

1. 查找并选择智能或静态列表，其中包含要创建受众的潜在客户。

   ![](assets/create-a-custom-audience-in-facebook-1.png)

1. 选择 **潜在客户** 选项卡，然后单击 **通过Ad Bridge发送** 图标。

   ![](assets/create-a-custom-audience-in-facebook-2.png)

1. 选择 **facebook** 并单击 **下一个**.

   ![](assets/create-a-custom-audience-in-facebook-3.png)

1. 单击 **Audience** 下拉菜单并选择 **+新受众**.

   ![](assets/create-a-custom-audience-in-facebook-4.png)

   >[!IMPORTANT]
   >
   >facebook API允许每个Facebook广告帐户最多500个自定义受众。

1. 键入 **受众名称**. 单击 **更新**.

   ![](assets/create-a-custom-audience-in-facebook-5.png)

   >[!NOTE]
   >
   >如果您有多个Facebook广告帐户，您将看到一个额外的下拉列表，允许您选择创建此受众的广告帐户。

   >[!TIP]
   >
   >是否要将新受众与当前与广告集或组关联的现有受众进行交换？ 选择 **替换现有受众** 复选框。 这样做将 **非** 删除正在替换的受众。

1. 完成后，状态对话框将更新。

   ![](assets/create-a-custom-audience-in-facebook-6.png)

   就是这样！ 在Facebook中，您将在以下位置看到新受众 **广告管理器** > **受众**.

   ![](assets/create-a-custom-audience-in-facebook-7.png)

   >[!NOTE]
   >
   >您推送到Facebook的所有列表都将变为静态。 Marketo中的智能列表不会自动更新Facebook中的受众列表以反映传输后所做的任何更改。

   >[!TIP]
   >
   >请参阅 [面向Marketo客户的Facebook学习路径](https://facebook.exceedlms.com/student/enrollments/create_enrollment_from_token/BF9TqSaCvM73PP4ScjhCm4fi){target="_blank"}. 它涵盖了您需要了解的所有信息，从创建Facebook页面到使用Marketo的广告网络集成定向Facebook广告。

   >[!MORELIKETHIS]
   >
   >[在Facebook中将潜在客户添加到自定义受众](/help/marketo/product-docs/demand-generation/facebook/add-leads-to-a-custom-audience-in-facebook.md)
