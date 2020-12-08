---
unique-page-id: 9437340
description: 使用Tealium标签管理器实施RTP - Marketo文档——产品文档
title: 使用Tealium标签管理器实现RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 使用Tealium标签管理器实现RTP {#implementing-rtp-using-tealium-tag-manager}

要实施RTP标签，请按照下面的安装说明操作。

1. 登录Tealium Tag Manager帐户。
1. 导航到“标记”选项卡，并添加“标记自定义容器标记”，该标记位于“标记”市场的“杂项”选项卡下。
1. 在标题字段中，输入 **Marketo RTP** ，然后单 **击完成**。
1. 保存更改。

   >[!NOTE]
   >
   >还不需要发布新容器。

1. 保存用户档案后，单击Tealium iQ控制台右上角的您的姓名／电子邮件地址。
1. 在“管理员”菜单中，单击“帐 **户管理员** ”下的“管理模板”。
1. 选择 **Tealium自定义容器:从下拉列表** 将RTP标记为打开标记模板。
1. 登录RTP帐户。
1. 转到“帐户设置”。

   >[!NOTE]
   >
   >如果您已从“支持”收到JavaScript标记，请继续执行步骤11。

1. 在“域”下，找到相关域，然后单击“ **生成标记**”。
1. 复制RTP JavaScript标签并将其粘贴到Tealium开始模板中的用户档案标签库代码和结束标签库代码之间。

   >[!NOTE]
   >
   >**重要步骤**
   >
   >从此文 `<!-- RTP tag -->` 件 `<!-- End of RTP tag -->` 中放置的代码中删除和标记。
   >
   >从此文 `<script type='text/javascript'>` 件 `</script>` 中放置的代码中删除任何和标记。

1. **单击“保存用户档案模板** ”，然后发布新用户档案。

