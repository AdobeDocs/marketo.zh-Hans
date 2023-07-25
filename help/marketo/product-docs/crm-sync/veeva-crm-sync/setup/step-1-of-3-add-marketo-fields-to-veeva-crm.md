---
description: 第1步（共3步） — 将Marketo字段添加到Veeva CRM - Marketo文档 — 产品文档
title: 第1步（共3步） — 将Marketo字段添加到Veeva CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 6%

---

# 第1步（共3步）：将Marketo字段添加到Veeva CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>您的Veeva CRM实例必须有权访问Salesforce API，以便在Marketo Engage和Veeva CRM之间同步数据。

Marketo Engage使用一组字段来捕获特定类型的营销相关信息。 如果您希望将此数据放在Veeva CRM中，请按照下面的说明操作。

`1.` 在Veeva CRM中为联系人对象创建一个自定义字段：分数

`2.` 如果需要，您可以创建其他字段（请参阅下表）。

所有这些自定义字段都是可选的，并且不是同步Marketo Engage和Veeva CRM的必需字段。

## 将Marketo字段添加到Veeva CRM {#add-marketo-fields-to-veeva-crm}

在上面列出的Veeva CRM中的潜在客户和联系人对象中添加自定义字段。 如果要添加更多，请参阅此部分末尾的可用字段表。

要添加“分数”字段，请执行以下步骤。

1. 登录到Veeva CRM并单击 **设置**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. 单击对象和字段，然后选择对象管理器。

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. 在搜索栏中，搜索联系人。

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. 单击“联系人”对象。

1. 选择字段和关系。

1. 单击 **新**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. 选择相应的字段类型（对于“分数 — 数字”）。

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. 单击 **下一个**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. 输入字段的字段标签、长度和字段名称，如下表所示。

<table>
 <tbody>
  <tr>
   <th>字段标签
   <th>字段名称
   <th>数据类型
   <th>字段属性
  </tr>
  <tr>
   <td>得分</td>
   <td>mkto71_Lead_Score</td>
   <td>数字</td>
   <td>长度10<br/>
小数位0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Veeva CRM在创建API名称时，会将__c附加到字段名称。

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>文本和数字字段需要长度，但日期/时间字段不需要。描述是可选的。

1. 单击 **下一个**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. 指定访问设置并单击 **下一个**.

1. 将所有角色设置为可见和只读。

1. 清除同步用户配置文件的“只读”复选框：

* 如果某个用户具有系统管理员的配置文件作为同步用户，请清除系统管理员配置文件的“只读”复选框（如下所示）。
* 如果您为同步用户创建了自定义配置文件，请清除该自定义配置文件的“只读”复选框。

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. 选择应显示字段的页面布局。

1. 单击 **保存并新建** 以返回并创建另外两个自定义字段。

1. 单击 **保存** 等你都吃完了。

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>通过将字段添加到联系人对象，也可以将其添加到人员帐户对象。

可选：对下表中的任何其他自定义字段使用上述过程。

<table>
 <tbody>
  <tr>
   <th>字段标签
   <th>字段名称
   <th>数据类型
   <th>字段属性
  </tr>
  <tr>
   <td>推断的城市</td>
   <td>mkto71_Inferred_City</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>推断公司</td>
   <td>mkto71_Inferred_Company</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>推断的国家</td>
   <td>mkto71_Inferred_Country</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>推断的都市区</td>
   <td>mkto71_Inferred_Metropolitan_Area</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>推断的电话区号</td>
   <td>mkto71_Inferred_Phone_Area_Code</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>推断的邮政编码</td>
   <td>mkto71_Inferred_Postal_Code</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>推断的状态区域</td>
   <td>mkto71_Inferred_State_Region</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>创建新字段后，Marketo自动分配的字段中的值不会立即在Veeva CRM中可用。 在对任一系统上的记录进行下一次更新时(即对Marketo和Veeva CRM之间同步的任何字段的更新)，Marketo会将数据同步到Veeva CRM。
