---
unique-page-id: 4720218
description: 使用Adobe Tag Manager实施RTP - Marketo文档 — 产品文档
title: 使用Adobe Tag Manager实施RTP
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 使用Adobe Tag Manager实施RTP {#implementing-rtp-using-adobe-tag-manager}

要实施RTP标记，请按照以下安装说明操作：

1. 登录到您的RTP帐户。

1. 转到&#x200B;**[!UICONTROL Account Settings]**。

   a.如果您已从支持部门收到JavaScript标记 — 请继续执行步骤4。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. 登录您的[!DNL Dynamic Tag Manager]帐户([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))。

1. 转到&#x200B;**[!UICONTROL Dashboard]。**&#x200B;单击相关的Web属性。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. 转到&#x200B;**[!UICONTROL Rules]**，单击&#x200B;**[!UICONTROL Create New Rule]**。

1. 填写以下内容

   1. [!UICONTROL Name]： **Marketo RTP**
   1. [!UICONTROL Conditions] （折叠） ：在 — **[!UICONTROL Top of Page]**&#x200B;处触发规则
   1. [!UICONTROL Javascript] （折叠）：单击&#x200B;**[!UICONTROL Add New Script]**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 调用新标记：**Marketo RTP标记**

1. 从[!UICONTROL RTP tag]中删除以下代码

   * `<script type='text/javascript'>`
   * `</script>`

1. 粘贴RTP JavaScript标记。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >确保删除所有标记，并仅保留脚本本身（否`<script type='text/javascript'>` ， `</script>` ）

1. 单击脚本编辑器中的&#x200B;**[!UICONTROL Save Code]**&#x200B;和规则编辑器中的&#x200B;**[!UICONTROL Save Rule]**。

1. 在“规则”面板中，找到Marketo RTP页面加载规则，然后在&#x200B;**[!UICONTROL Actions]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Activate Rules]**。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **[!UICONTROL Verify]**&#x200B;它出现在所有页面上，包括登陆页面和子域。

   您可以通过右键单击网站的页面来执行此操作。 转到&#x200B;**[!UICONTROL Inspect Element]**，单击&#x200B;**[!UICONTROL Network]**，搜索： **RTP**。
