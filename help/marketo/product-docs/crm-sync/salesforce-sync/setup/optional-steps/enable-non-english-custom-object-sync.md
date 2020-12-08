---
unique-page-id: 4719302
description: 启用非英语自定义对象同步- Marketo Docs —— 产品文档
title: 启用非英语自定义对象同步
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# 启用非英语自定义对象同步 {#enable-non-english-custom-object-sync}

如果您的Marketo同步用户设置为英语以外的语言，则在尝试启用自定义对象同步时可能会遇到错误。

## 错误 {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 避开它 {#getting-around-it}

1. 使用marketo同步用户登录Salesforce。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 在用户名下，转到“设 **置”**。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 在“个 **人信息**”下，单 **击“我的个人信息”**。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 单击 **编辑**。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 将“语言 **”** 更改 **为英语**。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 单击 **保存**。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 返回Marketo，在“管理员”> **“Salesforce”>“对象”下** ，单 **击“刷新模式**”。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 这将用英文提取对象列表。 现在，选择您选择的对象，然后单击“启 **用同步”**。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 请注意，您的自定义对象现已启用并同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 现在返回Salesforce并使用上述步骤将同步用户更改回首选语言。

>[!NOTE]
>
>**提醒**
>
>不要忘记最后一次刷新模式以将对象拉回您的语言。

