---
unique-page-id: 10092977
description: Microsoft Dynamics Sync过滤器——资格- Marketo Docs —— 产品文档
title: Microsoft Dynamics同步筛选器——限定
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Microsoft Dynamics同步筛选器：确定{#microsoft-dynamics-sync-filter-qualify}

在Microsoft Dynamics中，如果要将潜在客户转换为联系人，请务必使用此默认的Qualify流程。 然后，将其同步到Marketo。

## 转换进程{#the-conversion-process}

下面介绍过滤器在转化过程中的工作方式。

| 如果潜在客户同步筛选器为： | 联系人同步过滤器为： | 这是Marketo的结果 |
|---|---|---|
| False | False | Marketo中未同步任何内容 |
| True | True | 联系人已在Marketo中同步 |
| False | True | 在Marketo中创建了新的联系记录 |
| True | False | MS Dynamics更新Marketo中的潜在客户信息，但联系记录未同步 |

>[!CAUTION]
>
>我们仅支持现成的资格转换流程。

