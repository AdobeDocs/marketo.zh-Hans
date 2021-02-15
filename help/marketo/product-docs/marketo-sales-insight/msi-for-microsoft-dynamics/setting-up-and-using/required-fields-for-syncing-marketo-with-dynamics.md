---
unique-page-id: 11375827
description: 将Marketo与Dynamics同步的必填字段 — Marketo Docs — 产品文档
title: 将Marketo与Dynamics同步的必填字段
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# 将Marketo与Dynamics {#required-fields-for-syncing-marketo-with-dynamics}同步的必填字段

以下字段&#x200B;*必须*&#x200B;与Marketo同步，以使潜在客户和Contact for Sales Insight正常工作：

* 优先级
* 紧急
* 相对得分

如果缺少其中任何字段，您将在Marketo中看到一条错误消息，其中包含缺少字段的名称。 要解决此问题，请检查您的实例，确保字段已同步&#x200B;**Lead**&#x200B;和&#x200B;**Contact**。 否则，添加它们。

下面介绍如何验证和添加同步字段。

1. 转至“Admin”（管理员）并单击&#x200B;**Microsoft Dynamics**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“字段同步详细信息”上的&#x200B;**编辑**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 在潜在客户下，选中优先级复选框。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 现在，向下滚动并选中“紧急”复选框……

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...和“相对得分”复选框。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 接下来，选中“联系人的优先级”、“紧急性”和“相对分数”复选框。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>请确保至少等待10分钟以运行同步，然后再确认您已解决此问题。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
