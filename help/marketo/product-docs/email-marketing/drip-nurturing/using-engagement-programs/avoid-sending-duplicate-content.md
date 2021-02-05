---
unique-page-id: 10096409
description: 避免发送重复内容- Marketo Docs —— 产品文档
title: 避免发送重复内容
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# 避免发送重复内容{#avoid-sending-duplicate-content}

您收到过两次相同的电子邮件吗？ 烦人，不是吗？

以下是七个可能的情况和结果，可以防止与参与项目两次发送相同的消息。

## 方案{#scenarios}

人员会收到从客户参与引擎发送的电子邮件。

| 电子邮件的发送方 | 此人是 | Person获得电子邮件 |
|---|---|---|
| 单独、默认活动中的项目 | 不是默认项目的成员 | 是 |
| 单独、默认活动中的项目 | 默认项目的成员 | 否 |
| 默认项目内的活动，从&#x200B;**same** CEE项目内的转播触发 | 默认项目的成员 | 否 |
| 默认项目内的活动，从&#x200B;**same** CEE项目内的转播触发 | 不是默认项目的成员 | 是 |
| 默认项目内的活动，从&#x200B;**不同的** CEE项目内的转播触发 | 默认项目的成员 | 否 |
| 默认项目内的活动，从&#x200B;**不同的** CEE项目内的转播触发 | 不是默认项目的成员 | 是 |
| 使用智能流的&#x200B;**不同的** CEE项目 | 两个CEE项目的成员 | 否 |
