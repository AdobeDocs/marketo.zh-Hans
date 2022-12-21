---
unique-page-id: 7504923
description: 使用经理帐户在收入模型中设置Google AdWords转化 — Marketo文档 — 产品文档
title: 使用经理帐户在收入模型中设置Google AdWords转化
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 使用经理帐户在收入模型中设置Google AdWords转化 {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

将您的Google AdWords帐户关联到Marketo，以自动将离线转化数据从Marketo上传到Google AdWords。 然后，从AdWords UI中，您将能够轻松地查看哪些点击在您之后产生了合格的潜在客户、商机和新客户（或您想要跟踪的任何收入阶段） [添加自定义列](https://support.google.com/adwords/answer/3073556) 在AdWords中。

如果您有多个Google Adwords帐户，则可以使用 [Google AdWords管理员帐户](https://www.google.com/adwords/manager-accounts/) （以前称为My Client Center），以将其与Marketo集成。

您可以在收入模型中将AdWords离线转化映射到一个或多个阶段。 有两种方法：

* 暂存操作
* AdWords映射

>[!PREREQUISITES]
>
>[使用Manager帐户将Google AdWords添加为Launchpoint服务](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## 使用阶段操作 {#use-stage-action}

在“阶段操作”下映射AdWords转化。

1. 选择要映射到AdWords转化的步骤。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在 **暂存操作** 下拉框，选择 **设置AdWords转化**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 设置 **AdWords转化**.

   >[!NOTE]
   >
   >可以为每个子帐户选择不同的AdWords转换。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   提示：如果您没有任何AdWords转化，请通过单击 **+新建转化**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 单击 **保存**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. 完成将所有AdWords转化映射到收入阶段后，返回到摘要页面。 选择 **模型操作** 选择 **批准阶段**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 专业提示：添加新转化 {#pro-tip-add-a-new-conversion}

小费！ 可以从Marketo创建新的AdWords离线转化。

>[!CAUTION]
>
>从Marketo创建的新转化启用了“优化”设置。 这意味着允许AdWords竞价策略优化您对这些转化的竞价。 您可以从AdWords帐户中更改此设置。

1. 在 **暂存操作** 下拉框，选择 **设置AdWords转化**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 选择 **新转化**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. 输入 **转化名称**. 单击 **保存**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   太棒了！ 此新转化将显示在您的AdWords帐户中。

## 使用AdWords映射 {#use-adwords-mapping}

您可以使用AdWords映射将所有模型阶段与AdWords转化关联到一个位置。

1. 选择 **编辑AdWords映射**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 选择所需的 **AdWords帐户** 所需 **AdWords转化** 要跟踪的每个阶段。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. 映射阶段后，单击 **保存**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. 完成将所有AdWords转化映射到收入阶段后，返回到摘要页面。 选择 **模型操作** 选择 **批准阶段**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

要查看离线转化数据，您需要登录AdWords帐户。 我们建议您使用 [自定义列功能](https://support.google.com/adwords/answer/3073556) 要为从Marketo导入的每个离线转化创建转化计数列。
