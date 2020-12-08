---
unique-page-id: 3571797
description: 步骤2（共3步）-为Marketo（专业）创建Salesforce用户- Marketo文档——产品文档
title: 第2步（共3步）-为Marketo创建Salesforce用户（专业）
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---


# 第2步，共3步：为Marketo创建Salesforce用户(Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>这些步骤必须由Salesforce管理员完成

>[!NOTE]
>
>**先决条件**
>
>* [第1步，共3步：将Marketo字段添加到Salesforce(Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

>



在本文中，您将使用Salesforce页面布局自定义字段权限并创建Marketo-Salesforce同步用户。

## 设置页面布局 {#set-page-layouts}

Salesforce Professional通过页面布局设置字段级别的辅助功能，而不是Salesforce Enterprise/Unlimited的用户档案。 按照这些步骤操作，Marketo将允许用户同步自定义字段。

1. 在 **导航条** （无需按Enter）键入页面布 **局**，然后单击Lead下的Page **Layout** (页面布 ****&#x200B;局)。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 单击“ **潜在客** 户布局”旁边的“编辑”。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 单击并将新的 **Section** 拖入页面布局。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 在“章节名称”中输 **入“Marketo** ”，然 **后单击“OK**”。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 单击并将字段“ **客户获取日期** ”拖 **入Marketo部** 分。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 对以下字段重复上述步骤：

   * 赢取项目
   * 客户获取项目ID
   * 电子邮件选择退出
   * 推断城市
   * 推断公司
   * 推断国家
   * 推断的都市区
   * 推断电话区号
   * 推断的邮政编码
   * 推断的州区
   * 潜在客户得分
   * 原始推荐人
   * 原始搜索引擎
   * 原始搜索短语
   * 原始源信息
   * 原始源类型

   >[!NOTE]
   >
   >这些字段必须位于页面布局中，这样Marketo才能读／写它们。

   >[!TIP]
   >
   >通过向下拖动到页面右侧，为字段创建两列。 您可以将字段从一侧移动到另一侧，以平衡列长度。

1. 添加完 **字段后** ，单击“保存”。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 对“Salesforce联系人页面”布局重复 **上述所有步骤**。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 完成“联 **系人** ”页面布局后，请 **记住单击“保存”**。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >确保“全 **天事件** ”字段已添加到 **事件页面布局**。

## 创建同步用户 {#create-sync-user}

Marketo需要凭据才能访问Salesforce。 这对于使用以下步骤创建的专用用户是最好的。

>[!NOTE]
>
>如果您的组织没有其他Salesforce许可证，则可以使用具有系统管 **理员用户档案** 的现 **有Marketing用户** 。

1. 在导航搜索栏中输入“用户”，然后单击“管 **理用户** ”下 **的“用户”**。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 单击“ **新建用户**”。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填写必填字段，选择用 **户许可证：Salesforce**，设置 **用户档案:系统管理员**，选中“ **Marketing User** ”，然后单 **击“保存**”。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >确保您输入的电子邮件地址有效。 您需要以同步用户身份登录才能重置密码。

太棒了！ 现在，您有一个帐户，Marketo可使用它连接到Salesforce。 我们来吧。

>[!NOTE]
>
>**相关文章**
>
>* [第3步，共3步：Connect Marketo和Salesforce(Professional)](step-3-of-3-connect-marketo-and-salesforce-professional.md)

>



