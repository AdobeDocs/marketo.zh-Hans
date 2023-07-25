---
unique-page-id: 3571797
description: 第2步（共3步） — 创建Salesforce用户以使用Marketo （专业） - Marketo文档 — 产品文档
title: 第2步（共3步） — 创建Salesforce User for Marketo（专业）
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 8%

---

# 第2步（共3步）：创建Salesforce用户以使用Marketo（专业） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>这些步骤必须由Salesforce管理员完成

>[!PREREQUISITES]
>
>[第1步（共3步）：将Marketo字段添加到Salesforce（专业）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

在本文中，您将使用Salesforce页面布局自定义字段权限，并创建Marketo-Salesforce同步用户。

## 设置页面布局 {#set-page-layouts}

Salesforce Professional使用页面布局设置字段级辅助功能，而不是Salesforce Enterprise/Unlimited的Profiles。 执行以下步骤将允许Marketo同步用户更新自定义字段。

1. 类型 **页面布局** 导航搜索栏中，不按 **输入**，然后单击 **页面布局** 下 **潜在客户**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 单击 **编辑** 在“潜在客户布局”旁边。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 单击并拖动新的 **章节** 进入页面布局。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 输入“Marketo”作为 **分区名称** 并单击 **确定**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 单击并拖动字段 **客户获取日期** 到 **Marketo** 部分。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 对以下字段重复上述步骤：

   * 客户获取计划
   * 客户获取计划ID
   * 电子邮件选择退出
   * 推断的城市
   * 推断公司
   * 推断国家
   * 推断的都市区
   * 推断的电话区号
   * 推断的邮政编码
   * 推断的状态区域
   * 潜在客户分数
   * 原始反向链接
   * 原始搜索引擎
   * 原始搜索短语
   * 原始来源信息
   * 原始来源类型

   >[!NOTE]
   >
   >这些字段需要在页面布局中，以便Marketo可以对其执行读/写操作。

   >[!TIP]
   >
   >通过向下拖到页面右侧，为字段创建两列。 您可以将字段从一侧移动到另一侧，以平衡列长度。

1. 单击 **保存** 添加完字段后。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 对Salesforce重复上述所有步骤 **联系人页面布局**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 请记住单击 **保存** 当您使用 **联系人页面布局**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >确保 **全天活动** 字段已添加到 **事件页面布局**.

## 创建同步用户 {#create-sync-user}

Marketo需要凭据才能访问Salesforce。 最好是通过以下步骤创建的专用用户来完成此操作。

>[!NOTE]
>
>如果您的组织没有其他Salesforce许可证，则可以使用现有的 **营销用户** 使用 **系统管理员** 个人资料。

1. 在导航搜索栏中输入“用户”，然后单击 **用户** 下 **管理用户**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 单击 **新用户**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填写必填字段，然后选择 **用户许可证： Salesforce**，设置 **配置文件：系统管理员**，检查 **营销用户** 并单击 **保存**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >确保您输入的电子邮件地址有效。 您需要以同步用户身份登录才能重置密码。

太棒了！ 现在，您已拥有Marketo可用于连接到Salesforce的帐户。 我们开始吧。

>[!MORELIKETHIS]
>
>[第3步（共3步）：连接Marketo和Salesforce（专业）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
