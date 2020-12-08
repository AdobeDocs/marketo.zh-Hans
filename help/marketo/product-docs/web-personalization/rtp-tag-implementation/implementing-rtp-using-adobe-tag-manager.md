---
unique-page-id: 4720218
description: 使用Adobe Tag Manager实施RTP - Marketo Docs —— 产品文档
title: 使用Adobe Tag Manager实现RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# 使用Adobe Tag Manager实现RTP {#implementing-rtp-using-adobe-tag-manager}

要实施RTP标签，请按照以下安装说明操作：

1. 登录RTP帐户。
1. 转到“帐 **户设置”。**

   如果您已从支持部门收到JavaScript标记——请继续执行步骤4。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 在“域”下，找到相关域，然后单击“ **生成标记**”。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. 登录Dynamic Tag Manager帐户([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))。
1. 去 **仪表板。** 单击相关的Web属性。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. 转至“ **规则”** ，单 **击“创建新规则”。**

1. 填写以下内容

   1. 名称： **Marketo RTP**
   1. 条件（折叠）:触发规则位 **置——页面顶部**
   1. Javascript（折叠）:单击“ **添加新脚本”**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 调用新标记： **Marketo RTP标签**
1. 从RTP标签中删除以下代码

   * `<script type='text/javascript'>`
   * `</script>`

1. 粘贴RTP JavaScript标签。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >确保删除所有标记并仅保留脚本本身( `<script type='text/javascript'>` 否， `</script>` )

1. 在脚 **本编辑器中** ，单击“保存代码”, **在规则编辑器中** 单击“保存规则”。

1. 在“规则”面板中，找到Marketo RTP页面加载规则，并在“操作”下拉 **菜单** 中选择 **激活规则**。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **验证** 它是否显示在所有页面上，包括登陆页和子域。

   您可以通过右键单击网站页面来完成此操作。 转至 **Inspect** Element，单击**网络，**搜索： **RTP**。
