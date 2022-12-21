---
unique-page-id: 14352475
description: 在活动历史记录中安装Sales Connect事件字段 — Marketo文档 — 产品文档
title: 在活动历史记录中安装Sales Connect事件字段
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 在活动历史记录中安装Sales Connect事件字段 {#install-sales-connect-event-fields-on-activity-history}

将企业包安装到Salesforce后，您可以将Sales Connect事件字段安装到活动历史记录部分。 Sales Connect事件字段包括视图、点击和促销活动等信息。 这样，您就可以获得有关直接导入到Salesforce中的电子邮件的信息。

执行这些步骤时，请确保与Salesforce管理员合作。 在本例中，我们将在 **潜在客户页面布局**. 您还可以将这些字段安装到“联系人”、“帐户”和“机会页面布局”上。 请记住，在将电子邮件记录到Accounts和Opportunity时，您将需要您通过电子邮件发送的联系人作为联系人角色。

1. 单击 **设置**.
1. 单击 **自定义**.
1. 单击 **潜在客户**.
1. 单击 **页面布局**.
1. 单击 **编辑** 要更改的页面布局旁边。

   >[!NOTE]
   >
   >Sales Connect将为您安装一些页面布局，但如果您已经具有默认的页面布局，则您的团队将使用该页面布局进行安装。 如果您不想使用Sales Connect页面布局，则可以删除这些布局。

1. 向下滚动到活动历史记录部分。
1. 单击扳手进行编辑。
1. 选择要包含在活动历史记录部分中的Sales Connect字段。 如果此处未看到Sales Connect字段，则可能安装了错误的Salesforce包。
1. 单击 **添加** 来移动所需的字段。
1. 单击 **确定**.
1. 单击 **保存**.

   您的用户现在可以在Salesforce中看到有关其电子邮件的有价值信息和更新！
