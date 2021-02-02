---
unique-page-id: 2360362
description: 步骤1（共3步）-将Marketo字段添加到Salesforce(Enterprise/Unlimited)- Marketo文档——产品文档
title: 第1步（共3步）-将Marketo字段添加到Salesforce(Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---


# 第1步，共3步：将Marketo字段添加到Salesforce(Enterprise/Unlimited){#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>您必须具有访问Salesforce API的权限，才能在Marketo和Salesforce之间同步。

Marketo使用一组字段来捕获某些类型的营销相关信息。 如果您希望在Salesforce中使用此数据，请按照以下说明操作。

1. 在潜在客户和联系人对象的Salesforce中创建三个自定义字段：得分、客户获取项目和客户获取日期。
1. 在潜在客户和联系人之间映射这些自定义字段，以便在Salesforce中转换时，这些值继续存在。
1. 如有必要，可创建其他字段（请参阅下表）。

所有这些自定义字段都是可选字段，不必同步Marketo和Salesforce。 作为最佳实践，我们建议您确实为得分、客户赢取项目和客户赢取日期创建字段。

## 将Marketo字段添加到Salesforce {#add-marketo-fields-to-salesforce}

在以上列出的Salesforce中的潜在客户和联系人对象上添加三个自定义字段。 如果要添加更多，请参阅本节末尾的可用字段表。

对三个自定义字段中的每个字段执行以下步骤以添加它们。 开始和得分。

1. 登录Salesforce并单击&#x200B;**安装**。

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 在左侧的“生成”菜单中，单击&#x200B;**自定义**&#x200B;并选择&#x200B;**潜在客户**。 单击&#x200B;**字段**。

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. 单击页面底部的“Custom Fields &amp; Relationships（自定义字段和关系）”部分中的&#x200B;**New**。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 选择相应的字段类型(对于得分——数字；获取项目—文本；获取日期——日期／时间)。

   ![](assets/choose-field-type-2-hand.png)

1. 单击&#x200B;**下一步**。

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
   <td>日期／时间</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>赢取项目</td> 
   <td>mkto71_Acquisition_项目</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当Salesforce使用字段名称创建API名称时，会将__c附加到字段名称中。

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>文本和数字字段需要长度，但日期／时间字段不需要长度。描述是可选的。

1. 单击&#x200B;**下一步**。

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. 指定访问设置，然后单击&#x200B;**Next**:

   * 将所有角色设置为&#x200B;**Visible**&#x200B;和&#x200B;**只读**

   * 清除同步用户用户档案的&#x200B;**只读**&#x200B;复选框：

      * 如果您有用户档案为&#x200B;_系统管理员_&#x200B;的用户作为同步用户，请清除“系统管理员”用户档案的&#x200B;**只读**&#x200B;复选框（如下所示）
      * 如果为同步用户创建了&#x200B;_自定义用户档案_，请清除该自定义用户档案的&#x200B;**只读**&#x200B;复选框

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. 选择应显示字段的页面布局。

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. 单击&#x200B;**保存并新建**&#x200B;以返回并创建其他两个自定义字段。 单击&#x200B;**保存**，这三个操作都已完成。

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. 在左侧的“生成”菜单中，单击&#x200B;**自定义**&#x200B;并选择“联系人”。 单击“字段”。
1. 对联系人对象上的“分数”、“客户获取日期”和“客户获取项目”字段执行步骤3到步骤10，就像对潜在客户对象执行步骤一样。
1. （可选）对此表中的任何其他自定义字段使用上述过程。

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
   <td>客户获取项目ID</td> 
   <td>mkto71_Acquisition_项目_Id</td> 
   <td>数字</td> 
   <td>长度18<br>小数位0 </td> 
  </tr> 
  <tr> 
   <td>原始推荐人</td> 
   <td>mkto71_Original_推荐人</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>原始搜索引擎</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>原始搜索短语</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>原始源信息</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>原始源类型</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>推断城市</td> 
   <td>mkto71_Intermied_City</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>推断公司</td> 
   <td>mkto71_Intermited_公司</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>推断国家</td> 
   <td>mkto71_Intercreted_Country</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>推断的都市区</td> 
   <td>mkto71_Intercreted_Metropolitan_Area</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>推断电话区号</td> 
   <td>mkto71_Intermited_Phone_Area_Code</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>推断的邮政编码</td> 
   <td>mkto71_Intermited_Postal_Code</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
  <tr> 
   <td>推断的州区</td> 
   <td>mkto71_Intercreted_State_Region</td> 
   <td>文本</td> 
   <td>长度255</td> 
  </tr> 
 </tbody> 
</table>

## 映射转换的自定义字段{#map-custom-fields-for-conversions}

Salesforce中潜在客户对象上的自定义字段应映射到联系人对象上的联系人字段，以便在发生转换时传递数据。

1. 在右上角，单击&#x200B;**Setup**。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. 在Nav Search中键入“Fields”，无需按Enter。 字段显示在不同对象下；单击“Lead”下的&#x200B;**字段**。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. 转至“潜在客户自定义字段和关系”部分，然后单击&#x200B;**映射潜在客户字段**。

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. 单击要映射的字段旁边的下拉框。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 选择相应的联系人自定义字段。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 对于您创建的任何其他字段，重复上述步骤。

1. 完成后，单击&#x200B;**保存**。

   够轻松了，对吧？

>[!NOTE]
>
>这是指向整个过程](https://nation.marketo.com/videos/1475)的[视频的链接，它应该清晰可见！

>[!MORELIKETHIS]
>
>[第2步，共3步：为Marketo创建Salesforce用户(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
