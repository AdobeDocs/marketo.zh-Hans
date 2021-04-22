---
unique-page-id: 3571797
description: 第2步（共3步） — 为Marketo（专业版）创建Salesforce用户 — Marketo文档 — 产品文档
title: 第2步（共3步） — 为Marketo创建Salesforce用户(Professional)
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---

# 第2步，共3步：为Marketo(Professional){#step-of-create-a-salesforce-user-for-marketo-professional}创建Salesforce用户

>[!NOTE]
>
>这些步骤必须由Salesforce管理员完成

>[!PREREQUISITES]
>
>[第1步，共3步：将Marketo字段添加到Salesforce(Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

在本文中，您将使用Salesforce页面布局自定义字段权限，并创建Marketo-Salesforce同步用户。

## 设置页面布局{#set-page-layouts}

Salesforce Professional使用“页面布局”设置字段级辅助功能，而不是Salesforce Enterprise/Unlimited的用户档案。 按照这些步骤操作，Marketo同步用户可以更新自定义字段。

1. 在Nav搜索栏中键入&#x200B;**页面布局**&#x200B;而不按&#x200B;**Enter**，然后单击&#x200B;**Lead**&#x200B;下的&#x200B;**页面布局**。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 单击“潜在客户布局”旁边的&#x200B;**编辑**。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 单击并将新&#x200B;**部分**&#x200B;拖入页面布局中。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 在&#x200B;**节名称**&#x200B;中输入“Marketo”，然后单击&#x200B;**确定**。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 单击字段&#x200B;**“Acquisition Date**”并将其拖动到&#x200B;**Marketo**&#x200B;部分。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 对以下字段重复上述步骤：

   * 赢取项目
   * 客户获取项目ID
   * 电子邮选择退出件
   * 推断城市
   * 推断公司
   * 推断国家
   * 推断的都市区
   * 推断出的电话区号
   * 推断的邮政编码
   * 推断的州
   * 潜在客户分数
   * 原始推荐人
   * 原始搜索引擎
   * 原始搜索短语
   * 原始源信息
   * 原始源类型

   >[!NOTE]
   >
   >这些字段必须位于页面布局中，以便Marketo能够读/写它们。

   >[!TIP]
   >
   >通过向下拖动到页面右侧，为字段创建两列。 您可以将字段从一侧移动到另一侧，以平衡列长。

1. 添加完字段后，单击&#x200B;**保存**。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 对Salesforce **联系页面布局**&#x200B;重复上述所有步骤。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 完成&#x200B;**联系页面布局**&#x200B;操作后，请记住单击&#x200B;**保存**。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >确保&#x200B;**全天事件**&#x200B;字段已添加到&#x200B;**事件页面布局**。

## 创建同步用户{#create-sync-user}

Marketo需要凭据才能访问Salesforce。 最好使用通过以下步骤创建的专用用户完成此操作。

>[!NOTE]
>
>如果您的组织没有其他Salesforce许可证，则您可以将现有的&#x200B;**营销用户**&#x200B;与&#x200B;**系统管理员**&#x200B;用户档案一起使用。

1. 在导航搜索栏中输入“users”，然后单击&#x200B;**管理用户**&#x200B;下的&#x200B;**用户**。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 单击&#x200B;**新建用户**。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填写必填字段，选择&#x200B;**用户许可证：Salesforce**，设置&#x200B;**用户档案:系统管理员**，选中&#x200B;**营销用户**&#x200B;并单击&#x200B;**保存**。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >确保您输入的电子邮件地址有效。 您需要以同步用户身份登录才能重置密码。

太棒了！ 现在，您有一个帐户，Marketo可以用它连接到Salesforce。 我们来吧。

>[!MORELIKETHIS]
>
>[第3步，共3步：Connect Marketo和Salesforce(Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
