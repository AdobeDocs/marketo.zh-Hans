---
description: 第2步（共3步） — 创建Veeva CRM用户以进行Marketo Engage- Marketo文档 — 产品文档
title: 第2步（共3步） — 创建用于Marketo Engage的Veeva CRM用户
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 4%

---

# 第2步（共3步）：创建Veeva CRM用户以进行Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>本文中的步骤必须由Veeva CRM管理员完成。

>[!PREREQUISITES]
>
>[第1步（共3步）：将Marketo字段添加到Salesforce（专业）](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

在本文中，您将使用Veeva CRM页面布局自定义字段权限，并创建Marketo-Veeva CRM同步用户。

## 设置页面布局 {#set-page-layouts}

执行以下步骤将允许Marketo同步用户更新自定义字段。

1. 单击Nav搜索栏中的“帐户（人员帐户）”页面布局，而不按Enter，然后单击“联系人”下的“页面布局”。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. 单击 **页面布局**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. 单击 **HCP — 专业**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. 单击并拖动新的 **章节** 进入页面布局。

1. 在区域名称中输入“Marketo”，然后单击 **确定**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. 单击并将得分字段拖动到Marketo部分中。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. 对以下字段重复上述步骤：

   * 推断的城市
   * 推断公司
   * 推断国家
   * 推断的都市区
   * 推断的电话区号
   * 推断的邮政编码
   * 推断的状态区域

   >[!NOTE]
   >
   >这些字段需要在页面布局中，以便Marketo可以对其执行读/写操作。

   >[!TIP]
   >
   >通过向下拖到页面右侧，为字段创建两列。 您可以将字段从一侧移动到另一侧，以平衡列长度。

1. 完成HCP专业版面配置后，单击 **保存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

>[!NOTE]
>
>对其他“帐户”页面布局重复此操作。

## 创建配置文件 {#create-a-profile}

1. 单击 **设置**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. 在导航搜索栏中键入“profiles”，然后单击 **配置文件** 链接。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. 单击 **新**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. 选择“标准用户”，将配置文件命名为“Marketo-Salesforce Sync”，然后单击 **保存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## 设置配置文件权限 {#set-profile-permissions}

1. 单击 **编辑** 以设置安全权限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. 在“管理权限”部分下，确保选中“已启用API”。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >确保选中“密码永不过期”框。

1. 在“常规用户权限”部分下，确保选中编辑事件和编辑任务。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. 在“标准对象权限”部分下，确保选中“帐户”和“联系人”的“读取”、“创建”、“编辑”和“删除”权限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. 在“自定义对象权限”部分下，确保选中Call、Call Key Message和任何其他所需的“自定义对象”的“读取”权限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. 完成后，单击 **保存** 页面底部的。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## 设置字段权限 {#set-field-permissions}

1. 与您的营销人员讨论，了解哪些自定义字段是同步所必需的。

>[!NOTE]
>
>此步骤将阻止您不需要的字段显示在Marketo中，这将减少杂乱并加快同步速度。

1. 在用户档案详细信息页面中，转到字段级安全性部分。 单击“查看”可编辑Contact和Account对象的辅助功能。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

>[!TIP]
>
>您可以根据组织的需求配置其他对象。

1. 对于每个对象，单击 **编辑**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

找到不必要的字段，确保读取权限和编辑权限 **un**&#x200B;已选中。 单击 **保存** 完成时。

![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

>[!NOTE]
>
>仅编辑自定义字段的辅助功能。

1. 禁用完所有不必要的字段后，请选中以下对象字段的读取访问和编辑访问。 完成后单击保存。

<table>
 <tbody>
  <tr>
   <th>对象
   <th>字段
  </tr>
  <tr>
   <td>帐户</td>
   <td>类型字段</td>
  </tr>
  <tr>
   <td>Event</td>
   <td>所有字段</td>
  </tr>
  <tr>
   <td>任务</td>
   <td>所有字段</td>
  </tr>
 </tbody>
</table>

## 创建同步用户 {#create-sync-user}

Marketo需要凭据才能访问Veeva CRM。 最好是通过以下步骤创建的专用用户来完成此操作。

>[!NOTE]
>
>如果您的组织没有其他Veeva CRM许可证，则可以使用具有系统管理员配置文件的现有营销用户。

1. 在导航搜索栏中输入“用户”，然后单击 **用户** 在“管理用户”下。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. 单击 **新用户**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. 填写必填字段，选择用户许可证：Salesforce，设置配置文件：Marketo同步用户，然后单击 **保存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>确保您输入的电子邮件地址有效。 您需要以同步用户身份登录才能重置密码。

太棒了！ 现在，您有一个帐户，Marketo Engage可以使用它连接到Veeva CRM。 我们开始吧。

>[!MORELIKETHIS]
>
>[第3步（共3步）：连接Marketo和Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
