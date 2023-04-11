---
unique-page-id: 11372975
description: 步骤1（共3步） — 将Marketo字段添加到Salesforce（专业版） — Marketo文档 — 产品文档
title: 步骤1（共3步） — 将Marketo字段添加到Salesforce（专业）
exl-id: 1b52825e-201d-4b55-8edf-444b1653d591
source-git-commit: e84b8e03ce87f8aa0f16d2b0f22ee992e4151a55
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 步骤1（共3步）：将Marketo字段添加到Salesforce（专业版） {#step-of-add-marketo-fields-to-salesforce-professional}

>[!PREREQUISITES]
>
>您的Salesforce实例必须有权访问Salesforce API，才能在Marketo和Salesforce之间同步数据。

Marketo使用一组字段来捕获某些类型的营销相关信息。 如果要在Salesforce中获取此数据，请按照以下说明操作。

1. 在潜在客户和联系人对象的Salesforce中创建三个自定义字段：得分、客户获取计划和客户获取日期。
1. 在潜在客户和联系人之间映射这些自定义字段，以便在Salesforce中进行转换时，这些值会继续存在。
1. 如有必要，您可以创建其他字段（请参阅下表）。

所有这些自定义字段都是可选字段，并且不是同步Marketo和Salesforce所必需的字段。 作为最佳实践，我们建议您确实为分数、客户获取计划和客户获取日期创建字段。

## 将Marketo字段添加到Salesforce {#add-marketo-fields-to-salesforce}

在上面列出的Salesforce中的潜在客户和联系人对象上添加三个自定义字段。 如果要添加更多，请参阅此部分末尾的可用字段表。

对三个自定义字段中的每个字段执行以下步骤以添加它们。 开始于 **得分**.

1. 登录Salesforce并单击 **设置。**

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 在左侧的“构建”菜单中，单击 **自定义** 选择 **潜在客户**. 单击 **字段**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. 单击 **新建** 在页面底部的自定义字段和关系部分中。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 选择相应的字段类型(对于“得分 —  **数字**;收购计划 —  **文本**;收购日期 —  **日期/时间**)。

   ![](assets/choose-field-type-2-hand.png)

1. 单击 **下一个**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. 输入字段的字段标签、长度和字段名称，如下表所示。

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
   <td>数字</td> 
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
>Salesforce在使用字段名称创建API名称时，会将__c附加到字段名称。

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>文本和数字字段需要长度，但日期/时间字段没有。描述是可选的。

1. 单击 **下一个**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. 指定访问设置并单击 **下一个**:

   * 将所有角色设置为 **可见** 和 **只读**

   * 清除 **只读** 复选框，用于显示同步用户的配置文件：

      * 如果您的用户的配置文件为 _系统管理员_ 作为同步用户，清除 **只读** 复选框（如下所示）

      * 如果您创建了 _自定义用户档案_ 对于同步用户，请清除 **只读** 该自定义用户档案的复选框

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. 选择应显示字段的页面布局。

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. 单击 **保存并新建** 返回并创建其他两个自定义字段。 单击 **保存** 你三个都完蛋了。

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. 在左侧的“构建”菜单中，单击 **自定义** 选择 **联系人**. 单击 **字段**.
1. 对联系对象上的“分数”、“客户获取日期”和“客户获取程序”字段执行步骤3至10，就像您对潜在客户对象执行的操作一样。
1. （可选）对此表中的任何其他自定义字段使用上述过程。

<table> 
 <tbody> 
  <tr> 
   <th>字段标签</th> 
   <th>字段名称</th> 
   <th>数据类型</th> 
   <th>字段属性</th> 
  </tr> 
  <tr> 
   <td>客户获取计划ID</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>数字</td> 
   <td>长18<br>小数位0 </td> 
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
   <td>原始源信息</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>原始源类型</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>推断的城市</td> 
   <td>mkto71_Intermited_City</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>推断公司</td> 
   <td>mkto71_Intermited_Company</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>推断的国家</td> 
   <td>mkto71_Intercuted_Country</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>推断的都市区</td> 
   <td>mkto71_Intercuted_Metropolitan_Area</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>推断的电话区号</td> 
   <td>mkto71_Intermited_Phone_Area_Code</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>推断的邮政编码</td> 
   <td>mkto71_Intermited_Postal_Code</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
  <tr> 
   <td>推断的状态区域</td> 
   <td>mkto71_Intercuted_State_Region</td> 
   <td>文本</td> 
   <td>长255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>创建新字段后，由Marketo自动分配的字段中的值不会立即在Salesforce中可用。 Marketo将在下次更新到任一系统上的记录时(即，对Marketo和Salesforce之间同步的任何字段进行更新)，将数据同步到Salesforce。

## 映射自定义字段以进行转化  {#map-custom-fields-for-conversions}

Salesforce中潜在客户对象上的自定义字段应映射到联系人对象上的联系人字段，以便在发生转化时传递数据。

1. 单击右上角的“设置”。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. 在导航搜索中键入“字段”，而不按Enter。 字段显示在不同对象下；单击潜在客户下的字段。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. 转到潜在客户自定义字段和关系部分，然后单击映射潜在客户字段。

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. 单击要映射的字段旁边的下拉菜单。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 选择相应的联系人自定义字段。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 对您创建的任何其他字段重复上述步骤。

1. 完成后，单击保存。

够轻松的吧？

>[!MORELIKETHIS]
>
>[步骤2（共3步）：为Marketo创建Salesforce用户（专业版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)
