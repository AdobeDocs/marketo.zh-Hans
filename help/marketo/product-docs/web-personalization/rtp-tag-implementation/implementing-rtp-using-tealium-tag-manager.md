---
unique-page-id: 9437340
description: 使用Tealium Tag Manager实施RTP - Marketo文档 — 产品文档
title: 使用 Tealium 标记管理器实施 RTP
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 4%

---

# 使用[!DNL Tealium]标记管理器实施RTP {#implementing-rtp-using-tealium-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的[!DNL Tealium]标签管理器帐户。

1. 导航到[!UICONTROL Tags]选项卡并添加[!UICONTROL Tealium Custom Container Tag]，它位于标记市场的[!UICONTROL Misc]选项卡下。

1. 在[!UICONTROL Title field]中，输入&#x200B;**Marketo RTP**&#x200B;并单击&#x200B;**[!UICONTROL Finish]**。

1. 保存更改。

   >[!NOTE]
   >
   >尚不需要发布新容器。

1. 保存配置文件后，单击Tealium iQ控制台右上角的姓名/电子邮件地址。

1. 在[!UICONTROL Admin]菜单上，单击&#x200B;**[!UICONTROL Manage Templates]**&#x200B;下的[!UICONTROL Account Admin]。

1. 从下拉列表中选择&#x200B;**[!UICONTROL Tealium Custom Container]： Marketo RTP**&#x200B;以打开Tag模板。

1. 登录到您的RTP帐户。

1. 转到[!UICONTROL Account Settings]。

   >[!NOTE]
   >
   >如果您已从支持部门收到JavaScript标记，请继续执行步骤11。

1. 在域下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

1. 复制RTP JavaScript标记并将其粘贴到Tealium配置文件模板中的[!UICONTROL Start Tag Library Code]和[!UICONTROL End Tag Library Code]之间。

   >[!NOTE]
   >
   >**重要步骤**
   >
   >从您放置在此文件中的代码中删除`<!-- RTP tag -->`和`<!-- End of RTP tag -->`标记。
   >
   >从您放置在此文件中的代码中删除任何`<script type='text/javascript'>`和`</script>`标记。

1. 单击&#x200B;**[!UICONTROL Save Profile Template]**&#x200B;并发布新配置文件。
