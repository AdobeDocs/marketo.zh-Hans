---
description: 排除销售活动和字段无法同步到Salesforce的问题。 检查API日志记录、自定义字段和权限。
title: 为什么我的销售活动和活动字段没有同步到 Salesforce？
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 03f984d4049c119267c7b2c2baa4e68c7db34ad0
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 6%

---

# 为什么我的销售活动和活动字段没有同步到 Salesforce？ {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**我看不到同步到Salesforce的电子邮件或呼叫活动。**

* 确保已连接到Salesforce。 每个用户都需要拥有连接才能将其电子邮件和呼叫记录到Salesforce。
* 确保您已配置[Salesforce同步设置](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}。
* 电子邮件将基于Salesforce ID执行记录查找，作为主要查找，而电子邮件地址作为次要查找。 您可以在[操作Web应用](https://toutapp.com/next#command_center){target="_blank"}中确认人员记录具有链接到他们的Salesforce ID和电子邮件地址。
* 调用将仅根据Salesforce ID执行记录查找。 如果操作中的人员记录中不存在Salesforce ID，则不会记录调用。 您可以在[操作Web应用](https://toutapp.com/next#command_center){target="_blank"}中确认人员记录具有链接到他们的Salesforce ID。

**我在Salesforce更新中未看到活动字段。**

如果您在Salesforce中未看到电子邮件[活动属性字段](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}更新，则可能是由于您团队的字段可访问性受到限制所致。 Salesforce字段级别的安全性使Salesforce管理员能够围绕用户可查看和编辑的信息设置限制。 如果“操作”用户无权查看和编辑这些字段，则“操作”活动同步将无法更新这些字段。

* 请与您的Salesforce管理员合作，确保这些安全设置不会影响[操作Salesforce活动字段](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}。
* 如果您是Salesforce管理员，则可以在“安全控制”选项卡下方看到您的字段可访问性。 活动将与的主要对象包括：销售线索、联系人、帐户、业务机会和任务/活动。

>[!NOTE]
>
>与Lead 、 Contact 、 Account和Opportunity对象关联的字段将随Sales Insight Salesforce包一起安装。 与[任务/活动记录类型关联的字段需要由Salesforce管理员创建](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}。
