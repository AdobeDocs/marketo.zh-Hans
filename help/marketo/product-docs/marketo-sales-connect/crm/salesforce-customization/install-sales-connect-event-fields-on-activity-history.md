---
unique-page-id: 14352475
description: 在活动历史记录中安装Sales Connect事件字段 — Marketo文档 — 产品文档
title: 在活动历史记录上安装Sales Connect事件字段
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 在活动历史记录上安装Sales Connect事件字段 {#install-sales-connect-event-fields-on-activity-history}

将Enterprise软件包安装到Salesforce中后，您可以将Sales Connect事件字段安装到活动历史记录部分。 Sales Connect事件字段包括查看、点击和促销活动等信息。 这样，您可以将有关电子邮件的信息直接导入到Salesforce中。

执行这些步骤时，请确保与Salesforce管理员组成团队。 在此示例中，我们将这些字段安装到 **潜在客户页面布局**. 您还可以将字段安装到Contact 、 Account和Opportunity页面布局中。 请记住，在将电子邮件记录到“客户”和“业务机会”时，您将需要作为联系人角色发送电子邮件给您的联系人。

1. 单击 **设置**.
1. 单击 **自定义**.
1. 单击 **潜在客户**.
1. 单击 **页面布局**.
1. 单击 **编辑** 在要更改的页面布局旁边。

   >[!NOTE]
   >
   >Sales Connect将为您安装一些页面布局，但如果您已经有一个默认页面布局，您的团队将使用它进行安装。 如果您不想使用Sales Connect页面布局，可以将其删除。

1. 向下滚动到“活动历史记录”部分。
1. 单击要编辑的扳手。
1. 选择要包含在Activity History部分中的Sales Connect字段。 如果您未在此处看到Sales Connect字段，则表明您可能安装了错误的Salesforce包。
1. 单击 **添加** 将所需字段移到。
1. 单击 **确定**.
1. 单击 **保存**.

   您的用户现在可以在Salesforce中查看有关其电子邮件的宝贵信息和更新！
