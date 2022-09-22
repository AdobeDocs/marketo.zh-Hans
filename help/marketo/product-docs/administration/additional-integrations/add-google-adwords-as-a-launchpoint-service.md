---
unique-page-id: 6095008
description: 将Google AdWords添加为LaunchPoint服务 — Marketo文档 — 产品文档
title: 将Google AdWords添加为LaunchPoint服务
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
source-git-commit: 457b4aadac47b0a8614c3e6025d2e1ae287b5ecc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 将Google AdWords添加为LaunchPoint服务 {#add-google-adwords-as-a-launchpoint-service}

将您的Google AdWords帐户关联到Marketo，以自动将离线转化数据从Marketo上传到Google AdWords。 然后，从AdWords UI中，您将能够轻松地查看哪些点击在您之后产生了合格的潜在客户、商机和新客户（或您想要跟踪的任何收入阶段） [添加自定义列](https://support.google.com/adwords/answer/3073556)AdWords中的{target=&quot;_blank&quot;}。 此信息未显示在Marketo UI中。

详细了解 [Google离线转化导入功能](https://support.google.com/adwords/answer/2998031?hl=en){target=&quot;_blank&quot;}。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的客户成功经理。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>您还可以将 [Google AdWords as a Launchpoint服务（具有经理帐户）](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target=&quot;_blank&quot;}。

1. 转到 **管理员** 中。

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. 选择 **LaunchPoint**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. 选择 **新建** 和 **新服务**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. 输入显示名称并选择 **Google AdWords**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. 选择 **授权Marketo**.

   >[!NOTE]
   >
   >确保注销您的个人Gmail帐户并启用弹出窗口。

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. 选择与Google AdWords关联的帐户。

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. 选择 **接受**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. 状态将显示为 **成功**. 选择 **下一个**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. 将离线转化从Marketo上传到Google AdWords **每周** 或 **每日**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. 属性转换到 **首次单击** 或 **上次点击**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | 类型 | 条件 |
   |---|---|
   | 首次单击 | 离线转化将归因于用户在过去90天内点击的第一个AdWords广告 |
   | 上次点击 | 离线转化将归因于人员点击的最后一个AdWords广告 |

   >[!NOTE]
   >
   >在Marketo和AdWords中使用一致的归因模型可提供最准确的数据。

1. 单击 **创建**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[自动标记](https://support.google.com/adwords/answer/1752125?hl=en)必须选择{target=&quot;_blank&quot;}才能使此功能正常工作。 必须在AdWords内完成停用。

太棒了！ 现在，请参阅下面的相关文章，了解如何在收入模型中映射AdWords离线转化。

>[!MORELIKETHIS]
>
>[在收入模型中设置Google AdWords转化](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target=&quot;_blank&quot;}
