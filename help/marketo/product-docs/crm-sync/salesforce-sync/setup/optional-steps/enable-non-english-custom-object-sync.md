---
unique-page-id: 4719302
description: 了解如何在Marketo同步用户使用非英语语言时启用自定义对象同步。 在Salesforce中将同步用户语言设置为英语并刷新模式。
title: 启用非英语自定义对象同步
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 7%

---

# 启用非英语自定义对象同步 {#enable-non-english-custom-object-sync}

如果将Marketo同步用户设置为英语以外的语言，则在尝试启用自定义对象同步时可能会遇到错误。

## 错误 {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 绕过它 {#getting-around-it}

1. 使用marketo同步用户登录[!DNL Salesforce]。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 在用户名下，转到&#x200B;**[!UICONTROL Setup]**。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 在&#x200B;**[!UICONTROL Personal Information]**&#x200B;下，单击&#x200B;**[!UICONTROL My Personal Information]**。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 单击 **[!UICONTROL Edit]**。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 将&#x200B;**[!UICONTROL Language]**&#x200B;更改为&#x200B;**[!UICONTROL English]**。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 返回Marketo，在&#x200B;**[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objects]**&#x200B;下，单击&#x200B;**[!UICONTROL Refresh Schema]**。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 这将拉取英文的对象列表。 现在选择您选择的对象并单击&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 请注意，您的自定义对象现已启用并同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 现在，返回[!DNL Salesforce]并使用上述步骤将同步用户更改回您的首选语言。

>[!NOTE]
>
>不要忘记最后一次刷新架构以用您的语言拉回对象。
