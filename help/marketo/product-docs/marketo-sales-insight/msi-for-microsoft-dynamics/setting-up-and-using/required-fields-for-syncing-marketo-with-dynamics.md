---
unique-page-id: 11375827
description: 将Marketo与Dynamics同步的必填字段 — Marketo文档 — 产品文档
title: 将Marketo与Dynamics同步的必填字段
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 将Marketo与Dynamics同步的必填字段 {#required-fields-for-syncing-marketo-with-dynamics}

这些字段 *必须* 与Marketo同步，以便潜在客户和联系人能够进行Sales Insight：

* 优先级
* 紧急
* 相对分数

如果缺少其中任何字段，您将在Marketo中看到一条错误消息，其中包含缺少的字段的名称。 要解决此问题，请签入您的实例以确保这两个字段都同步 **商机** 和 **联系人**. 如果不能，请添加它们。

以下是如何验证和添加同步字段。

1. 转到“管理员”并单击 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击 **编辑** 在字段同步详细信息上。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 在Lead下，选中Priority复选框。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 现在，向下滚动并选中紧急状态复选框……

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...和“相对分数”复选框。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 接下来，选中“优先级”、“紧急程度”和“联系人的相对分数”复选框。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 单击 **保存**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>请确保至少等待10分钟，以便运行同步，然后再验证是否已修复此问题。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
