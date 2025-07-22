---
unique-page-id: 4718683
description: 批准阶段并将潜在客户分配给收入模型 — Marketo文档 — 产品文档
title: 审批阶段并将销售线索分配给收入模型
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# 审批阶段并将销售线索分配给收入模型 {#approving-stages-and-assigning-leads-to-a-revenue-model}

通过添加现有潜在客户、为任何新潜在客户创建分配规则，启动并运行您的&#x200B;**收入模型**。

## 审批阶段 {#approving-stages}

让我们在添加任何潜在客户之前批准模型的各个阶段。

1. 转到&#x200B;**[!UICONTROL Analytics]**&#x200B;区域。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 选择要批准其阶段的模型。

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. 在&#x200B;**[!UICONTROL Model Actions]**&#x200B;下，选择&#x200B;**[!UICONTROL Approve Stages]**。

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. 您将收到一个警报；单击&#x200B;**[!UICONTROL Assign Leads]**。

   ![](assets/image2015-4-28-17-3a5-3a39.png)

太棒了！ 让我们继续并分配这些潜在客户。

## 分配现有潜在客户 {#assigning-existing-leads}

[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)以识别潜在客户数据库中模型某一阶段的潜在客户。

1. [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)后，单击&#x200B;**[!UICONTROL Leads]**&#x200B;选项卡。

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. 单击&#x200B;**[!UICONTROL Select All]**&#x200B;以选择潜在客户。

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. 打开&#x200B;**[!UICONTROL Lead Actions]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL Special]**。 单击 **[!UICONTROL Change Revenue Stage...]**。

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. 选择正确的&#x200B;**[!UICONTROL Model]**&#x200B;和正确的&#x200B;**[!UICONTROL Stage]**。 单击 **[!UICONTROL Run Now]**。

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. 重复上述步骤，直到所有潜在客户都分配到模型的各个阶段。

太棒了！ 要指定如何将新潜在客户分配给阶段，请创建分配规则。

>[!NOTE]
>
>如果您的模型处于“已批准阶段”状态，则不会在商机的活动日志中看到任何更改收入阶段事件。 如果您的模型获得完全批准，并且您将商机移动到其当前所处的相同阶段，则将跳过此流程步骤。

## 新建销售线索：创建分配规则  {#new-leads-create-assignment-rules}

1. 再次单击&#x200B;**Marketo主页**，然后选择&#x200B;**[!UICONTROL Analytics]**。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 单击树中的模型，然后单击&#x200B;**[!UICONTROL Model Actions]**&#x200B;菜单，选择&#x200B;**[!UICONTROL Assignment Rules]**。

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. 如果分配规则包含多个默认选择，请单击&#x200B;**[!UICONTROL Stage]**，进行选择，然后单击&#x200B;**[!UICONTROL Add Choice]**。

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## 示例分配规则 {#example-assignment-rule}

创建[!UICONTROL Lead Score]规则以将得分最低的新潜在客户分配给适当的步骤。

1. 在&#x200B;**[!UICONTROL If]**&#x200B;下，选择&#x200B;**[!UICONTROL Lead Score]**。 然后选择&#x200B;**[!UICONTROL at least]**。

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. 在字段中输入&#x200B;**40**&#x200B;并选择&#x200B;**[!UICONTROL Sales Lead]**&#x200B;作为[!UICONTROL Stage]。 单击&#x200B;**[!UICONTROL Save]**&#x200B;以完成。

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>要批准您的模型，请阅读我们的帮助页面：**[批准和取消批准收入模型](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**。
