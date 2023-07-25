---
unique-page-id: 6095008
description: '"添加 [!DNL Google AdWords] as a [!DNL LaunchPoint] 服务 — Marketo文档 — 产品文档”'
title: '"添加 [!DNL Google AdWords] as a [!DNL LaunchPoint] 服务”'
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# 添加 [!DNL Google AdWords] as a [!DNL LaunchPoint] 服务 {#add-google-adwords-as-a-launchpoint-service}

关联您的 [!DNL Google AdWords] 帐户到Marketo以自动将离线转化数据从Marketo上传到 [!DNL Google AdWords]. 然后，从 [!DNL AdWords] 在UI中，您将能够轻松地看到哪些点击导致了符合条件的潜在客户、机会和新客户（或您希望跟踪的任何收入阶段） [添加自定义列](https://support.google.com/adwords/answer/3073556){target="_blank"} 在 [!DNL AdWords]. 此信息不会显示在Marketo UI中。

详细了解 [Google的脱机转换导入功能](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>并非所有客户都已购买此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>您还可以集成 [[!DNL Google AdWords] as a [!DNL Launchpoint] 经理帐户服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}.

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. 选择 **[!UICONTROL 启动点]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. 选择 **[!UICONTROL 新]** 和 **[!UICONTROL 新服务]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. 输入 [!UICONTROL 显示名称] 并选择 **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. 选择 **[!UICONTROL 授权Marketo]**.

   >[!NOTE]
   >
   >确保从您的个人注销 [!DNL Gmail] 帐户并启用弹出窗口。

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. 选择您的关联帐户 [!DNL Google AdWords].

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. 选择 **[!UICONTROL 接受]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. 状态将显示为 **[!UICONTROL 成功]**. 选择 **[!UICONTROL 下一个]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. 将离线转化从Marketo上传到 [!DNL Google AdWords] **[!UICONTROL 每周]** 或 **[!UICONTROL 每日]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. 将属性转化为 **[!UICONTROL 首次点击]** 或 **[!UICONTROL 最后点击]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | 类型 | 条件 |
   |---|---|
   | [!UICONTROL 首次点击] | 离线转化将归因于 [!DNL AdWords] 过去90天内用户点击的广告 |
   | [!UICONTROL 最后点击] | 离线转化将归属于最后一个 [!DNL AdWords] 用户点击的 |

   >[!NOTE]
   >
   >在Marketo中使用一致的归因模型和 [!DNL AdWords] 提供最准确的数据。

1. 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[自动标记](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} 必须选中，此功能才能正常工作。 必须在内部完成停用 [!DNL AdWords].

太棒了！ 现在，请参阅下面的相关文章以了解如何映射 [!DNL AdWords] 您的收入模型中的离线转化。

>[!MORELIKETHIS]
>
>[设置 [!DNL Google AdWords] 收入模型中的转化](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target="_blank"}
