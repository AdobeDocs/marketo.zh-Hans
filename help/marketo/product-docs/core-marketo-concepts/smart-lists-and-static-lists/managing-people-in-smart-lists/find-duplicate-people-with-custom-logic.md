---
unique-page-id: 2952636
description: 使用自定义逻辑查找重复的人员 — Marketo文档 — 产品文档
title: 使用自定义逻辑查找重复人员
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '124'
ht-degree: 19%

---

# 使用自定义逻辑查找重复人员 {#find-duplicate-people-with-custom-logic}

Marketo Engage具有系统智能列表，可通过匹配重复人员的电子邮件地址来查找重复人员。 如果要使用其他字段查找重复项，请按照以下步骤操作。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. 进入 **[!UICONTROL Marketing Activities]** 区域。

![](assets/ma-2.png)

1. 选择您的智能列表，单击&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡。

   ![](assets/two-4.png)

1. 找到并将 **[!UICONTROL Duplicate Fields]** 过滤器拖到画布上。

   ![](assets/three-4.png)

1. 从四个可用选项中选择一个：

   * [!UICONTROL Email Address]
   * [!UICONTROL Full Name]
   * [!UICONTROL Last Name]
   * [!UICONTROL Updated At]

   >[!NOTE]
   >
   >除电子邮件地址外，所有字段均区分大小写。 因此，在“全名”字段中使用“john doe”将&#x200B;_不会_&#x200B;返回John Doe的结果。

   ![](assets/four-2.png)

   完成！ 运行智能列表以查找具有先前所选字段中的相同值的人员。
