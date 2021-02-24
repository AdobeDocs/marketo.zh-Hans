---
unique-page-id: 6095029
description: 在收入模型 — Marketo Docs — 产品文档中设置Google AdWords转换
title: 在收入模型中设置Google AdWords转换
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# 在收入模型{#set-google-adwords-conversions-in-the-revenue-model}中设置Google AdWords转换

将您的Google AdWords帐户关联到Marketo，以自动将线下转换数据从Market上传到Google AdWords。 然后，从AdWords UI中，您将能够在AdWords中[添加自定义列](https://support.google.com/adwords/answer/3073556)后轻松查看哪些点击产生了合格的潜在客户、机会和新客户（或您要跟踪的任何收入阶段）。

>[!NOTE]
>
>这是从Marketo到Google AdWords的推动集成。 转换数据将仅&#x200B;_在Google AdWords门户中显示_，而不在Marketo UI _中显示_。

了解有关[Google的脱机转换导入功能的更多信息](https://support.google.com/adwords/answer/2998031?hl=en)。 将AdWords脱机转换映射到收入模型中的一个或多个阶段。 有三种方法可执行映射：

* AdWords转换
* 舞台操作
* AdWords映射

如果您使用Stage Action，则可以从Marketo创建新的AdWord脱机转换。

>[!PREREQUISITES]
>
>[将Google AdWords添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## 使用AdWord转换{#use-adwords-conversion}

1. 转至&#x200B;**Analytics**&#x200B;区域。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. 选取模型。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. 单击&#x200B;**编辑草稿**。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. 选择要映射到AdWords转换的收入阶段。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 选择要映射到Marketo舞台的&#x200B;**AdWords Conversion**。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   不错！ 您的AdWords转换数据将在您选择的节奏下上传到您的Google AdWords。

## 使用Stage操作{#use-stage-action}

您还可以在“阶段操作”下映射AdWords转换。

1. 选择要映射到AdWord转换的步骤。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**阶段操作**&#x200B;下拉列表中，选择&#x200B;**设置AdWord转换**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 选择&#x200B;**AdWords Conversion**。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **提示**:如果您没有任何AdWords转换，请单击+新建转换 **来创建一个**。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

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

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 输入&#x200B;**转换名称**。 单击&#x200B;**保存**。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   太棒了！ 此新转换将显示在您的AdWords帐户中。

## 使用AdWords映射{#use-adwords-mapping}

您可以使用AdWords映射将所有模型阶段与AdWords转换关联到一个位置。

1. 选择&#x200B;**编辑AdWords映射**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 为要跟踪的每个阶段选择所需的&#x200B;**AdWords Conversion**。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. 映射阶段后，单击&#x200B;**保存**。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. 完成所有AdWords转换到收入阶段的映射后，返回摘要页。 选择&#x200B;**模型操作**&#x200B;并选择&#x200B;**批准阶段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

要视图脱机转换数据，您需要登录AdWords帐户。 我们建议您使用其[自定义列功能](https://support.google.com/adwords/answer/3073556)为从Marketo导入的每个脱机转换创建转换计数列。
