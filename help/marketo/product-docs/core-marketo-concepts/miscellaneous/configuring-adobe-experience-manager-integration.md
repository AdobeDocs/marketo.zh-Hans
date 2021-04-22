---
unique-page-id: 30081815
description: 配置Adobe Experience Manager集成 — Marketo文档 — 产品文档
title: 配置Adobe Experience Manager集成
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 配置Adobe Experience Manager集成{#configuring-adobe-experience-manager-integration}

配置AEM，以便您能够访问、选择AEM资源并将其导入Marketo Design Studio。

>[!NOTE]
>
>**需要管理权限**

>[!CAUTION]
>
>目前，仅Firefox完全支持此功能。 Safari中不支持此功能，并且可能无法在最新版Chrome(v. 80)中工作，具体取决于您的SameSite Cookie设置。

1. 导航到Adobe Experience Manager(URL特定于您的公司)。

   ![](assets/one.png)

1. 您可以使用Adobe登录或在本地登录。 在此示例中，我们将在本地登录。

   ![](assets/two.png)

1. 在&#x200B;**工具**&#x200B;中，单击&#x200B;**操作**&#x200B;并选择&#x200B;**Web控制台**。

   ![](assets/2a.png)

1. 在您的浏览器中，搜索（Windows上的ctrl+f，Mac上的cmd+f）“Adobe Granite跨来源资源共享策略”。

   ![](assets/three.png)

1. 单击右侧的&#x200B;**+**&#x200B;符号。

   ![](assets/four.png)

1. 在&#x200B;**允许的来源(Regexp)**&#x200B;文本框中，键入`https://.*\.marketo\.com`并单击&#x200B;**保存**。

   ![](assets/five-psd.png)

1. 在页面顶部的标题中，单击&#x200B;**Web控制台**&#x200B;并选择&#x200B;**系统信息**。

   ![](assets/six.png)

1. 在“服务器信息”下，单击&#x200B;**重新启动**&#x200B;按钮。

   ![](assets/seven.png)

1. 单击&#x200B;**确定**&#x200B;进行确认。

   ![](assets/eight.png)

1. 在Marketo Classic中，单击&#x200B;**Admin**。

   ![](assets/nine.png)

1. 在“集成”下，选择&#x200B;**Adobe Experience Manager**。

   ![](assets/ten.png)

1. 单击&#x200B;**编辑**。

   ![](assets/eleven.png)

1. 输入您的AEM URL，然后单击&#x200B;**确定**。

   ![](assets/twelve.png)

   你都准备好了！ 您现在可以[将AEM资源导入Marketo Sky](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio)中的Design Studio。
