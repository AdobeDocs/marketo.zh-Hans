---
unique-page-id: 4720218
description: 使用Adobe Tag Manager实施RTP - Marketo文档 — 产品文档
title: 使用Adobe Tag Manager实施RTP
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 使用Adobe Tag Manager实施RTP {#implementing-rtp-using-adobe-tag-manager}

要实施RTP标记，请按照以下安装说明操作：

1. 登录到您的RTP帐户。

1. 转到 **帐户设置**.

   a.如果您已从“支持”处收到JavaScript标记，请继续执行步骤4。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 在“域”下，找到相关域并单击 **生成标记**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. 登录您的Dynamic Tag Manager帐户([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))。

1. 转到 **功能板。** 单击相关的Web属性。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. 转到 **规则**，单击 **创建新规则**.

1. 填写以下内容

   1. 名称： **Marketo RTP**
   1. 条件（折叠）：触发规则位置 —  **页面顶部**
   1. Javascript（折叠）：单击 **添加新脚本**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 调用新标记： **Marketo RTP标记**

1. 从RTP标记中删除以下代码

   * `<script type='text/javascript'>`
   * `</script>`

1. 粘贴RTP JavaScript标记。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >确保删除所有标记并仅保留脚本本身（否） `<script type='text/javascript'>` , `</script>` )

1. 单击 **保存代码** 和 **保存规则** 在规则编辑器中。

1. 在“规则”面板中，找到Marketo RTP页面加载规则，并在 **操作** 下拉选择 **激活规则**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **验证** 显示在所有页面上（包括登陆页面和子域）。

   您可以通过右键单击您网站的页面来执行此操作。 转到 **Inspect元素**，单击 **网络**，搜索： **RTP**.
