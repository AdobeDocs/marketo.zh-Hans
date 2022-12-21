---
description: 步骤2（共3步） — 为Marketo Engage创建Veve CRM用户 — Marketo文档 — 产品文档
title: 步骤2（共3步） — 创建Veeva CRM用户以进行Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 4%

---

# 步骤2（共3步）：创建Veeva CRM用户以进行Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>本文中的步骤必须由Veeva CRM管理员完成。

>[!PREREQUISITES]
>
>[步骤1（共3步）：将Marketo字段添加到Salesforce（专业版）](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;}

在本文中，您将使用Veeva CRM页面布局自定义字段权限，并创建Marketo-Veeva CRM同步用户。

## 设置页面布局 {#set-page-layouts}

执行这些步骤后，Marketo同步用户将可以更新自定义字段。

1. 在导航搜索栏中单击“帐户（人员帐户）”页面布局，而不按Enter键，然后单击“联系人”下的“页面布局”。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. 单击 **页面布局**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. 单击 **HCP — 专业**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. 单击并拖动新 **区域** 到页面布局中。

1. 在“节名称”中输入“Marketo”，然后单击 **确定**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. 单击并将Score字段拖动到Marketo部分。

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
   >这些字段需要位于页面布局上，以便Marketo能够读取/写入它们。

   >[!TIP]
   >
   >通过向下拖动到页面右侧为字段创建两列。 您可以将字段从一侧移动到另一侧，以平衡列长度。

1. 完成HCP-Professional布局后，单击 **保存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

>[!NOTE]
>
>对其他“帐户页面布局”重复此操作。

## 创建用户档案 {#create-a-profile}

1. 单击 **设置**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. 在导航搜索栏中键入“profiles”，然后单击 **用户档案** 链接。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. 单击 **新建**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. 选择“标准用户”，将配置文件命名为“Marketo-Salesforce同步”，然后单击 **保存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## 设置配置文件权限 {#set-profile-permissions}

1. 单击 **编辑** 来设置安全权限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. 在管理权限部分下，确保选中已启用API。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >确保选中密码永不过期框。

1. 在“常规用户权限”部分下，确保选中编辑事件和编辑任务。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. 在标准对象权限部分下，确保为帐户和联系人选中读取、创建、编辑和删除权限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. 在“自定义对象权限”部分下，确保选中“调用”、“调用密钥消息”和任何其他所需的自定义对象的读取权限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. 完成后，单击 **保存** 页面底部。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## 设置字段权限 {#set-field-permissions}

1. 与营销人员讨论，以了解同步所需的自定义字段。

>[!NOTE]
>
>此步骤将阻止您不需要的字段在Marketo中显示，这将减少杂乱并加快同步速度。

1. 在用户档案详细信息页面中，转到字段级别安全部分。 单击“查看”(View)可编辑联系人和帐户对象的辅助功能。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

>[!TIP]
>
>您可以根据组织的需求配置其他对象。

1. 对于每个对象，单击 **编辑**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

找到不必要的字段，确保具有读取访问权限和编辑访问权限 **联合国**&#x200B;选中。 单击 **保存** 完成时。

![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

>[!NOTE]
>
>仅编辑自定义字段的辅助功能。

1. 在禁用所有不必要的字段后，请选中以下对象字段的读取访问和编辑访问。 完成后，单击保存。

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

Marketo需要凭据才能访问Veeva CRM。 最好使用通过以下步骤创建的专用用户来完成此操作。

>[!NOTE]
>
>如果贵组织没有其他Veva CRM许可证，则可以将现有营销用户与系统管理员配置文件一起使用。

1. 在导航搜索栏中输入“用户”，然后单击 **用户** 在“管理用户”下。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. 单击 **新用户**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. 填写必填字段，选择用户许可证：Salesforce中，设置用户档案：Marketo同步用户并单击 **保存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>确保您输入的电子邮件地址有效。 您需要以同步用户身份登录才能重置密码。

太棒了！ 现在，您拥有一个Marketo Engage可用于连接到Veeva CRM的帐户。 我们来吧。

>[!MORELIKETHIS]
>
>[步骤3（共3步）：连接Marketo和Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target=&quot;_blank&quot;}
