---
unique-page-id: 9437340
description: 使用Tealium Tag Manager实施RTP - Marketo文档 — 产品文档
title: 使用Tealium标签管理器实施RTP
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# 使用Tealium标签管理器实施RTP {#implementing-rtp-using-tealium-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的Tealium Tag Manager帐户。

1. 导航到“标记”选项卡，然后添加Tealium自定义容器标记，该标记位于标记市场的“杂项”选项卡下。

1. 在标题字段中，输入 **MARKETO RTP** 并单击 **完成**.

1. 保存更改。

   >[!NOTE]
   >
   >尚不需要发布新容器。

1. 保存配置文件后，单击Tealium iQ控制台右上角的姓名/电子邮件地址。

1. 在管理员菜单中，单击 **管理模板** 在“帐户管理员”下。

1. 选择 **Tealium自定义容器：Marketo RTP** 以打开标记模板。

1. 登录到您的RTP帐户。

1. 转到“帐户设置”。

   >[!NOTE]
   >
   >如果您已从支持部门收到JavaScript标记，请继续执行步骤11。

1. 在“域”下，找到相关域并单击 **生成标记**.

1. 复制RTP JavaScript标记，并将其粘贴到Tealium配置文件模板的“开始标记库代码”和“结束标记库代码”之间。

   >[!NOTE]
   >
   >**重要步骤**
   >
   >删除 `<!-- RTP tag -->` 和 `<!-- End of RTP tag -->` 来自您放置在此文件中的代码的标记。
   >
   >删除任意 `<script type='text/javascript'>` 和 `</script>` 来自您放置在此文件中的代码的标记。

1. **单击保存配置文件模板** 并发布您的新配置文件。
