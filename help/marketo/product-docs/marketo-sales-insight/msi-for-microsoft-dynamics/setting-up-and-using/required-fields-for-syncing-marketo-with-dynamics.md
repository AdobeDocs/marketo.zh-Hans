---
unique-page-id: 11375827
description: 将Marketo与Dynamics同步的必填字段 — Marketo文档 — 产品文档
title: 将Marketo与Dynamics同步的必填字段
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 1%

---

# 与[!DNL Dynamics]同步Marketo所需的字段 {#required-fields-for-syncing-marketo-with-dynamics}

这些字段&#x200B;*必须*&#x200B;与Marketo同步，以便[!UICONTROL Lead]和[!UICONTROL Contact]都能正常工作：[!DNL Sales Insight]

* 优先级
* 紧急
* 相对分数

如果缺少这些字段中的任何一个，您将在Marketo中看到一条错误消息，其中包含缺少的字段的名称。 要解决此问题，请签入您的实例以确保字段已为&#x200B;**[!UICONTROL Lead]**&#x200B;和&#x200B;**[!UICONTROL Contact]**&#x200B;同步。 如果不能，请添加它们。

以下是如何验证和添加同步字段。

1. 转到[!UICONTROL Admin]并单击&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击&#x200B;**[!UICONTROL Edit]**&#x200B;上的[!UICONTROL Field Sync Details]。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 在[!UICONTROL Lead]下，选中[!UICONTROL Priority]复选框。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 现在，向下滚动并选中[!UICONTROL Urgency]复选框……

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...和[!UICONTROL Relative Score]复选框。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 接下来，选中[!UICONTROL Priority]的[!UICONTROL Urgency]、[!UICONTROL Relative Score]和[!UICONTROL Contact]复选框。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>请确保至少等待10分钟，以便运行同步，然后再验证是否已修复此问题。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
