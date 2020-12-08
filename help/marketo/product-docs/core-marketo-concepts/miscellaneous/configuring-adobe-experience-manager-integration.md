---
unique-page-id: 30081815
description: 配置Adobe Experience Manager集成- Marketo Docs —— 产品文档
title: 配置Adobe Experience Manager集成
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 配置Adobe Experience Manager集成 {#configuring-adobe-experience-manager-integration}

配置AEM，以便您能够访问、选择AEM资产并将其导入Marketo的Design Studio。

>[!NOTE]
>
>**需要管理员权限**

>[!CAUTION]
>
>目前，仅Firefox完全支持此功能。 Safari中不支持，并且可能在最新版Chrome(v. 80)中无法使用，具体取决于您的SameSite cookie设置。

1. 导航到Adobe Experience Manager(URL特定于您的公司)。

   ![](assets/one.png)

1. 您可以使用Adobe登录或在本地登录。 在此示例中，我们将在本地登录。

   ![](assets/two.png)

1. 在“ **工具**”中，单 **击“操作** ” **，然后选**&#x200B;择“Web控制台”。

   ![](assets/2a.png)

1. 在您的浏览器中，搜索（Windows上的ctrl+f,Mac上的cmd+f）“AdobeGranite跨来源资源共享策略”。

   ![](assets/three.png)

1. 单击 **右** 侧的+符号。

   ![](assets/four.png)

1. 在“允 **许的来源** (Regexp)”文本框中，键入“https://”。*\.marketo\.com”（不带引号），然后单击“保 **存”**。

   ![](assets/five-psd.png)

1. 在页面顶部的标题中，单击“Web控 **制台”** ，然后选择 **“系统信息”**。

   ![](assets/six.png)

1. 在“服务器信息”下，单击“重 **新启** 动”按钮。

   ![](assets/seven.png)

1. 单击 **确定** ，以进行确认。

   ![](assets/eight.png)

1. 在Marketo Classic中，单击“管 **理员**”。

   ![](assets/nine.png)

1. 在“集成”下，选择 **Adobe Experience Manager**。

   ![](assets/ten.png)

1. 单击 **编辑**。

   ![](assets/eleven.png)

1. 输入AEM URL，然后单击“ **确定**”。

   ![](assets/twelve.png)

   你们都准备好了！ 您现在可 [以Marketo Sky将AEM资源导入Design Studio](http://help.marketo.com/hc/en-us/articles/360036765993)。

