---
description: 第1步（共3步） — 将Marketo字段添加到Salesforce (Enterprise/Unlimited) - Marketo文档 — 产品文档
title: 第1步（共3步） — 将Marketo字段添加到Salesforce (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 第1步（共3步）：将Marketo字段添加到Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>您必须有权访问Salesforce API，才能在Marketo Engage和Salesforce之间同步。

Marketo使用一组字段来捕获某些类型的营销相关信息。 如果您希望在Salesforce中使用此数据，请按照以下说明操作。

1. 在Salesforce中针对潜在客户和联系人对象创建三个自定义字段：“得分”、“客户获取计划”和“客户获取日期”。
1. 在潜在客户和联系人之间映射这些自定义字段，以便在Salesforce中进行转化时，值会延续。
1. 如有必要，您可以创建其他附加字段（请参阅下表）。

所有这些自定义字段都是可选的，并且不是同步Marketo和Salesforce的必需字段。 作为最佳实践，我们建议您为“得分”、“客户获取计划”和“客户获取日期”创建字段。

## 将Marketo字段添加到Salesforce {#add-marketo-fields-to-salesforce}

在上面列出的Salesforce中的潜在客户和联系人对象中添加三个自定义字段。 如果要添加更多字段，请参阅本节末尾的可用字段表。

对三个自定义字段中的每一个执行以下步骤以添加它们。 从得分开始。

1. 登录到Salesforce，然后单击“设置”。

   屏幕快照

1. 在快速查找中，搜索“对象”一词

   屏幕快照

1. 单击对象管理器并搜索“潜在客户”

   屏幕快照

1. 单击LABEL下的Lead ，然后单击左侧的Fields and Relationships。

   屏幕快照

1. 单击“字段和关系”页面中名为“新建”的按钮

   屏幕快照

1. 选择相应的字段类型（对于“得分 — 编号”、“客户获取计划 — 文本”、“客户获取日期 — 日期/时间”）。

   屏幕快照

1. 单击“下一步”。

   屏幕快照

1. 输入字段的字段标签、长度和字段名称，如下表所示。

   表

   >[!NOTE]
   >
   >当Salesforce使用字段名称创建API名称时，会将__c附加到字段名称。

   屏幕快照

   >[!NOTE]
   >
   >文本和数字字段需要长度，但日期/时间字段不需要。说明是可选的。

1. 单击“下一步”。

   屏幕快照

1. 指定访问设置，然后单击下一步：

   将所有角色设置为可见和只读

   清除同步用户配置文件的只读复选框：

   如果您的用户具有系统管理员的配置文件作为同步用户，请清除系统管理员配置文件的“只读”复选框（如下所示）
如果您为同步用户创建了自定义配置文件，请清除该自定义配置文件的“只读”复选框

   屏幕快照

1. 选择应显示该字段的页面布局。

   屏幕快照

1. 单击保存并新建以返回并创建其他两个自定义字段。 单击“保存” ，您已完成这三项。

   屏幕快照

* 在对象管理器中，搜索“联系人”。 单击“字段和关系”。
* 对联系对象的“得分”、“客户获取日期”和“客户获取计划”字段执行步骤5至12，就像对潜在客户对象执行操作一样。
* 或者，将上述过程用于此表的任何其他自定义字段。

  表

  >[!NOTE]
  >
  >创建新字段后，Marketo自动分配的字段中的值将无法立即在Salesforce中使用。 下次更新任一系统上的记录时(即，更新在Salesforce和Marketo之间同步的任何字段)，Marketo都会将数据同步到Salesforce。

## 映射用于转换的自定义字段 {#map-custom-fields-for-conversions}

Salesforce中商机对象上的自定义字段应映射到联系人对象上的联系人字段，以便在发生转化时保留数据。

1. 单击右上角的设置。

   屏幕快照

1. 在快速查找中，搜索“对象”一词

   屏幕快照

1. 转到Lead Custom Fields &amp; Relationship部分，然后单击Map Lead Fields

   屏幕快照

1. 单击要映射的字段旁边的下拉菜单，位于相应的选项卡 — 帐户、联系人或机会下。

   屏幕快照

1. 选择相应的联系人自定义字段。

   屏幕快照

1. 对创建的任何其他字段重复上述步骤。

1. 完成后单击保存。
