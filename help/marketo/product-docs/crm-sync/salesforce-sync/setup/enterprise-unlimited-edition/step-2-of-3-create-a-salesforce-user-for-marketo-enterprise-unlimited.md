---
unique-page-id: 2360364
description: 第2步（共3步） — 为Marketo创建Salesforce用户（企业/无限制） — Marketo文档 — 产品文档
title: 第2步（共3步） — 为Marketo创建Salesforce用户（企业/无限制）
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 2%

---

# 步骤2（共3步）：为Marketo创建Salesforce用户（企业/无限制） {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>这些步骤必须由Salesforce管理员完成

>[!PREREQUISITES]
>
>[步骤1（共3步）：将Marketo字段添加到Salesforce（企业/无限制）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

在本文中，您将在Salesforce配置文件中设置用户权限，并创建Marketo-Salesforce集成帐户。

## 创建用户档案 {#create-a-profile}

1. 单击 **设置**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. 在导航搜索栏中键入“profiles”，然后单击 **用户档案** 链接。

   ![](assets/sfdc-profiles-hands.png)

1. 单击 **新建**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. 选择 **标准用户**，将配置文件命名为“Marketo-Salesforce同步”，然后单击 **保存**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## 设置配置文件权限 {#set-profile-permissions}

1. 单击 **编辑** 来设置安全权限。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. 在 **管理权限** 部分，确保选中以下框：

   * 已启用API
   * 编辑HTML模板
   * 管理公共文档
   * 管理公共模板

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >请务必检查 **密码永不过期** 框中。

1. 在“常规用户权限”部分下，确保选中以下框：

   * 转换潜在客户
   * 编辑事件
   * 编辑任务

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. 在标准对象权限部分下，确保选中读取、创建、编辑和删除权限：

   * 帐户
   * 促销活动
   * 联系人
   * 潜在客户
   * 机会

   >[!NOTE]
   >
   >如果您计划使用营销活动同步，则授予营销活动权限。

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. 完成后，单击 **保存** 页面底部。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## 设置字段权限 {#set-field-permissions}

1. 与营销人员讨论，以了解同步所需的自定义字段。

   >[!NOTE]
   >
   >此步骤将阻止您不需要的字段在Marketo中显示，这将减少杂乱并加快同步速度。

1. 在用户档案详细信息页面中，转到 **字段级别安全性** 中。 单击 **查看** 要编辑对象的辅助功能，请执行以下操作：

   * 商机
   * 联系人
   * 帐户
   * 机会

   >[!TIP]
   >
   >您可以根据组织的需求配置其他对象。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 对于每个对象，单击 **编辑**.

   ![](assets/sfdc-sync-field-edit1.png)

1. 找到不需要的字段，确保 **读取访问** 和 **编辑访问** ，则不会选中。 单击 **保存** 等你完事了。

   >[!NOTE]
   >
   >仅编辑自定义字段的辅助功能。

   ![](assets/sfdc-sync-field-edit2.png)

1. 禁用所有不需要的字段后，必须检查 **读取访问和编辑访问** ，用于以下对象字段。 单击 **保存** 等你完事了。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>对象</p></th> 
   <th colspan="1" rowspan="1"><p>字段</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>帐户</p></td> 
   <td colspan="1" rowspan="1"><p>类型字段</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Event</p></td> 
   <td colspan="1" rowspan="1"><p>所有字段</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>任务</p></td> 
   <td colspan="1" rowspan="1"><p>所有字段</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## 创建Marketo-Salesforce同步帐户 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>创建专用的Salesforce帐户(例如marketo@yourcompany.com)，以区分Marketo与其他Salesforce用户所做的更改。

1. 在导航搜索栏中键入“管理用户”，然后单击 **用户**. 单击 **新用户**.

   ![](assets/sfdc-new-users.png)

1. 填写必填字段。 然后，选择 **用户许可证：Salesforce** 以及您之前创建的配置文件。 单击 **保存** 等你完事了。

   ![](assets/image2014-12-9-9-3a20-3a56.png)

步骤2（共2步）已完成。

>[!NOTE]
>
>[步骤3（共3步）：连接Marketo和Salesforce（企业/无限制）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
