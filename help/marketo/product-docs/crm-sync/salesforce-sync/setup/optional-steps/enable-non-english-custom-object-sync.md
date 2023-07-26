---
unique-page-id: 4719302
description: 启用非英语自定义对象同步 — Marketo文档 — 产品文档
title: 启用非英语自定义对象同步
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 启用非英语自定义对象同步 {#enable-non-english-custom-object-sync}

如果将Marketo同步用户设置为英语以外的语言，则在尝试启用自定义对象同步时可能会遇到错误。

## 错误 {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 绕过它 {#getting-around-it}

1. 使用marketo同步用户登录Salesforce。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 在用户名下，转到 **设置**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 下 **个人信息**，单击 **我的个人信息**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 单击 **编辑**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 更改 **语言** 到 **英语**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 单击 **保存**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 返回Marketo，在 **管理员> Salesforce >对象** 单击 **刷新架构**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 这将拉取英文的对象列表。 现在，选择您选择的对象并单击 **启用同步**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 请注意，您的自定义对象现已启用并同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 现在，返回到Salesforce并使用上述步骤将同步用户更改回您的首选语言。

>[!NOTE]
>
>不要忘记最后一次刷新架构以用您的语言拉回对象。
