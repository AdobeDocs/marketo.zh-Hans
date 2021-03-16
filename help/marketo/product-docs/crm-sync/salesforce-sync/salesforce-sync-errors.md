---
description: Salesforce同步错误 — Marketo文档 — 产品文档
title: Salesforce同步错误
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Salesforce同步错误{#salesforce-sync-errors}

视图同步过程中遇到的错误的摘要。 这包括由于无法同步不兼容的数据而导致的错误。

>[!NOTE]
>
>**需要管理权限**

## 视图同步错误{#view-sync-errors}

1. 单击&#x200B;**管理员**。

   ![](assets/salesforce-sync-errors-1.png)

1. 在“集成”下，单击&#x200B;**Salesforce**，然后单击&#x200B;**同步错误**&#x200B;选项卡。

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>列出的错误范围从当前时间到当前同步前五天。

| 字段 | 说明 |
|---|---|
| 失败时间 | 记录级别&#x200B;_或_&#x200B;作业级别 |
| 失败的日期/时间 | 错误详细信息 |
| 错误类型 | SFDC返回消息 |

>[!TIP]
>
>单击记录级别记录可显示相关对象的Marketo和Salesforce ID。 在某些情况下，记录和作业级别错误上的消息直接来自Salesforce。 在线搜索可能会提供更多详细信息。

## 筛选器同步错误{#filter-sync-errors}

1. 要筛选数据，请单击页面最右侧的筛选图标。

   ![](assets/salesforce-sync-errors-3.png)

1. 选择日期和时间范围，然后按错误类型（任务层或记录层）进行筛选。 完成后，单击&#x200B;**应用**。

   ![](assets/salesforce-sync-errors-4.png)

**可选步骤**:要导出同步错误，请单击“ **导出**”。数据将导出为CSV。

![](assets/salesforce-sync-errors-5.png)
