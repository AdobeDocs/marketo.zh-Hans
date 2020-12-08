---
unique-page-id: 14745823
description: 在Salesforce中创建工作流规则- Marketo Docs —— 产品文档
title: 在Salesforce中创建工作流规则
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# 在Salesforce中创建工作流规则 {#creating-workflow-rules-in-salesforce}

在并行使用Marketo Sales Insight(MSI)和Marketo Sales Connect(MSC)时，Salesforce中的MSI最佳押注功能将不会更新。 所有其他MSI功能均正常工作(查看iFrame中有趣的时刻、发送电子邮件、向活动添加内容等)。 本文优惠了使“最佳下注”再次工作的补救方法。

>[!NOTE]
>
>这只会影响同时使用 **MSI** 和MSE以及希望使用MSI最佳押注功能的客户。 如果您不需要／使用“最佳赌注”，您可以忽略。

## 入门 {#getting-started}

解决方法包括创建新的工作流规则，将新MSE字段的值复制到旧MSI字段。 您需要为联系人对象创建四个工作流规则，并为自己的Salesforce实例中的潜在客户对象创建相同的四个工作流规则。 这可能要求您具有CRM管理权限（取决于您在CRM中的角色和设置）。

下面是工作流规则的建议名称和每个规则的说明。 这些属性适用于联系人和潜在客户对象：

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>更新有趣的矩设计字段</td> 
   <td><p>复制自：上次营销人员参<br>与DescCopy:《最后有趣的时刻》</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的矩类型字段</td> 
   <td><p>复制自：上次营销人员参<br>与类型复制到：最后有趣的时刻类型</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的时刻源字段</td> 
   <td><p>复制自：上次Marketo Engagement<br>SourceCopy到：最后有趣的时刻源</p></td> 
  </tr> 
  <tr> 
   <td>更新“感兴趣的时刻日期”字段</td> 
   <td><p>复制自：上次营销人员参<br>与日期复制到：最后一个有趣的时刻日期</p></td> 
  </tr> 
 </tbody> 
</table>

## 说明 {#instructions}

1. 单击“设 **置**”后，搜索“工 **作流** ”并选 **择“工作流规则**”。

   ![](assets/one-1.png)

1. 选择 **新规则**。

   ![](assets/two-1.png)

1. 单击对象下拉框，选择潜 **在客**&#x200B;户，然后单击 **下一步**。

   ![](assets/three-1.png)

1. 输入“更新有趣的时刻设计字段”作为规则名称。 选择创建的单 **选按钮，并在每次编辑该按钮**。 在“规则条件”(Rule Criteria)下拉框中，选择 **公式的计算结果为true**。 搜索并选择ISCHANGED函数。 然后，高亮显示默认字段值，并单击“ **插入字段”**。

   ![](assets/four-1.png)

1. 在“插入字段”弹出窗口中，选择“上次 **市场营销参与设计”** ，然后单 **击“插入**”。

   ![](assets/five-1.png)

1. 单击“ **保存并下一步**”。

   ![](assets/6.png)

1. 在添加工作流操作下拉框中，选择新 **建字段更新**。

   ![](assets/seven.png)

1. 在“名称”字段中，输入“更新有趣的时刻设计字段”（唯一名称将自动生成）。 在“要更新的字段”下拉框中，选择“最 **后感兴趣的时刻设计**”。 选择使 **用公式设置新值单选按钮** ，然后单击显示 **公式编辑器**。

   ![](assets/eight.png)

1. 单击“插 **入字段** ”按钮。

   ![](assets/9a.png)

1. 选择“ **上次营销人员**”，然后单 **击“插入**”。 在下一页，单击“保 **存**”。

   ![](assets/nine.png)

1. 单击 **完成**。

   ![](assets/twelve.png)

1. 单击 **激活** ，以打开工作流规则。

   ![](assets/thirteen.png)

   在上一步之后，您可以选择克隆“入门”部分中列出的其他字段的工作流规则：Desc、Type、Source、Date。 在“联系人”对象中完成四个工作流规则后，对“潜在客户”对象重复相同的规则。

