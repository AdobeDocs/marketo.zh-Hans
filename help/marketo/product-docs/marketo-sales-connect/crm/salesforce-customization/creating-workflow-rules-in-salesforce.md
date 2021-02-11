---
unique-page-id: 14745823
description: 在Salesforce中创建工作流规则- Marketo Docs —— 产品文档
title: 在Salesforce中创建工作流规则
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# 在Salesforce{#creating-workflow-rules-in-salesforce}中创建工作流规则

在并行使用Marketo Sales Insight(MSI)和Marketo Sales Connect(MSC)时，Salesforce中的MSI最佳押注功能将不会更新。 所有其他MSI功能均正常工作(查看iFrame中有趣的时刻、发送电子邮件、向活动添加内容等)。 本文优惠了使“最佳下注”再次工作的补救方法。

>[!NOTE]
>
>这仅会影响同时使用&#x200B;**** MSI和MSE以及希望使用MSI最佳押注功能的客户。 如果您不需要／使用“最佳赌注”，您可以忽略。

## 入门{#getting-started}

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
   <td><p>复制自：上次营销人员参与Desc<br>复制到：《最后有趣的时刻》</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的矩类型字段</td> 
   <td><p>复制自：上次营销人员参与类型<br>复制到：最后有趣的时刻类型</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的时刻源字段</td> 
   <td><p>复制自：上次营销人员参与源<br>复制到：最后有趣的时刻源</p></td> 
  </tr> 
  <tr> 
   <td>更新“感兴趣的时刻日期”字段</td> 
   <td><p>复制自：上次市场营销人员参与日期<br>复制到：最后一个有趣的时刻日期</p></td> 
  </tr> 
 </tbody> 
</table>

## 说明{#instructions}

1. 单击&#x200B;**设置**&#x200B;后，搜索&#x200B;**工作流**&#x200B;并选择&#x200B;**工作流规则**。

   ![](assets/one-1.png)

1. 选择&#x200B;**新建规则**。

   ![](assets/two-1.png)

1. 单击“对象”下拉框，选择&#x200B;**潜在客户**，然后单击&#x200B;**下一步**。

   ![](assets/three-1.png)

1. 输入“更新有趣的时刻设计字段”作为规则名称。 选择已创建的单选按钮&#x200B;**，并且每次编辑**。 在“规则条件”下拉框中，选择&#x200B;**公式的计算结果为true**。 搜索并选择ISCHANGED函数。 然后，高亮显示默认字段值，并单击&#x200B;**插入字段**。

   ![](assets/four-1.png)

1. 在“插入字段”弹出窗口中，选择&#x200B;**上次市场营销参与说明**&#x200B;并单击&#x200B;**插入**。

   ![](assets/five-1.png)

1. 单击&#x200B;**保存并下一步**。

   ![](assets/6.png)

1. 在添加工作流操作下拉框中，选择&#x200B;**新建字段更新**。

   ![](assets/seven.png)

1. 在“名称”字段中，输入“更新有趣的时刻设计字段”（唯一名称将自动生成）。 在“要更新的字段”下拉框中，选择&#x200B;**最后一个有趣的时刻Desc**。 选择&#x200B;**使用公式设置新值**&#x200B;单选按钮，然后单击&#x200B;**显示公式编辑器**。

   ![](assets/eight.png)

1. 单击&#x200B;**插入字段**&#x200B;按钮。

   ![](assets/9a.png)

1. 选择&#x200B;**上次营销活动设计**，然后单击&#x200B;**插入**。 在下一页，单击&#x200B;**保存**。

   ![](assets/nine.png)

1. 单击&#x200B;**完成**。

   ![](assets/twelve.png)

1. 单击&#x200B;**激活**&#x200B;以打开工作流规则。

   ![](assets/thirteen.png)

   在上一步之后，您可以选择克隆“入门”部分中列出的其他字段的工作流规则：Desc、Type、Source、Date。 在“联系人”对象中完成四个工作流规则后，对“潜在客户”对象重复相同的规则。
