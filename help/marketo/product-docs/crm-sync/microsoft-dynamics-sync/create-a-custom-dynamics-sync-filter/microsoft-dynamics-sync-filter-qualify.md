---
unique-page-id: 10092977
description: Microsoft Dynamics同步过滤器 — 资格 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步过滤器 — Qualify
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Microsoft Dynamics同步过滤器：确定 {#microsoft-dynamics-sync-filter-qualify}

在Microsoft Dynamics中，如果要将潜在客户转换为联系人，请务必使用此默认的“鉴别”流程。 然后，将其同步到Marketo。

## 转换过程 {#the-conversion-process}

以下是过滤器在转换过程中的工作方式。

| 如果潜在客户同步筛选器为： | 联系人同步过滤器为： | 这是在Marketo |
|---|---|---|
| 假 | 假 | 在Marketo中未同步任何内容 |
| 真 | 真 | 联系人将在Marketo中同步 |
| 假 | 真 | 在Marketo中创建新联系人记录 |
| 真 | 假 | MS Dynamics会更新Marketo中的潜在客户信息，但联系记录未同步 |

>[!CAUTION]
>
>我们仅支持现成的资格转换流程。
