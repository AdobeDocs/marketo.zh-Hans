---
unique-page-id: 14352404
description: “管理设置”选项卡- Marketo Docs —— 产品文档
title: “管理员设置”选项卡
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# 管理设置选项卡{#admin-settings-tab}

“管理员设置”选项卡将允许任何帐户的管理员查看其团队的设置（与计划限制相关），以及成批控制其团队电子邮件登录Salesforce的方式。

如果选中&#x200B;**覆盖我的团队**&#x200B;的所有Salesforce同步设置复选框，您将看到选项，该选项将仅允许通过BCC进行记录，或仅允许通过API进行记录。

如果选择&#x200B;**API日志**，则在单击&#x200B;**保存更改**&#x200B;后，将为整个团队设置为Opportunity、Lead和Contacts的所有设置。

从此处，您还可以在整个团队中大量启用Opportunity和任务同步。

>[!NOTE]
>
>批量启用这些设置将在团队的Salesforce设置中使用大量API调用。

1. 启用“配置我的团队的设置”。

1. 启用团队范围同步设置。

1. 配置您希望如何将电子邮件活动和最近的MSE活动记录到SFDC。

1. 启用“同步销售连接任务”是可选的。

>[!NOTE]
>
>MSC允许您跳过任务，而SFDC不允许，因此您必须决定SFDC如何处理跳过任务的。
