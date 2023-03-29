---
unique-page-id: 7504893
description: 使用经理帐户添加Google AdWords as a Launchpoint服务 — Marketo文档 — 产品文档
title: 使用Manager帐户将Google AdWords添加为Launchpoint服务
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

# 使用Manager帐户将Google AdWords添加为Launchpoint服务 {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

将您的Google AdWords帐户关联到Marketo，以自动将离线转化数据从Marketo上传到Google AdWords。 然后，从AdWords UI中，您将能够轻松地查看哪些点击在您之后产生了合格的潜在客户、商机和新客户（或您想要跟踪的任何收入阶段）  [添加自定义列](https://support.google.com/adwords/answer/3073556){target="_blank"} 在AdWords中。 此信息未显示在Marketo UI中。

如果您有多个Google Adwords帐户，则可以使用 [Google AdWords管理员帐户](https://www.google.com/adwords/manager-accounts/){target="_blank"} （以前称为My Client Center），以将其与Marketo集成。

详细了解 [Google离线转化导入功能](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>您还可以将 [作为Launchpoint服务的独立Google AdWords帐户](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. 转到 **管理员** 中。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. 选择 **LaunchPoint**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. 单击 **新建** 下拉框并选择 **新服务**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. 输入显示名称并选择 **Google AdWords**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. 选择 **授权Marketo**.

   >[!NOTE]
   >
   >确保注销您的个人Gmail帐户并启用弹出窗口。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. 选择与关联的帐户 **Google AdWords**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. 单击 **接受**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. 状态将显示为 **成功**. 选择 **下一个**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. 将离线转化从Marketo上传到Google AdWords **每周** 或 **每日**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. 属性转换到 **首次单击** 或 **上次点击**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | 类型 | 条件 |
   |---|---|
   | 首次单击 | 离线转化将归因于用户在过去90天内点击的第一个AdWords广告 |
   | 上次点击 | 离线转化将归因于人员点击的最后一个AdWords广告 |

   >[!NOTE]
   >
   >[自动标记](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} 必须选择此功能才能正常工作。 它必须在AdWords中激活。

1. 单击 **下一个**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. 取消选择您不希望更新的帐户。 单击&#x200B;**创建**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   现在，请参阅下面的相关文章，了解如何在收入模型中映射AdWords离线转化。

   >[!MORELIKETHIS]
   >
   >[使用经理帐户在收入模型中设置Google AdWords转化](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
