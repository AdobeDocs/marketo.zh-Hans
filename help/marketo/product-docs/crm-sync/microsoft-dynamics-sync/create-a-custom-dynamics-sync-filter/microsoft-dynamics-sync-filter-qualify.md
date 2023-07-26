---
unique-page-id: 10092977
description: Microsoft Dynamics同步筛选器 — 资格 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步筛选器 — 限定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Microsoft Dynamics同步筛选器：符合条件 {#microsoft-dynamics-sync-filter-qualify}

当您想要在Microsoft Dynamics中将潜在客户转换为联系人时，请确保使用此默认的“限定”流程。 然后，将其同步到Marketo。

## 转换过程 {#the-conversion-process}

下面是这些过滤器在转换过程中的工作方式。

| 如果潜在客户同步过滤器为： | 联系人同步筛选器为： | 这是Marketo中的结果 |
|---|---|---|
| False | False | Marketo中未同步任何内容 |
| True | True | 该联系人已在Marketo中同步 |
| False | True | 在Marketo中创建新联系人记录 |
| True | False | MS Dynamics在Marketo中更新潜在客户信息，但联系人记录未同步 |

>[!CAUTION]
>
>我们仅支持现成的“确认资格”转换流程。
