---
description: 路径 — Marketo文档 — 产品文档
title: 路由
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 863e5e542e2006ee15f44ad949e876e56a9b39e3
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# 路由 {#routing}

以Dynamic Chat预订的会议可以采用两种方式路由。 循环调度法，或使用自定义规则。

轮询：会议按顺序分配给座席。 如果你有5个座席，3个座席，参加上次会议，4个座席，接下一个，5个座席，然后返回1号座席。

自定义规则：您可以根据所选的属性选择特定座席以接收会议。

## 创建自定义规则 {#create-a-custom-rule}

在此示例中，我们将所有推断的状态（CA、OR和WA）的会议发送给John座席。

1. 在配置下，单击 **路由规则**.

   ![](assets/routing-1.png)

1. 单击 **自定义规则** 选项卡。

   ![](assets/routing-2.png)

1. 单击 **创建规则**.

   ![](assets/routing-3.png)

1. 命名您的规则。 （可选）您可以添加说明并设置其优先级。 单击 **下一个**.

   ![](assets/routing-4.png)

1. 选择所需的座席。

   ![](assets/routing-5.png)

1. 将拖到所需的属性上。

   ![](assets/routing-6.png)

1. 查找并选择所需的值。

   ![](assets/routing-7.png)

1. 选择所有所需值后，单击 **保存**.

   ![](assets/routing-8.png)

## 帐户路由 {#account-routing}

识别并上传您的目标帐户和各自的销售负责人，并将来自这些帐户的访客直接路由到各自的帐户负责人。

![](assets/routing-9.png)

团队路由

智能列表路由的成员
