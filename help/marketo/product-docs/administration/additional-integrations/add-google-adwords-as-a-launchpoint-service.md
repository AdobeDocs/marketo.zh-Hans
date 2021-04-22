---
unique-page-id: 6095008
description: 将Google AdWords添加为LaunchPoint服务 — Marketo Docs — 产品文档
title: 将Google AdWords添加为LaunchPoint服务
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 将Google AdWords添加为LaunchPoint服务{#add-google-adwords-as-a-launchpoint-service}

将您的Google AdWords帐户链接到Marketo，以自动将线下转换数据从Marketo上传到Google AdWords。 然后，从AdWords UI中，您将能够在AdWords中[添加自定义列](https://support.google.com/adwords/answer/3073556)后轻松查看哪些点击产生了合格的潜在客户、机会和新客户（或您要跟踪的任何收入阶段）。 此信息不显示在Marketo UI中。

了解有关[Google的脱机转换导入功能的更多信息](https://support.google.com/adwords/answer/2998031?hl=en)。

>[!NOTE]
>
>**需要管理权限**

>[!NOTE]
>
>您还可以将[Google AdWords作为Launchpoint服务与管理器帐户](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)集成。

1. 转至&#x200B;**Admin**&#x200B;部分。

   ![](assets/login-admin.png)

1. 选择&#x200B;**LaunchPoint**。

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. 选择&#x200B;**新建**&#x200B;和&#x200B;**新建服务**。

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. 输入显示名称，然后选择&#x200B;**Google AdWords**。

   ![](assets/new-service-google.png)

1. 选择&#x200B;**授权Marketo**。

   >[!NOTE]
   >
   >确保注销您的个人Gmail帐户并启用弹出窗口。

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. 选择与Google AdWords关联的帐户。

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. 选择&#x200B;**接受**。

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. 状态将显示为&#x200B;**Success**。 选择&#x200B;**下一步**。

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. 将您的脱机转换从Marketo上传到Google AdWords **Weekly**&#x200B;或&#x200B;**Daily**。

   ![](assets/image2015-2-23-16-3a53-3a4.png)

1. 属性转换为&#x200B;**First Click**&#x200B;或&#x200B;**Last Click**。

   | 类型 | 定义 |
   |---|---|
   | 首次单击 | 脱机转换将归因于过去90天内用户点击的第一个AdWords广告 |
   | 上次单击 | 脱机转换将归因于用户点击的上一个AdWords广告 |

   >[!NOTE]
   >
   >在Marketo和AdWords中使用一致的归因模型可提供最准确的数据。

   ![](assets/image2015-2-23-16-3a57-3a49.png)

1. 单击&#x200B;**创建**。

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[必须选](https://support.google.com/adwords/answer/1752125?hl=en) 择“自动标记”才能使此功能正常工作。必须在AdWords内完成取消激活。

太棒了！ 现在，请参阅以下相关文章，了解如何在收入模型中映射AdWords离线转化率。

>[!MORELIKETHIS]
>
>[在收入模型中设置Google AdWords转换](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
