---
unique-page-id: 1146897
description: 删除智能列表或列表中的人员 — Marketo文档 — 产品文档
title: 删除智能列表或列表中的人员
exl-id: 192e79e6-d816-44e3-84c4-212cd73eb3ce
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 删除智能列表或列表中的人员 {#delete-people-in-a-smart-list-or-list}

您可以快速轻松地删除列表或智能列表中的部分/所有人员。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 转到 **营销活动**.

   ![](assets/ma-1.png)

1. 选择包含要删除的所有人员的列表/智能列表，然后转到 **人员** 选项卡。

   ![](assets/two-1.png)

   >[!CAUTION]
   >
   >删除人员时，您不仅要从列表中删除他们，还会从数据库中完全删除他们。

1. 单击 **全选**. 您也可以使用Ctrl/Cmd并单击来手动选取一些记录。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >如果结果跨多个页面，请单击 **全选** 将选择所有页面中的所有人员。

1. 要从Marketo中完全删除用户，请单击 **删除人员**.

   ![](assets/four-1.png)

1. 设置 **从CRM中删除** 到 **true** 如果您还想从CRM中删除记录。

   ![](assets/five.png)

   >[!CAUTION]
   >
   >从Marketo和您的CRM中删除意味着您将永远无法在任一系统中恢复。 人民和他们的历史将永远消失。 如果以后再添加它们，它们将被视为全新的记录。

   >[!NOTE]
   >
   >如果您的Marketo未与CRM绑定，则该选项将灰显，就像屏幕快照中一样。

1. 单击 **立即运行**.

   ![](assets/image2014-9-24-13-3a0-3a3.png)

1. 如果您删除超过50人，您将看到此内容。 键入要删除的人员数量，检查 **无法撤消** 框，然后单击 **删除**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >要查看批量删除的结果，请单击 **查看结果** 在屏幕右上角的“单流量操作”弹出框中。 删除时间可能会大不相同，具体取决于多个因素。

   这是一个绝佳的功能，使用它时要格外小心！
