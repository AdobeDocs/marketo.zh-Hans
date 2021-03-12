---
unique-page-id: 2952636
description: 查找具有自定义逻辑的重复人员 — Marketo Docs — 产品文档
title: 使用自定义逻辑查找重复
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# 查找具有自定义逻辑{#find-duplicate-people-with-custom-logic}的重复

Marketo有一个系统智能列表，通过匹配重复的电子邮件地址来查找客户。 如果您想使用其他字段查找重复，请看以下方法。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 转至&#x200B;**营销活动**&#x200B;区域。

![](assets/ma-2.png)

1. 选择您的智能列表，单击&#x200B;**智能列表**&#x200B;选项卡。

   ![](assets/two-4.png)

1. 在画布上查找并拖动&#x200B;**重复字段**&#x200B;滤镜。

   ![](assets/three-4.png)

1. 从四个可用选项中选择一个：

   * 电子邮件地址
   * 全名
   * 姓氏
   * 更新日期

   >[!NOTE]
   >
   >除“电子邮件地址”之外，所有字段均区分大小写。 因此，在“全名”字段中使用“john doe”将&#x200B;_不_&#x200B;返回John Doe的结果。

   ![](assets/four-2.png)

   完成！ 运行智能列表，以在先前选择的字段中查找具有相同值的人。
