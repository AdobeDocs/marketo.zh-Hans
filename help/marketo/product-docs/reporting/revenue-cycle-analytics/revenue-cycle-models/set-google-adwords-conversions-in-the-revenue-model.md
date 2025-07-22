---
unique-page-id: 6095029
description: 在收入模型中设置 [!DNL Google AdWords] 转化 — Marketo文档 — 产品文档
title: 在收入模型中设置 [!DNL Google AdWords] 转化
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# 在收入模型中设置[!DNL Google AdWords]转化 {#set-google-adwords-conversions-in-the-revenue-model}

将您的[!DNL Google AdWords]帐户关联到Marketo以自动将离线转化数据从Marketo上传到[!DNL Google AdWords]。 然后，在[!DNL AdWords]中[添加自定义列](https://support.google.com/adwords/answer/3073556)后，您将能够从[!DNL AdWords] UI中轻松查看哪些点击导致合格的潜在客户、机会和新客户（或您希望跟踪的任何收入阶段）。

>[!NOTE]
>
>这是从Marketo到[!DNL Google AdWords]的推送集成。 转化数据将&#x200B;_仅_&#x200B;显示在您的[!DNL Google AdWords]门户中，_不显示在Marketo UI_&#x200B;中。

详细了解[Google的脱机转换导入功能](https://support.google.com/adwords/answer/2998031?hl=en)。 将[!DNL AdWords]离线转化映射到收入模型的一个或多个阶段。 有三种方法可执行映射：

* [!DNL AdWords]转换
* 暂存操作
* [!DNL AdWords]映射

如果您使用暂存操作，则可以从Marketo创建新的[!DNL AdWords]离线转换。

>[!PREREQUISITES]
>
>[添加 [!DNL Google AdWords] 作为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## 使用[!DNL AdWords]转换 {#use-adwords-conversion}

1. 转到&#x200B;**[!UICONTROL Analytics]**&#x200B;区域。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. 选择模型。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. 单击 **[!UICONTROL Edit Draft]**。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. 选择要映射到[!DNL AdWords]转换的收入阶段。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 选择要映射到Marketo阶段的&#x200B;**[!UICONTROL AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   太好了！ 您的[!DNL AdWords]转化数据将以您选择的节奏上传到[!DNL Google AdWords]。

## 使用暂存操作 {#use-stage-action}

您还可以映射[!UICONTROL AdWords Conversion]下的&#x200B;**[!UICONTROL Stage Actions]**。

1. 选择要映射到[!DNL AdWords]转换的步骤。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**[!UICONTROL Stage Actions]**&#x200B;下拉列表下，选择&#x200B;**[!UICONTROL Set AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 选择&#x200B;**[!UICONTROL AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **提示**：如果您没有任何[!DNL AdWords]转化，请单击&#x200B;**[!UICONTROL +New Conversion]**&#x200B;以创建一个。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. 完成将所有[!DNL AdWords]转化映射到收入阶段后，返回摘要页面。 选择&#x200B;**[!UICONTROL Model Actions]**&#x200B;并选择&#x200B;**[!UICONTROL Approve Stages]**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 专业提示：添加新转化 {#pro-tip-add-a-new-conversion}

专业提示！ 可从Marketo创建新的[!DNL AdWords]离线转换。

>[!CAUTION]
>
>从Marketo创建的新转化启用了“优化”设置。 这意味着允许[!DNL AdWords]竞价策略优化您的竞价以实现这些转化。 你可以从[!DNL AdWords]帐户更改此设置。

1. 在&#x200B;**[!UICONTROL Stage Actions]**&#x200B;下拉列表下，选择&#x200B;**[!UICONTROL Set AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 选择 **[!UICONTROL New Conversion]**。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 输入&#x200B;**[!UICONTROL Conversion Name]**。 单击 **[!UICONTROL Save]**。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   太棒了！ 此新转化将显示在您的[!DNL AdWords]帐户中。

## 使用[!DNL AdWords]映射 {#use-adwords-mapping}

您可以使用[!UICONTROL AdWords Conversion]映射在一个位置将所有模型阶段与[!DNL AdWords]相关联。

1. 选择 **[!UICONTROL Edit AdWords Mappings]**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 为要跟踪的每个阶段选择所需的&#x200B;**[!UICONTROL AdWords Conversion]**。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. 映射阶段后，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. 完成将所有[!DNL AdWords]转化映射到收入阶段后，返回摘要页面。 选择&#x200B;**[!UICONTROL Model Actions]**&#x200B;并选择&#x200B;**[!UICONTROL Approve Stages]**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

要查看离线转化数据，您需要登录[!DNL AdWords]帐户。 我们建议您使用其[自定义列功能](https://support.google.com/adwords/answer/3073556)为您从Marketo导入的每个离线转化创建转化计数列。
