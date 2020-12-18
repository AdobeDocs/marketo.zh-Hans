---
unique-page-id: 14352404
description: “管理设置”选项卡- Marketo Docs —— 产品文档
title: “管理员设置”选项卡
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 管理设置选项卡{#admin-settings-tab}

“管理员设置”选项卡将允许任何帐户的管理员查看其团队的设置（与计划限制相关），以及成批控制其团队电子邮件登录Salesforce的方式。

如果选中&#x200B;**覆盖我的团队**&#x200B;的所有Salesforce同步设置复选框，您将看到选项，该选项将仅允许通过BCC进行记录，或仅允许通过API进行记录。

如果选择&#x200B;**API日志**，则为Opportunity、Lead和Contacts `will be set for the entire team after you click **Save Changes**.`选择的所有设置

从此处，您还可以在整个团队中大量启用Opportunity和任务同步。

>[!NOTE]
>
>批量启用这些设置将在团队的Salesforce设置中使用大量API调用。

1 —— 启用“配置我的团队的设置”

2 —— 启用团队范围同步设置

3 —— 配置您希望如何将电子邮件活动和最新的MSE活动记录到SFDC

4 —— 启用“同步销售连接任务”是可选的

(附注：MSE允许您跳过任务，而SFDC不允许，因此您必须决定SFDC如何处理跳过任务的)
