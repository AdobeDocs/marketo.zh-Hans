---
unique-page-id: 7504923
description: 在收入模型中设置Google AdWords转换，其中包含经理帐户 — 营销文档 — 产品文档
title: 在收入模型中使用Manager帐户设置Google AdWords转换
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# 在收入模型中设置Google AdWords转换，其Manager帐户{#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

将您的Google AdWords帐户关联到Marketo，以自动将线下转换数据从Market上传到Google AdWords。 然后，从AdWords UI中，您将能够在AdWords中[添加自定义列](https://support.google.com/adwords/answer/3073556)后轻松查看哪些点击产生了合格的潜在客户、机会和新客户（或您要跟踪的任何收入阶段）。

如果您有多个Google Adwords帐户，则可以使用[Google AdWords管理器帐户](https://www.google.com/adwords/manager-accounts/)（以前称为“我的客户中心”）将其与Marketo集成。

您可以将AdWords脱机转换映射到收入模型中的一个或多个阶段。 有两种方式：

* 舞台操作
* AdWords映射

>[!PREREQUISITES]
>
>[通过Manager帐户将Google AdWords添加为Launchpoint服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## 使用Stage操作{#use-stage-action}

在“阶段操作”下映射AdWords转换。

1. 选择要映射到AdWord转换的步骤。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**阶段操作**&#x200B;下拉列表中，选择&#x200B;**设置AdWord转换**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 设置&#x200B;**AdWords Conversion**。

   >[!NOTE]
   >
   >可以为每个子帐户选择不同的AdWord转换。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   提示：如果您没有任何AdWords转换，请单击&#x200B;**+新转换**&#x200B;创建一个。

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. 完成所有AdWords转换到收入阶段的映射后，返回摘要页。 选择&#x200B;**模型操作**&#x200B;并选择&#x200B;**批准阶段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 专业提示：添加新转换{#pro-tip-add-a-new-conversion}

专业提示！ 可从Marketo创建新的AdWords脱机转换。

>[!CAUTION]
>
>从Market创建的新转换，以启用“优化”设置。 这意味着允许AdWords竞价策略优化您对这些转换的竞价。 您可以从AdWords帐户更改此设置。

1. 在&#x200B;**阶段操作**&#x200B;下拉列表中，选择&#x200B;**设置AdWord转换**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 选择&#x200B;**新建转换**。

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. 输入&#x200B;**转换名称**。 单击&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   太棒了！ 此新转换将显示在您的AdWords帐户中。

## 使用AdWords映射{#use-adwords-mapping}

您可以使用AdWords映射将所有模型阶段与AdWords转换关联到一个位置。

1. 选择&#x200B;**编辑AdWords映射**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 为要跟踪的每个阶段选择所需的&#x200B;**AdWords帐户**&#x200B;和所需的&#x200B;**AdWords转换**。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. 映射阶段后，单击&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. 完成所有AdWords转换到收入阶段的映射后，返回摘要页。 选择&#x200B;**模型操作**&#x200B;并选择&#x200B;**批准阶段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

要视图脱机转换数据，您需要登录AdWords帐户。 我们建议您使用其[自定义列功能](https://support.google.com/adwords/answer/3073556)为从Marketo导入的每个脱机转换创建转换计数列。
