---
description: 为什么我的销售活动和活动字段没有同步到Salesforce？ - Marketo文档 — 产品文档
title: 为什么我的销售活动和活动字段没有同步到Salesforce？
exl-id: 0836876d-1b89-4464-a841-81320a6e45fd
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 为什么我的销售活动和活动字段没有同步到Salesforce？ {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**我没有看到电子邮件或呼叫活动同步到Salesforce。**

* 确保已连接到Salesforce。 每个用户都需要拥有连接才能将其电子邮件和呼叫记录到Salesforce。
* 确保您已配置 [Salesforce同步设置](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* 电子邮件将根据Salesforce ID作为主要查找进行记录查找，并将电子邮件地址作为次要查找。 您可以在中确认人员记录是否具有链接到他们的Salesforce ID和电子邮件地址 [操作Web应用程序](https://toutapp.com/next#command_center){target="_blank"}.
* 调用将仅根据Salesforce ID执行记录查找。 如果“操作”中的人员记录中不存在Salesforce ID，则不会记录调用。 您可以在中确认人员记录具有与其关联的Salesforce ID [操作Web应用程序](https://toutapp.com/next#command_center){target="_blank"}.

**在Salesforce更新中看不到活动字段。**

如果您没有看到电子邮件 [活动属性字段](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} 在Salesforce中进行更新，这可能是由于您团队的字段可访问性受到限制所致。 Salesforce字段级安全保护，使Salesforce管理员能够对用户可查看和编辑的信息设置限制。 如果“操作”用户无权查看和编辑这些字段，则“操作”活动同步将无法更新这些字段。

* 与您的Salesforce管理员合作，确保这些安全设置不会受到干扰 [Actions Salesforce Activity字段](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* 如果您是Salesforce管理员，则可以在“安全控制”选项卡下看到“字段可访问性”。 活动将与的主要对象包括：销售线索、联系人、帐户、业务机会和任务/活动。

>[!NOTE]
>
>与Lead 、 Contact 、 Account和Opportunity对象关联的字段将随Sales Insight Salesforce包一起安装。 与关联的字段 [需要创建任务/活动记录类型](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} 由Salesforce管理员创建。
