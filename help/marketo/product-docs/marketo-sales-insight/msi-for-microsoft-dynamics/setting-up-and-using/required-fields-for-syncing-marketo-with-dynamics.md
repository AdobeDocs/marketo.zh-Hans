---
unique-page-id: 11375827
description: 将Marketo与Dynamics同步的必填字段 — Marketo文档 — 产品文档
title: 将Marketo与Dynamics同步的必填字段
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# 将Marketo与Dynamics同步的必填字段 {#required-fields-for-syncing-marketo-with-dynamics}

这些字段 *必须* 与Marketo同步，以便潜在客户和联系人以便Sales Insight正常工作：

* 优先级
* 紧急
* 相对分数

如果这些字段中有任何字段缺失，您将在Marketo中看到一条错误消息，其中包含缺少字段的名称。 要修复此问题，请在实例中检查，以确保字段已同步，这两者均适用 **商机** 和 **联系人**. 如果没有，请添加它们。

以下是如何验证和添加同步字段。

1. 转到“管理员”并单击 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击 **编辑** 在字段同步详细信息中。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 在“潜在客户”下，选中“优先级”复选框。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 现在，向下滚动并选中“紧急”复选框……

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...和“相对得分”复选框。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 接下来，选中联系人的优先级、紧急性和相对分数复选框。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 单击 **保存**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>请确保至少等待10分钟以运行同步，然后再确认您已修复此问题。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星形和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
