---
unique-page-id: 7516460
description: 在Salesforce中为Sales Insight提供多语言支持做准备 — Marketo文档 — 产品文档
title: 为Salesforce中的多语言支持准备Sales Insight
exl-id: b808fa91-accd-4e0c-8223-0717faccab10
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 1%

---

# 为Salesforce中的多语言支持准备Sales Insight {#prepare-sales-insight-for-multi-lingual-support-in-salesforce}

>[!NOTE]
>
>**需要管理员权限**

Marketo Sales Insight按语言存储。 因此，如果您希望它适用于多种语言，则必须分别输入每种语言的凭据。

>[!NOTE]
>
>Sales Insight当前支持：
>
>* 英语
>* 法语
>* 德语
>
>任何其他语言均默认使用英语。

## 为Marketo Sales Insight添加新语言 {#adding-a-new-language-for-marketo-sales-insight}

1. 登录Salesforce。 在右上角您的名称下方的下拉菜单中，单击 **设置**.

   ![](assets/image2015-7-6-16-3a5-3a6.png)

1. 下 **我的个人信息**，单击 **个人信息**.

   ![](assets/image2015-7-6-16-3a5-3a25.png)

1. 单击 **编辑**.

   ![](assets/image2015-7-6-16-3a5-3a38.png)

1. 选择语言并单击 **保存**.

   ![](assets/image2015-7-6-16-3a5-3a47.png)

1. 您的Salesforce界面现在使用选定的语言。 您可以单击 **+** 图标，以查看所有可用的选项卡。

   ![](assets/image2015-7-6-16-3a6-3a10.png)

1. 单击 **配置Marketo Sales Insight** （使用选定的语言）。

   ![](assets/image2015-7-6-16-3a7-3a15.png)

1. 转到Marketo。 找到您的 [Marketo Sales Insight **API配置** 详细信息](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-marketo-sales-insight).

   ![](assets/image2015-7-6-16-3a41-3a2.png)

1. 输入Marketo中的API详细信息，然后单击 **保存**.

   ![](assets/image2015-7-6-16-3a7-3a43.png)

## 将Salesforce改回英语 {#change-salesforce-back-to-english}

完成自定义Salesforce组织后，下面是如何将个人配置返回为英语的。

>[!NOTE]
>
>以下屏幕截图为法文，并附有英文说明。  您将看到相同的屏幕，其中包含使用您在上一步中选择的语言编写的文本。

1. 在您的名称下，单击 **设置**.

![](assets/image2015-7-6-16-3a5-3a6.png)

1. 单击 **个人信息** 下 **我的个人信息**.

   ![](assets/image2015-7-6-16-3a8-3a3.png)

1. 单击 **编辑**.

   ![](assets/image2015-7-6-16-3a8-3a19.png)

1. 选择 **英语** 从“语言”下拉列表中，单击 **保存**.

   ![](assets/image2015-7-6-16-3a8-3a31.png)

   现在你的Salesforce又用英语了！
