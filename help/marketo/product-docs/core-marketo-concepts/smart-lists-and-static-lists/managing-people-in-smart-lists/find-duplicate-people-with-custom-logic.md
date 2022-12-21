---
unique-page-id: 2952636
description: 使用自定义逻辑查找重复人员 — Marketo文档 — 产品文档
title: 使用自定义逻辑查找重复人员
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 5%

---

# 使用自定义逻辑查找重复人员 {#find-duplicate-people-with-custom-logic}

Marketo有一个系统智能列表，可通过匹配重复的人员电子邮件地址来查找他们。 如果要使用其他字段查找重复项，请参阅以下操作方法。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 转到 **营销活动** 的上界。

![](assets/ma-2.png)

1. 选择智能列表，单击 **智能列表** 选项卡。

   ![](assets/two-4.png)

1. 查找并拖动 **复制字段** 过滤到画布上。

   ![](assets/three-4.png)

1. 从四个可用选项中选择一个：

   * 电子邮件地址
   * 全名
   * 姓氏
   * 更新日期：

   >[!NOTE]
   >
   >除“电子邮件地址”之外，所有字段均区分大小写。 因此，在“全名”字段中使用“john doe”将 _not_ 返回无名氏的结果。

   ![](assets/four-2.png)

   完成! 运行智能列表，以在之前选择的字段中查找具有相同值的人员。
