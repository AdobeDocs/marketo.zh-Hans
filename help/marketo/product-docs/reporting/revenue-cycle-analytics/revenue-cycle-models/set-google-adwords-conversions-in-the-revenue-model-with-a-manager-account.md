---
unique-page-id: 7504923
description: 使用经理帐户在收入模型中设置Google AdWords转化 — Marketo文档 — 产品文档
title: 使用经理帐户在收入模型中设置Google AdWords转化
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 使用经理帐户在收入模型中设置Google AdWords转化 {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

将您的Google AdWords帐户关联到Marketo，以自动将离线转化数据从Marketo上传到Google AdWords。 然后，在AdWords中[添加自定义列](https://support.google.com/adwords/answer/3073556)后，您可以从AdWords UI中轻松查看哪些点击导致合格的潜在客户、机会和新客户（或您希望跟踪的任何收入阶段）。

如果您有多个Google Adwords帐户，则可以使用[Google AdWords管理器帐户](https://www.google.com/adwords/manager-accounts/)（以前称为“我的客户端中心”）将它们与Marketo集成。

您可以将AdWords离线转化映射到收入模型的一个或多个阶段。 有两种方法可用：

* 暂存操作
* AdWords映射

>[!PREREQUISITES]
>
>[使用经理帐户将Google AdWords添加为Launchpoint服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## 使用暂存操作 {#use-stage-action}

在暂存操作下映射AdWords转换。

1. 选择要映射到AdWords转换的步骤。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**暂存操作**&#x200B;下拉列表下，选择&#x200B;**设置AdWords转换**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 设置&#x200B;**AdWords转换**。

   >[!NOTE]
   >
   >可以为每个子帐户选择不同的AdWords转换。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   提示：如果您没有任何AdWords转化，请单击&#x200B;**+新建转化**&#x200B;以创建一个。

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. 完成将所有AdWords转化映射到收入阶段后，返回摘要页面。 选择&#x200B;**模型操作**&#x200B;并选择&#x200B;**批准阶段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 专业提示：添加新转化 {#pro-tip-add-a-new-conversion}

专业提示！ 可以从Marketo创建新的AdWords离线转化。

>[!CAUTION]
>
>从Marketo创建的新转化启用了“优化”设置。 这意味着允许AdWords竞价策略优化您对这些转化的竞价。 您可以通过AdWords帐户更改此设置。

1. 在&#x200B;**暂存操作**&#x200B;下拉列表下，选择&#x200B;**设置AdWords转换**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 选择&#x200B;**新转换**。

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. 输入&#x200B;**转换名称**。 单击&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   太棒了！ 此新转化将显示在您的AdWords帐户中。

## 使用AdWords映射 {#use-adwords-mapping}

您可以使用AdWords映射将所有模型阶段与AdWords转换关联到一个位置。

1. 选择&#x200B;**编辑AdWords映射**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 为要跟踪的每个阶段选择所需的&#x200B;**AdWords帐户**&#x200B;和所需的&#x200B;**AdWords转换**。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. 映射阶段后，单击&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. 完成将所有AdWords转化映射到收入阶段后，返回摘要页面。 选择&#x200B;**模型操作**&#x200B;并选择&#x200B;**批准阶段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

要查看离线转化数据，您需要登录AdWords帐户。 我们建议您使用其[自定义列功能](https://support.google.com/adwords/answer/3073556)为您从Marketo导入的每个离线转化创建转化计数列。
