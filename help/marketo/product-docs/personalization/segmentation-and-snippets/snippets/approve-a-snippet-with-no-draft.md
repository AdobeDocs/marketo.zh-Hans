---
unique-page-id: 10095644
description: 批准非草稿 — Marketo文档 — 产品文档的代码片段
title: 批准非草稿代码片段
exl-id: a06aa77a-68f1-41a4-b2bd-bf1882b81578
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 批准非草稿代码片段 {#approve-a-snippet-with-no-draft}

## 批准代码片段 {#approve-the-snippet}

每次批准代码片段时，都会触发“无草稿”。 这包括由其他工作区中的资产共享或引用的代码片段。

1. 转到 **Design Studio**.

   ![](assets/go-to-design-studio.png)

1. 选择一个代码片段，然后在 **代码片段操作** 下拉菜单，选择 **批准**.

   ![](assets/approve-snippet.png)

1. 在“批准代码片段”对话框中选择一个选项，然后单击 **批准**:

   * **全部更新**:此选项不会使用代码片段创建已批准资产的草稿。 所有资产都会获取更新并维护其以前的状态。 屏幕右上方会显示进度模块；它可以随时关闭。 要恢复该代码片段，请右键单击代码片段名称并选择显示批准状态。
   * **创建草稿**:此选项将使用代码片段创建已批准资产的草稿。 如果需要先审核代码片段更改，请选择此选项。 必须手动批准所有草稿。

   ![](assets/snippet-dialog-box.png)

   >[!NOTE]
   >
   >对于尚未使用的新代码片段，不会显示“批准草稿”屏幕。 在一个或多个资产中使用代码片段时，会显示该代码片段。

>[!CAUTION]
>
>此功能旨在通过代码片段批准工作流程节省时间。 但是，有一些限制需要注意。 请参阅 [本文档](https://nation.marketo.com/docs/DOC-4415) 以了解详细信息。 该文档还包含错误处理和故障诊断信息。

>[!MORELIKETHIS]
>
>[为片段启用非草稿](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md)
