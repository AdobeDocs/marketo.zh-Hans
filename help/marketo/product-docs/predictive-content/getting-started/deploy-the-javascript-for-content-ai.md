---
unique-page-id: 11385053
description: 部署JavaScript for Content-AI - Marketo文档 — 产品文档
title: 部署JavaScript for Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# 部署JavaScript for Content-AI {#deploy-the-javascript-for-content-ai}

要使用预测内容，您需要生成和设置RTP（Web个性化）标记。

## 生成标记 {#generate-tag}

1. 登录到您的预测内容帐户。 转到 **帐户设置**.

   ![](assets/settings-dropdown-account-hands.png)

1. In **域配置**，找到相关域并单击 **生成标记**.

   ![](assets/generate-tag.png)

1. 将Web个性化标记复制并粘贴到网站的HTML中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >复制Web个性化JavaScript标记，并将其粘贴为页面标题中的第一个脚本，介于 `<head> </head>` 标记之间。 查看更多详细信息 [此处为实施说明](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. 验证标记是否出现在所有页面上，包括登陆页面和子域。 右键单击您网站的页面以检查此项。 转到 **查看页面源** 在Web浏览器中。 搜索：“RTP”。

1. 确认标记切换开关设置为 **日期**.
