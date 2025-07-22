---
unique-page-id: 10092977
description: Microsoft Dynamics同步过滤器 — 符合条件 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步筛选器 — 限定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步筛选器：符合条件 {#microsoft-dynamics-sync-filter-qualify}

当您想要在[!DNL Microsoft Dynamics]中将潜在客户转换为联系人时，请确保使用此默认资格验证流程。 然后，将其同步到Marketo。

## 转换过程 {#the-conversion-process}

下面是这些过滤器在转换过程中的工作方式。

| 如果潜在客户同步过滤器为： | 联系人同步筛选器为： | 这是Marketo中的结果 |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Marketo中未同步任何内容 |
| [!UICONTROL True] | [!UICONTROL True] | 该联系人已在Marketo中同步 |
| [!UICONTROL False] | [!UICONTROL True] | 在Marketo中创建新联系人记录 |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics]更新Marketo中的潜在客户信息，但联系人记录未同步 |

>[!CAUTION]
>
>我们仅支持现成的“确认资格”转换流程。
