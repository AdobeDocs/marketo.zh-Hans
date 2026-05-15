---
unique-page-id: 10092977
description: 了解将潜在客户转化为联系人时的Dynamics同步过滤器资格流程。 了解潜在客户和联系人同步筛选器值如何影响Marketo同步。
title: Microsoft Dynamics同步筛选器 — 限定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/3jC9Y9fpBNjUzjE1Dy7JBuhNlYQpnc7kjF2LxV-hrp4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 116
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步筛选器：符合条件 {#microsoft-dynamics-sync-filter-qualify}

当您想要在[!DNL Microsoft Dynamics]中将潜在客户转换为联系人时，请使用此默认的“限定”流程。 然后，将其同步到Marketo。

## 转换过程 {#the-conversion-process}

| 如果潜在客户同步过滤器为： | 联系人同步筛选器为： | 这是Marketo中的结果 |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Marketo中未同步任何内容 |
| [!UICONTROL True] | [!UICONTROL True] | 该联系人已在Marketo中同步 |
| [!UICONTROL False] | [!UICONTROL True] | 在Marketo中创建新联系人记录 |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics]更新Marketo中的潜在客户信息，但联系人记录未同步 |

>[!CAUTION]
>
>我们仅支持现成的“确认资格”转换流程。
