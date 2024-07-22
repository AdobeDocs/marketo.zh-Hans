---
unique-page-id: 9437340
description: 使用Tealium Tag Manager实施RTP - Marketo文档 — 产品文档
title: 使用Tealium标签管理器实施RTP
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# 使用Tealium标签管理器实施RTP {#implementing-rtp-using-tealium-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的Tealium Tag Manager帐户。

1. 导航到“标记”选项卡，然后添加Tealium自定义容器标记，该标记位于标记市场的“杂项”选项卡下。

1. 在“标题”字段中，输入&#x200B;**Marketo RTP**&#x200B;并单击&#x200B;**完成**。

1. 保存更改。

   >[!NOTE]
   >
   >尚不需要发布新容器。

1. 保存配置文件后，单击Tealium iQ控制台右上角的姓名/电子邮件地址。

1. 在“管理员”菜单中，单击“帐户管理员”下的&#x200B;**管理模板**。

1. 从下拉列表中选择&#x200B;**Tealium自定义容器： Marketo RTP**&#x200B;以打开“标记”模板。

1. 登录到您的RTP帐户。

1. 转到“帐户设置”。

   >[!NOTE]
   >
   >如果您已从支持部门收到JavaScript标记，请继续执行步骤11。

1. 在“域”下，找到相关域，然后单击&#x200B;**生成标记**。

1. 复制RTP JavaScript标记，并将其粘贴到Tealium配置文件模板的“开始标记库代码”和“结束标记库代码”之间。

   >[!NOTE]
   >
   >**重要步骤**
   >
   >从您放置在此文件中的代码中删除`<!-- RTP tag -->`和`<!-- End of RTP tag -->`标记。
   >
   >从您放置在此文件中的代码中删除任何`<script type='text/javascript'>`和`</script>`标记。

1. **单击“保存配置文件模板”**&#x200B;并发布您的新配置文件。
