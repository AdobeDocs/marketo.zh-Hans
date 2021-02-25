---
unique-page-id: 9437340
description: 使用Tealium Tag Manager - Marketo Docs — 产品文档实施RTP
title: 使用Tealium标签管理器实现RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 使用Tealium标签管理器{#implementing-rtp-using-tealium-tag-manager}实现RTP

要实施RTP标签，请按照以下安装说明操作。

1. 登录到Tealium Tag Manager帐户。

1. 导航到“标记”选项卡，并添加位于“标记”市场的“杂项”选项卡下的“定制容器标记”。

1. 在“标题”字段中，输入&#x200B;**Marketo RTP**&#x200B;并单击&#x200B;**完成**。

1. 保存更改。

   >[!NOTE]
   >
   >现在还不需要发布新容器。

1. 保存用户档案后，单击Tealium iQ控制台右上角的您的姓名/电子邮件地址。

1. 在“管理员”菜单上，单击“帐户管理员”下的“管理模板&#x200B;**”。**

1. 选择&#x200B;**Tealium自定义容器:从下拉列表中将RTP**&#x200B;标记为打开标记模板。

1. 登录到RTP帐户。

1. 转到“帐户设置”。

   >[!NOTE]
   >
   >如果您已从“支持”收到JavaScript标记，请继续执行步骤11。

1. 在“Domain（域）”下，找到相关域，然后单击“Generate Tag **（生成标记**）”。

1. 复制RTP JavaScript标签并将其粘贴到Tealium开始模板中的JavaScript标签库代码和End Tag Library Code之间。

   >[!NOTE]
   >
   >**重要步骤**
   >
   >从此文件中放置的代码中删除`<!-- RTP tag -->`和`<!-- End of RTP tag -->`标签。
   >
   >从此文件中放置的代码中删除任何`<script type='text/javascript'>`和`</script>`标记。

1. **单击“保存用户档案** 模板”并发布新用户档案。
