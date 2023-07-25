---
unique-page-id: 4718683
description: 批准阶段并将潜在客户分配给收入模型 — Marketo文档 — 产品文档
title: 审批阶段并将销售线索分配给收入模型
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 审批阶段并将销售线索分配给收入模型 {#approving-stages-and-assigning-leads-to-a-revenue-model}

获取您的 **收入模型** 添加现有潜在客户，为任何新潜在客户创建分配规则，从而启动并运行。

## 审批阶段 {#approving-stages}

让我们在添加任何潜在客户之前批准模型的各个阶段。

1. 转到 **分析** 区域。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 选择要批准其阶段的模型。

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. 下 **模型操作**，选择 **批准阶段**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. 您将收到一个警告消息；单击 **分配潜在客户**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

太棒了！ 让我们继续并分配这些潜在客户。

## 分配现有潜在客户 {#assigning-existing-leads}

[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 为Lead数据库中的模型的一个阶段确定Lead。

1. 一旦您 [已创建您的智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)，单击 **潜在客户** 选项卡。

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. 单击 **全选** 以选择潜在客户。

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. 打开 **潜在客户操作** 下拉菜单并选择 **特殊**. 单击 **更改收入阶段**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. 选择正确的 **模型** 和正确的 **暂存**. 单击 **立即运行**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. 重复上述步骤，直到将所有潜在客户都分配到模型的各个阶段。

太棒了！ 要指定如何将新潜在客户分配给阶段，请创建分配规则。

>[!NOTE]
>
>如果您的模型处于“已批准阶段”状态，则不会在商机的活动日志中看到任何“更改收入阶段”事件。 如果您的模型获得完全批准，如果将潜在客户移动到其当前所处的相同阶段，则将跳过此流程步骤。

## 新销售线索：创建分配规则  {#new-leads-create-assignment-rules}

1. 单击 **Marketo主页** 再次，然后选择 **分析**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 在树中单击模型，然后 **模型操作** 菜单，选择 **分配规则**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. 如果您的分配规则包含多个默认选项，请单击 **暂存**，进行选择，然后单击 **添加选项**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## 示例分配规则 {#example-assignment-rule}

创建“商机得分”规则，以将得分最低的新商机分配给适当的步骤。

1. 下 **如果**，选择 **商机得分**. 然后选择 **至少**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. 输入 **40** 在字段中，然后选择 **销售线索** 作为舞台。 单击 **保存** 完成。

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>要批准您的模型，请阅读我们的帮助页面，网址为 **[批准和取消批准收入模型](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
