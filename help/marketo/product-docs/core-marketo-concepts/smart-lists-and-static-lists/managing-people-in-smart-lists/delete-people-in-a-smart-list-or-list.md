---
unique-page-id: 1146897
description: 删除智能列表或列表中的人员 — Marketo文档 — 产品文档
title: 删除智能列表或列表中的人员
exl-id: 192e79e6-d816-44e3-84c4-212cd73eb3ce
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 删除智能列表或列表中的人员 {#delete-people-in-a-smart-list-or-list}

您可以快速、轻松地删除列表或智能列表中的某些/所有人员。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 转到 **营销活动**.

   ![](assets/ma-1.png)

1. 选择包含所有要删除的人员的列表/智能列表，然后转到 **人员** 选项卡。

   ![](assets/two-1.png)

   >[!CAUTION]
   >
   >删除人员时，您不仅会将其从列表中删除，还会从数据库中完全删除。

1. 单击 **全选**. 您还可以使用Ctrl/Cmd并单击来手动选取一些记录。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >如果结果跨越多个页面，请单击 **全选** 将选择所有页面中的所有人员。

1. 要从Marketo中完全删除人员，请单击 **删除人员**.

   ![](assets/four-1.png)

1. 已设置 **从CRM中删除** to **true** 如果您还要从CRM中删除记录，请执行以下操作：

   ![](assets/five.png)

   >[!CAUTION]
   >
   >从Marketo和您的CRM中删除意味着您将永远无法在任一系统中恢复。 人民和他们的历史将永远消失。 如果稍后再将它们添加回来，它们将被视为全新记录。

   >[!NOTE]
   >
   >如果您的Marketo未绑定到CRM，则选项将像屏幕截图中一样灰显。

1. 单击 **立即运行**.

   ![](assets/image2014-9-24-13-3a0-3a3.png)

1. 如果您删除的人员超过50人，则会看到此消息。 键入要删除的人数，并检查 **无法撤消** 框，然后单击 **删除**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >要查看成批删除的结果，请单击 **查看结果** 在屏幕右上角的“单流动操作”弹出框中。 删除时间可能会因多种因素而有很大差异。

   这是个很棒的功能，使用时要小心！
