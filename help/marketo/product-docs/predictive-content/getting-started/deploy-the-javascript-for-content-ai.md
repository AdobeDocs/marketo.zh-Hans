---
unique-page-id: 11385053
description: 部署JavaScript for Content-AI - Marketo Docs — 产品文档
title: 部署JavaScript for Content-AI
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# 部署JavaScript for Content-AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>根据购买日期，您的Marketo订阅可能包括Marketo Predictive Content或Content`<sup>AI</sup>`。 对于使用预测内容的用户，Marketo在2018年4月30日之前一直在启用“内容`<sup>AI</sup>`分析”功能。 要使这些功能在该日期之后继续运行，请联系您的Marketo客户成功经理以升级到Marketo内容`<sup>AI</sup>`。

要使用预测内容，您需要生成并设置RTP（Web个性化）`tag.`

## 生成标记{#generate-tag}

1. 登录您的预测内容帐户。 转到&#x200B;**帐户设置**。

   ![](assets/settings-dropdown-account-hands.png)

1. 在&#x200B;**域配置**&#x200B;中，找到相关域，然后单击&#x200B;**生成标记。**

   ![](assets/generate-tag.png)

1. 将“Web个性化”标签复制并粘贴到您网站的HTML中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >复制Web Personalization JavaScript标签，并将其作为页面标题中的第一个脚本粘贴到`<head> </head>`标签之间。 请参阅此处的更详细[实施说明](https://docs.marketo.com/display/docs/rtp+tag+implementation) [。](https://pages2.marketo.com/rtp-implementation.html)

1. 验证标记是否显示在所有页面上，包括登陆页和子域。 右键单击`website’s`页面可选中此选项。 在Web浏览器中转至&#x200B;**视图页面源**。 搜索：“RTP”。
1. 确认将“标记”切换设置为&#x200B;**ON**。

