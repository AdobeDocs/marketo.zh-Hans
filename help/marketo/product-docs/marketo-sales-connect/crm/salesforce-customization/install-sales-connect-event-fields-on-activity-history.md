---
unique-page-id: 14352475
description: 安装活动历史记录中的Sales Connect事件字段- Marketo Docs —— 产品文档
title: 在事件历史记录上安装Sales Connect活动字段
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 在事件历史记录上安装Sales Connect活动字段 {#install-sales-connect-event-fields-on-activity-history}

将Enterprise包安装到Salesforce后，您可以将Sales Connect事件字段安装到活动历史记录部分。 Sales Connect事件字段包括视图、点击和活动等信息。 这允许您将电子邮件的相关信息直接导入Salesforce。

确保在执行这些步骤时与您的Salesforce管理员进行协作。 在此示例中，我们将将字段安装到Lead **页面布局中**。 您还可以将字段安装到“联系人”、“帐户”和“业务机会页面布局”中。 请记住，在将电子邮件记录到帐户和业务机会时，您将需要您以联系角色身份发送电子邮件的联系人。

1. 单击“ **设置**”。
1. 单击“ **自定义**”。
1. 单击 **潜在客户**。
1. 单击“ **页面布局**”。
1. 单击 **要更改** 的页面布局旁边的“编辑”。

   >[!NOTE]
   >
   >Sales Connect将为您安装一些页面布局，但如果您已经使用了默认的页面布局，您将希望在该处安装它。 如果不想使用Sales Connect页面布局，可以删除这些布局。

1. 向下滚动到“活动历史记录”部分。
1. 单击扳手进行编辑。
1. 在“活动历史记录”部分选择要包括的Sales Connect字段。 如果此处未看到Sales Connect字段，则可能安装了错误的Salesforce包。
1. 单击 **添加** ，将所需字段移到上方。
1. 单击 **确定**。
1. 单击 **保存**。

   您的用户现在可以在Salesforce中查看有关其电子邮件的宝贵信息和更新！

