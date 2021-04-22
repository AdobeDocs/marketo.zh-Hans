---
unique-page-id: 10092977
description: Microsoft Dynamics Sync过滤器 — 资格 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步筛选器 — 限定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Microsoft Dynamics同步筛选器：确定{#microsoft-dynamics-sync-filter-qualify}

在Microsoft Dynamics中将潜在客户转换为联系人时，请确保使用此默认的“确定”流程。 然后，将其同步到Marketo。

## 转换进程{#the-conversion-process}

以下是过滤器在转化过程中的工作方式。

| 如果潜在客户同步过滤器为： | 联系人同步过滤器为： | 这是Marketo |
|---|---|---|
| False | False | 未在Marketo中同步任何内容 |
| True | True | 联系人已同步到Marketo |
| False | True | 在Marketo中创建了新的联系记录 |
| True | False | MS Dynamics更新Marketo中的潜在客户信息，但联系记录未同步 |

>[!CAUTION]
>
>我们仅支持开箱即用的资格转换流程。
