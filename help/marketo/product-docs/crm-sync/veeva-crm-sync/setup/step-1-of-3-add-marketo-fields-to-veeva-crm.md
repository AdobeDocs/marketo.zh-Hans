---
description: 第1步（共3步） — 将Marketo字段添加到 [!DNL Veeva] CRM - Marketo文档 — 产品文档
title: 第1步（共3步） — 将Marketo字段添加到 [!DNL Veeva] CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 8%

---

# 第1步（共3步）：将Marketo字段添加到[!DNL Veeva] CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>您的[!DNL Veeva] CRM实例必须有权访问Salesforce API，以便在Marketo Engage和[!DNL Veeva] CRM之间同步数据。

Marketo Engage使用一组字段来捕获某些类型的营销相关信息。 如果您希望在[!DNL Veeva] CRM中使用此数据，请按照下面的说明操作。

1. 在[!DNL Veeva] CRM中针对联系人对象创建一个自定义字段：分数
1. 如果需要，您可以创建其他字段（请参阅下表）。

所有这些自定义字段都是可选的，并且不是同步Marketo Engage和[!DNL Veeva] CRM的必需字段。

## 将Marketo字段添加到[!DNL Veeva] CRM {#add-marketo-fields-to-veeva-crm}

在上面列出的[!DNL Veeva] CRM中的潜在客户和联系人对象中添加自定义字段。 如果要添加更多字段，请参阅本节末尾的可用字段表。

要添加Score字段，请执行以下步骤。

1. 登录到[!DNL Veeva] CRM并单击&#x200B;**[!UICONTROL Setup]**。

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. 单击&#x200B;**[!UICONTROL Objects and Fields]**&#x200B;并选择&#x200B;**[!UICONTROL Object Manager]**。

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. 在搜索栏中，搜索“联系人”。

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. 单击&#x200B;**[!UICONTROL Contact]**&#x200B;对象。

1. 选择 **[!UICONTROL Fields and Relationships]**。

1. 单击 **[!UICONTROL New]**。

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. 选择相应的字段类型（对于“分数 — 数字”）。

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. 为字段输入&#x200B;**[!UICONTROL Field Label]**、**[!UICONTROL Length]**&#x200B;和&#x200B;**[!UICONTROL Field Name]**，如下表所示。

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
   <td>数值</td>
   <td>长度10<br/>
小数位0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>[!DNL Veeva] CRM在创建API名称时将__c附加到字段名称。

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>文本和数字字段需要长度，但日期/时间字段不需要。说明是可选的。

1. 单击 **[!UICONTROL Next]**。

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. 指定访问设置并单击&#x200B;**[!UICONTROL Next]**。

1. 将所有角色设置为&#x200B;**[!UICONTROL Visible]**&#x200B;和&#x200B;**[!UICONTROL Read-Only]**。

1. 清除同步用户配置文件的&#x200B;**[!UICONTROL Read-Only]**&#x200B;复选框：

* 如果您的用户具有系统管理员的配置文件作为同步用户，请清除系统管理员配置文件的[!UICONTROL Read-Only]复选框（如下所示）。
* 如果您为同步用户创建了自定义配置文件，请清除该自定义配置文件的[!UICONTROL Read-Only]复选框。

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. 选择应显示该字段的页面布局。

1. 单击&#x200B;**[!UICONTROL Save & New]**&#x200B;返回并创建其他两个自定义字段。

1. 完成全部三个操作后，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>通过将字段添加到Contact对象，也可以将其添加到Person Account对象。

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
>创建新字段后，Marketo自动分配的字段中的值将不能立即在[!DNL Veeva] CRM中使用。 下次更新任一系统上的记录时(即更新在Marketo和[!DNL Veeva] CRM之间同步的任何字段)，Marketo会将数据同步到[!DNL Veeva] CRM。
