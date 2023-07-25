---
description: 路径 — Marketo文档 — 产品文档
title: 路由
exl-id: 9515c264-7d9b-4613-a245-15620c846a5c
feature: Dynamic Chat
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 1%

---

# 路由 {#routing}

以Dynamic Chat预订的会议可通过两种方式路由。 循环调度程序，或使用自定义规则。

轮询：会议按顺序分配给座席。 如果你有5个座席，3个座席，参加最后一个会议，4个座席，接着是5个座席，然后回到1号座席。

自定义规则：您可以根据所选的属性选择特定座席来接收会议。

## 创建自定义规则 {#create-a-custom-rule}

在此示例中，我们将所有推断的状态为CA、OR和WA的会议发送给John座席。

1. 在Dynamic Chat中，选择 **路由**.

   ![](assets/routing-1.png)

1. 单击 **自定义规则** 选项卡。

   ![](assets/routing-2.png)

1. 单击 **创建规则**.

   ![](assets/routing-3.png)

1. 为规则命名，然后单击 **下一个**.

   ![](assets/routing-4.png)

1. 选择所需的代理。

   ![](assets/routing-5.png)

1. 拖动到所需的属性上。

   ![](assets/routing-6.png)

1. 查找并选择所需的值。

   ![](assets/routing-7.png)

1. 选择所有所需值后，单击 **保存**.

   ![](assets/routing-8.png)
