---
unique-page-id: 7504893
description: 通过Manager帐户将Google AdWords添加为Launchpoint服务 — Marketo Docs — 产品文档
title: 通过Manager帐户将Google AdWords添加为Launchpoint服务
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 将Google AdWords添加为Launchpoint服务，其Manager帐户{#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

将您的Google AdWords帐户链接到Marketo，以自动将线下转换数据从Marketo上传到Google AdWords。 然后，从AdWords UI中，您将能够在AdWords中[添加自定义列](https://support.google.com/adwords/answer/3073556)后轻松查看哪些点击产生了合格的潜在客户、机会和新客户（或您要跟踪的任何收入阶段）。 此信息不显示在Marketo UI中。

如果您有多个Google Adwords帐户，则可以使用[Google AdWords管理器帐户](https://www.google.com/adwords/manager-accounts/)（以前称为My Client Center）将它们与Marketo集成。

了解有关[Google的脱机转换导入功能的更多信息](https://support.google.com/adwords/answer/2998031?hl=en)。

>[!NOTE]
>
>**需要管理权限**

>[!NOTE]
>
>您还可以将[独立Google AdWords帐户集成为Launchpoint服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)。

1. 转至&#x200B;**Admin**&#x200B;部分。

   ![](assets/login-admin-1.png)

1. 选择&#x200B;**LaunchPoint**。

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. 选择&#x200B;**新建**&#x200B;和&#x200B;**新建服务**。

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. 输入显示名称，然后选择&#x200B;**Google AdWords**。

   ![](assets/new-service-google-1.png)

1. 选择&#x200B;**授权Marketo**。

   >[!NOTE]
   >
   >确保注销您的个人Gmail帐户并启用弹出窗口。

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. 选择与&#x200B;**Google AdWords**&#x200B;关联的帐户。

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. 选择&#x200B;**接受**。

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. 状态将显示为&#x200B;**Success**。 选择&#x200B;**下一步**。

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. 将您的脱机转换从Marketo上传到Google AdWords **Weekly**&#x200B;或&#x200B;**Daily**。

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. 属性转换为&#x200B;**First Click**&#x200B;或&#x200B;**Last Click**。

   | 类型 | 定义 |
   |---|---|
   | 首次单击 | 脱机转换将归因于过去90天内用户点击的第一个AdWords广告 |
   | 上次单击 | 脱机转换将归因于用户点击的上一个AdWords广告 |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >[必须选](https://support.google.com/adwords/answer/1752125?hl=en) 择“自动标记”才能使此功能正常工作。必须在AdWords中激活。

1. 单击&#x200B;**下一步**。

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. 取消选择您不希望更新的帐户。 单击&#x200B;**创建**。

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   现在，请参阅以下相关文章，了解如何在收入模型中映射AdWords脱机转换。

   >[!MORELIKETHIS]
   >
   >[在收入模型中使用Manager帐户设置Google AdWords转换](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)
