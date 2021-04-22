---
unique-page-id: 4719302
description: 启用非英语自定义对象同步 — Marketo Docs — 产品文档
title: 启用非英语自定义对象同步
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 启用非英语自定义对象同步{#enable-non-english-custom-object-sync}

如果您的Marketo sync用户设置为英语以外的语言，则在尝试启用自定义对象同步时可能会遇到错误。

## 错误{#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 绕过它{#getting-around-it}

1. 使用marketo同步用户登录到Salesforce。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 在用户名下，转到&#x200B;**Setup**。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 在&#x200B;**个人信息**&#x200B;下，单击&#x200B;**我的个人信息**。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 单击&#x200B;**编辑**。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 将&#x200B;**Language**&#x200B;更改为&#x200B;**English**。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 返回Marketo后，在&#x200B;**管理> Salesforce > Objects**&#x200B;下，单击&#x200B;**刷新模式**。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 这将用英语提取对象列表。 现在，选择您选择的对象并单击&#x200B;**启用同步**。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 请注意，您的自定义对象现已启用并同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 现在，返回Salesforce并使用上述步骤将同步用户更改回首选语言。

>[!NOTE]
>
>不要忘记最后一次刷新模式，以将对象拉回您的语言。
