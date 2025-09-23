---
unique-page-id: 2360362
description: 第1步（共3步） — 将Marketo字段添加到Salesforce (Enterprise/Unlimited) - Marketo文档 — 产品文档
title: 第1步（共3步） — 将Marketo字段添加到Salesforce (Enterprise/Unlimited)
exl-id: bcfba281-0d4b-42c3-b52a-ce1c3da884ba
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 9%

---

# 第1步（共3步）：将Marketo字段添加到[!DNL Salesforce] (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>您必须有权访问[!DNL Salesforce] API才能在Marketo和[!DNL Salesforce]之间同步。

Marketo使用一组字段来捕获某些类型的营销相关信息。 如果您希望在[!DNL Salesforce]中使用此数据，请按照下面的说明操作。

1. 在[!DNL Salesforce]中针对潜在客户和联系人对象创建三个自定义字段：“得分”、“客户获取计划”和“客户获取日期”。
1. 在潜在客户和联系人之间映射这些自定义字段，以便在[!DNL Salesforce]中的转化时，值会延续。
1. 如有必要，您可以创建其他附加字段（请参阅下表）。

所有这些自定义字段都是可选的，不需要这些字段来同步Marketo和[!DNL Salesforce]。 作为最佳实践，我们建议您为“得分”、“客户获取计划”和“客户获取日期”创建字段。

## 将Marketo字段添加到[!DNL Salesforce] {#add-marketo-fields-to-salesforce}

在以上列出的[!DNL Salesforce]中的潜在客户和联系人对象中添加三个自定义字段。 如果要添加更多字段，请参阅本节末尾的可用字段表。

对三个自定义字段中的每一个执行以下步骤以添加它们。 从得分开始。

1. 登录到[!DNL Salesforce]并单击&#x200B;**[!UICONTROL Setup]**。

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 在左侧的“生成”菜单中，单击&#x200B;**[!UICONTROL Customize]**&#x200B;并选择&#x200B;**[!UICONTROL Leads]**。 单击 **[!UICONTROL Fields]**。

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. 单击页面底部“自定义字段和关系”部分中的&#x200B;**[!UICONTROL New]**。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 选择相应的字段类型（对于“得分 — 编号”、“客户获取计划 — 文本”、“客户获取日期 — 日期/时间”）。

   ![](assets/choose-field-type-2-hand.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. 为字段输入[!UICONTROL Field Label]、[!UICONTROL Length]和[!UICONTROL Field Name]，如下表所示。

<table>
 <thead>
  <tr>
   <th>
    <div>
      字段标签
    </div></th>
   <th>
    <div>
      字段名称
    </div></th>
   <th>
    <div>
      数据类型
    </div></th>
   <th>
    <div>
      字段属性
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>得分</td>
   <td>mkto71_Lead_Score</td>
   <td>数值</td>
   <td>长度10<br>小数位0 </td>
  </tr>
  <tr>
   <td>获取日期</td>
   <td>mkto71_Acquisition_Date</td>
   <td>日期/时间</td>
   <td> </td>
  </tr>
  <tr>
   <td>客户获取计划</td>
   <td>mkto71_Acquisition_Program</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>[!DNL Salesforce]在创建API名称时将__c附加到字段名称。

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>文本和数字字段需要长度，但日期/时间字段不需要。说明是可选的。

1. 单击 **[!UICONTROL Next]**。

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. 指定访问设置并单击&#x200B;**[!UICONTROL Next]**：

   * 将所有角色设置为&#x200B;**[!UICONTROL Visible]**&#x200B;和&#x200B;**[!UICONTROL Read-Only]**

   * 清除同步用户配置文件的&#x200B;**[!UICONTROL Read-Only]**&#x200B;复选框：

      * 如果您的用户具有&#x200B;_系统管理员_&#x200B;的配置文件作为同步用户，请清除系统管理员配置文件的&#x200B;**[!UICONTROL Read-Only]**&#x200B;复选框（如下所示）
      * 如果您为同步用户创建了&#x200B;_自定义配置文件_，请清除该自定义配置文件的&#x200B;**[!UICONTROL Read-Only]**&#x200B;复选框

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. 选择应显示该字段的页面布局。

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. 单击&#x200B;**[!UICONTROL Save & New]**&#x200B;返回并创建其他两个自定义字段。 完成全部三个操作后，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. 在左侧的“生成”菜单中，单击&#x200B;**[!UICONTROL Customize]**&#x200B;并选择“联系人”。 单击 [!UICONTROL Fields]。
1. 对联系对象的“得分”、“客户获取日期”和“客户获取计划”字段执行步骤3至10，就像对潜在客户对象执行操作一样。
1. 或者，将上述过程用于此表的任何其他自定义字段。

<table>
 <thead>
  <tr>
   <th>
    <div>
      字段标签
    </div></th>
   <th>
    <div>
      字段名称
    </div></th>
   <th>
    <div>
      数据类型
    </div></th>
   <th>
    <div>
      字段属性
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>客户获取计划ID</td>
   <td>mkto71_Acquisition_Program_Id</td>
   <td>数值</td>
   <td>长度18<br>小数位0 </td>
  </tr>
  <tr>
   <td>原始反向链接</td>
   <td>mkto71_Original_Referrer</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>原始搜索引擎</td>
   <td>mkto71_Original_Search_Engine</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>原始搜索短语</td>
   <td>mkto71_Original_Search_Phrase</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>原始来源信息</td>
   <td>mkto71_Original_Source_Info</td>
   <td>文本</td>
   <td>长255</td>
  </tr>
  <tr>
   <td>原始来源类型</td>
   <td>mkto71_Original_Source_Type</td>
   <td>文本</td>
   <td>长255</td>
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
>创建新字段后，Marketo自动分配的字段中的值将不能立即在[!DNL Salesforce]中使用。 下次更新任一系统上的记录时(即更新Marketo与[!DNL Salesforce]之间同步的任何字段)，Marketo会将数据同步到[!DNL Salesforce]。

## 映射用于转换的自定义字段 {#map-custom-fields-for-conversions}

[!DNL Salesforce]中商机对象上的自定义字段应映射到联系人对象上的联系人字段，以便在发生转化时保留数据。

1. 单击右上角的&#x200B;**[!UICONTROL Setup]**。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. 在导航搜索中键入“Fields”，而不按Enter。 字段显示在不同的对象下；单击&#x200B;**[!UICONTROL Fields]**&#x200B;下的[!UICONTROL Leads]。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. 转到[!UICONTROL Lead Custom Fields & Relationships]部分并单击&#x200B;**[!UICONTROL Map Lead Fields]**。

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. 单击要映射的字段旁边的下拉菜单。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 选择相应的联系人自定义字段。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 对创建的任何其他字段重复上述步骤。

1. 完成后，单击&#x200B;**[!UICONTROL Save]**。

   够简单了吧？

>[!MORELIKETHIS]
>
>[第2步（共3步）：为Marketo (Enterprise/Unlimited)创建 [!DNL Salesforce] 用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
