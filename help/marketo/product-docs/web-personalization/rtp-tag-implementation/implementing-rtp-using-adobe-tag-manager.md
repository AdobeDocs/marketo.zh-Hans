---
unique-page-id: 4720218
description: 使用Adobe Tag Manager实施RTP - Marketo Docs — 产品文档
title: 使用Adobe Tag Manager实现RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# 使用Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}实现RTP

要实施RTP标签，请按照以下安装说明操作：

1. 登录到RTP帐户。

1. 转到&#x200B;**帐户设置**。

   a.如果您已从“支持”收到JavaScript标记 — 请继续执行步骤4。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 在“Domain（域）”下，找到相关域，然后单击“Generate Tag **（生成标记**）”。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. 登录Dynamic Tag Manager帐户([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))。

1. 转到&#x200B;**仪表板。** 单击相关的Web属性。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. 转至&#x200B;**规则**，单击&#x200B;**创建新规则**。

1. 填写以下内容

   1. 名称：**Marketo RTP**
   1. 条件（折叠）：触发规则位于 — **页面顶部**
   1. Javascript（折叠）：单击&#x200B;**添加新脚本**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 调用新标记：**Marketo RTP标签**

1. 从RTP标签中删除以下代码

   * `<script type='text/javascript'>`
   * `</script>`

1. 粘贴RTP JavaScript标签。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >确保删除所有标记，并仅保留脚本本身（无`<script type='text/javascript'>`、`</script>`）

1. 单击脚本编辑器中的&#x200B;**保存代码**&#x200B;和规则编辑器中的&#x200B;**保存规则**。

1. 在“规则”面板中，找到Marketo RTP页面加载规则，并在&#x200B;**操作**&#x200B;下拉列表中选择&#x200B;**激活规则**。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **验** 证它是否显示在所有页面上，包括登陆页和子域。

   您可以通过右键单击网站页面来执行此操作。 转至&#x200B;**Inspect元素**，单击&#x200B;**网络**，搜索：**RTP**。
