---
unique-page-id: 3571797
description: 第2步（共3步） — 为Marketo创建Salesforce用户（专业版） — Marketo文档 — 产品文档
title: 步骤2（共3步） — 为Marketo创建Salesforce用户（专业版）
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 4%

---

# 步骤2（共3步）：为Marketo创建Salesforce用户（专业版） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>这些步骤必须由Salesforce管理员完成

>[!PREREQUISITES]
>
>[步骤1（共3步）：将Marketo字段添加到Salesforce（专业版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

在本文中，您将使用Salesforce页面布局自定义字段权限，并创建Marketo-Salesforce同步用户。

## 设置页面布局 {#set-page-layouts}

Salesforce Professional使用“页面布局”设置字段级别的辅助功能，而不是Salesforce Enterprise/Unlimited的“配置文件”。 执行这些步骤后，Marketo同步用户将可以更新自定义字段。

1. 类型 **页面布局** 搜索栏中，而不按 **输入**，然后单击 **页面布局** 在 **潜在客户**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 单击 **编辑** “潜在客户布局”旁边。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 单击并拖动新 **区域** 到页面布局中。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 输入“Marketo”表示 **节名称** 单击 **确定**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 单击并拖动字段 **客户获取日期** 到 **Marketo** 中。

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
   * 原始源信息
   * 原始源类型

   >[!NOTE]
   >
   >这些字段需要位于页面布局上，以便Marketo能够读取/写入它们。

   >[!TIP]
   >
   >通过向下拖动到页面右侧为字段创建两列。 您可以将字段从一侧移动到另一侧，以平衡列长度。

1. 单击 **保存** 完成添加字段时。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 为Salesforce重复上述所有步骤 **联系页面布局**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 请记住单击 **保存** 你什么时候 **联系页面布局**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >确保 **全天事件** 字段 **事件页面布局**.

## 创建同步用户 {#create-sync-user}

Marketo需要凭据才能访问Salesforce。 最好使用通过以下步骤创建的专用用户来完成此操作。

>[!NOTE]
>
>如果贵组织没有其他Salesforce许可证，则可以使用现有 **营销用户** 和 **系统管理员** 配置文件。

1. 在导航搜索栏中输入“用户”，然后单击 **用户** 在 **管理用户**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 单击 **新用户**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填写必填字段，选择 **用户许可证：Salesforce**，请设置 **用户档案：系统管理员**，勾选 **营销用户** 单击 **保存**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >确保您输入的电子邮件地址有效。 您需要以同步用户身份登录才能重置密码。

太棒了！ 现在，您拥有一个Marketo可用于连接到Salesforce的帐户。 我们来吧。

>[!MORELIKETHIS]
>
>[步骤3（共3步）：连接Marketo和Salesforce(Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
