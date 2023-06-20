---
description: Salesforce同步错误 — Marketo文档 — 产品文档
title: Salesforce同步错误
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
source-git-commit: 4d88547ecdc25a2a1e0de49fab1493bbefd6800b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Salesforce同步错误 {#salesforce-sync-errors}

查看同步过程中遇到的错误的摘要。 这包括因无法同步不兼容的数据而导致的错误。

>[!NOTE]
>
>**需要管理员权限**

## 查看同步错误 {#view-sync-errors}

1. 单击 **管理员**.

   ![](assets/salesforce-sync-errors-1.png)

1. 在集成下，单击 **Salesforce**，则 **同步错误** 选项卡。

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>列出的错误范围从当前时间到当前同步前五天。

| 字段 | 描述 |
|---|---|
| 失败日期 | 记录级别 _或_ 作业级别 |
| 失败的日期/时间 | 错误详细信息 |
| 错误类型 | SFDC返回消息 |

>[!TIP]
>
>单击记录级别记录会显示相关对象的Marketo和Salesforce ID。 在某些情况下，记录中的消息和工作级别错误是直接从Salesforce中获取的。 联机搜索可提供更多详细信息。

## 筛选器同步错误 {#filter-sync-errors}

1. 要筛选数据，请单击页面最右侧的筛选图标。

   ![](assets/salesforce-sync-errors-3.png)

1. 选择您的日期和时间范围，然后按错误类型筛选（作业级别或记录级别）。 单击 **应用** 完成时。

   ![](assets/salesforce-sync-errors-4.png)

**可选步骤**：要导出同步错误，请单击 **导出**. 数据将导出为CSV。

![](assets/salesforce-sync-errors-5.png)
