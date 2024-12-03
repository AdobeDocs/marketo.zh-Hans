---
unique-page-id: 6095008
description: 添加 [!DNL Google AdWords] 作为 [!DNL LaunchPoint] 服务 — Marketo文档 — 产品文档
title: 将 [!DNL Google AdWords] 添加为 [!DNL LaunchPoint] 服务
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---

# 将[!DNL Google AdWords]添加为[!DNL LaunchPoint]服务 {#add-google-adwords-as-a-launchpoint-service}

将您的[!DNL Google AdWords]帐户关联到Marketo以自动将离线转化数据从Marketo上传到[!DNL Google AdWords]。 然后，在[!DNL AdWords]中[添加自定义列](https://support.google.com/adwords/answer/3073556){target="_blank"}后，您将能够从[!DNL AdWords] UI中轻松查看哪些点击导致合格的潜在客户、机会和新客户（或您希望跟踪的任何收入阶段）。 此信息不显示在Marketo UI中。

详细了解[Google的脱机转换导入功能](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}。

>[!AVAILABILITY]
>
>并非所有Marketo Engage用户都已购买此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>您还可以将[[!DNL Google AdWords] 作为 [!DNL Launchpoint] 服务与经理帐户](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}集成。

1. 转到&#x200B;**[!UICONTROL 管理员]**&#x200B;区域。

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. 选择&#x200B;**[!UICONTROL 启动点]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. 选择&#x200B;**[!UICONTROL 新建]**&#x200B;和&#x200B;**[!UICONTROL 新服务]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. 输入[!UICONTROL 显示名称]并选择&#x200B;**[!UICONTROL Google AdWords]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. 选择&#x200B;**[!UICONTROL 授权Marketo]**。

   >[!NOTE]
   >
   >确保注销个人[!DNL Gmail]帐户并启用弹出窗口。

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. 选择与[!DNL Google AdWords]关联的帐户。

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. 选择&#x200B;**[!UICONTROL 接受]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. 状态将显示为&#x200B;**[!UICONTROL 成功]**。 选择&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. 将离线转化从Marketo上载到[!DNL Google AdWords] **[!UICONTROL 每周]**&#x200B;或&#x200B;**[!UICONTROL 每日]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. 属性转换为&#x200B;**[!UICONTROL 首次点击]**&#x200B;或&#x200B;**[!UICONTROL 上次点击]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | 类型 | 定义 |
   |---|---|
   | [!UICONTROL 首次点击] | 离线转化将归因于某人在过去90天内点击的第一个[!DNL AdWords]广告 |
   | [!UICONTROL 最后点击] | 离线转化将归因于某人点击的最后一个[!DNL AdWords]广告 |

   >[!NOTE]
   >
   >在Marketo和[!DNL AdWords]中使用一致的归因模型可提供最准确的数据。

1. 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >必须选择[自动标记](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"}才能使此功能正常工作。 必须在[!DNL AdWords]内完成停用。

太棒了！ 现在，请参阅下面的相关文章，了解如何在收入模型中映射[!DNL AdWords]离线转化。

>[!MORELIKETHIS]
>
>在收入模型中设置[转化 [!DNL Google AdWords] ](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target="_blank"}
