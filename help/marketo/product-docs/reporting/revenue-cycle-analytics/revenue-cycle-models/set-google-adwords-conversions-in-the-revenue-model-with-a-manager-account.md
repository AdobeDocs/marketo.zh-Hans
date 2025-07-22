---
unique-page-id: 7504923
description: 使用经理帐户在收入模型中设置 [!DNL Google AdWords] 转化 — Marketo文档 — 产品文档
title: 使用经理帐户在收入模型中设置 [!DNL Google AdWords] 转化
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# 使用经理帐户在收入模型中设置[!DNL Google AdWords]转化 {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

将您的[!DNL Google AdWords]帐户关联到Marketo以自动将离线转化数据从Marketo上传到[!DNL Google AdWords]。 然后，在[!DNL AdWords]中[添加自定义列](https://support.google.com/adwords/answer/3073556)后，您将能够从[!DNL AdWords] UI中轻松查看哪些点击导致合格的潜在客户、机会和新客户（或您希望跟踪的任何收入阶段）。

如果您有多个[!DNL Google Adwords]帐户，则可以使用[[!DNL Google AdWords] 经理帐户](https://www.google.com/adwords/manager-accounts/)（以前称为“我的客户端中心”）将它们与Marketo集成。

您可以将[!DNL AdWords]离线转化映射到收入模型的一个或多个阶段。 有两种方法可用：

* 暂存操作
* [!DNL AdWords]映射

>[!PREREQUISITES]
>
>[添加 [!DNL Google AdWords] 作为具有经理帐户的Launchpoint服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## 使用暂存操作 {#use-stage-action}

在暂存操作下映射[!DNL AdWords]转化。

1. 选择要映射到[!DNL AdWords]转换的步骤。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**[!UICONTROL Stage Actions]**&#x200B;下拉列表下，选择&#x200B;**[!UICONTROL Set AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 设置&#x200B;**[!DNL AdWords]转换**。

   >[!NOTE]
   >
   >可以为每个子帐户选择不同的[!DNL AdWords]转换。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   提示：如果您没有任何[!DNL AdWords]转化，请单击&#x200B;**[!UICONTROL +New Conversion]**&#x200B;以创建一个。

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. 输入&#x200B;**转换名称**。 单击 **[!UICONTROL Save]**。

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   太棒了！ 此新转化将显示在您的[!DNL AdWords]帐户中。

## 使用[!DNL AdWords]映射 {#use-adwords-mapping}

您可以使用[!DNL AdWords]映射在一个位置将所有模型阶段与[!DNL AdWords]转化关联。

1. 选择 **[!UICONTROL Edit AdWords Mappings]**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 为要跟踪的每个阶段选择所需的&#x200B;**[!DNL AdWords]帐户**&#x200B;和所需的&#x200B;**[!DNL AdWords]转化**。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. 映射阶段后，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. 完成将所有[!DNL AdWords]转化映射到收入阶段后，返回摘要页面。 选择&#x200B;**[!UICONTROL Model Actions]**&#x200B;并选择&#x200B;**[!UICONTROL Approve Stages]**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

要查看离线转化数据，您需要登录[!DNL AdWords]帐户。 我们建议您使用其[自定义列功能](https://support.google.com/adwords/answer/3073556)为您从Marketo导入的每个离线转化创建转化计数列。
