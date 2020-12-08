---
unique-page-id: 11375827
description: 将Marketo与Dynamics同步的必填字段- Marketo Docs —— 产品文档
title: 将Marketo与Dynamics同步的必填字段
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 将Marketo与Dynamics同步的必填字段 {#required-fields-for-syncing-marketo-with-dynamics}

要使Lead *和Contact* for Sales Insight正常工作，这些字段必须与Marketo同步：

* 优先级
* 紧急
* 相对得分

如果这些字段中有任何一个缺失，您将在Marketo中看到一条错误消息，其中包含缺失字段的名称。 要解决此问题，请检查您的实例，以确保潜在客户和联系人的字 **段都** 已同 **步**。 否则，添加它们。

下面介绍如何验证和添加同步字段。

1. 转至“Admin”（管理）并单击“Microsoft Dynamics”(Microsoft Dynamics)。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“Edit on Field Sync Details”（在字段同步详细信息上编辑）。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 在潜在客户下，选中优先级复选框。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 现在，向下滚动并选中“紧急”复选框……

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...和“相对得分”复选框。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 然后，选中“联系人的优先级”、“紧急性”和“相对得分”复选框。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 单击“保存”。

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>请务必等待至少10分钟以运行同步，然后确认您已修复问题。

>[!NOTE]
>
>**相关文章**
>
>[为潜在客户／联系人记录设置星星和火焰](http://docs.marketo.com/x/BICMAg)

