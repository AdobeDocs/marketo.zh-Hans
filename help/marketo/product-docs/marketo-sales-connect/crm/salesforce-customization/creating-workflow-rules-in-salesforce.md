---
unique-page-id: 14745823
description: 在Salesforce中创建工作流规则 — Marketo文档 — 产品文档
title: 在Salesforce中创建工作流规则
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# 在Salesforce中创建工作流规则 {#creating-workflow-rules-in-salesforce}

在并行使用Marketo Sales Insight (MSI)和Marketo Sales Connect (MSC)时，Salesforce中的MSI最佳匹配功能不会更新。 所有其他MSI功能均可正常使用（查看iFrame中的有趣时刻、发送电子邮件、添加到营销活动等）。 本文提供了使Best Bets再次正常工作的解决方法。

>[!NOTE]
>
>这仅会影响同时使用&#x200B;**1} MSI和MSE以及希望在MSI中使用最佳匹配功能的客户。**&#x200B;如果您不需要/使用“最佳匹配”，则可以忽略。

## 快速入门 {#getting-started}

解决方法包括创建新工作流规则，以将新MSE字段中的值复制到旧MSI字段中。 您需要为联系人对象创建四个工作流规则，并在自己的Salesforce实例中为潜在客户对象创建相同的四个工作流规则。 这可能会要求您拥有CRM管理员权限（具体取决于您在CRM中的角色和设置）。

以下是工作流规则的建议名称和说明。 这些选项适用于Contact和Lead对象：

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>更新有趣时刻描述字段</td> 
   <td><p>复制自：上次Marketo参与度描述<br>复制至：上次有趣时刻描述</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣时刻类型字段</td> 
   <td><p>复制自：上次Marketo参与类型<br>复制至：上一个有趣的时刻类型</p></td> 
  </tr> 
  <tr> 
   <td>更新“有趣的时刻”Source字段</td> 
   <td><p>复制自：上次Marketo参与Source<br>复制至：上一个有趣的时刻Source</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣时刻日期字段</td> 
   <td><p>复制自：上次Marketo参与日期<br>复制至：上一个有趣的时刻日期</p></td> 
  </tr> 
 </tbody> 
</table>

## 说明 {#instructions}

1. 单击&#x200B;**设置**&#x200B;后，搜索&#x200B;**工作流**&#x200B;并选择&#x200B;**工作流规则**。

   ![](assets/one-1.png)

1. 选择&#x200B;**新规则**。

   ![](assets/two-1.png)

1. 单击“对象”下拉列表并选择&#x200B;**潜在客户**，然后单击&#x200B;**下一步**。

   ![](assets/three-1.png)

1. 输入“更新有趣的时间描述字段”作为规则名称。 选择单选按钮&#x200B;**已创建，并且每次都编辑**。 在“规则条件”下拉列表中选择&#x200B;**公式计算结果为true**。 搜索并选择ISCHANGED函数。 然后，突出显示默认字段值并单击&#x200B;**插入字段**。

   ![](assets/four-1.png)

1. 在“插入字段”弹出窗口中，选择&#x200B;**最后一个Marketo参与描述**，然后单击&#x200B;**插入**。

   ![](assets/five-1.png)

1. 单击&#x200B;**保存和下一步**。

   ![](assets/6.png)

1. 在添加工作流操作下拉列表中，选择&#x200B;**新字段更新**。

   ![](assets/seven.png)

1. 在名称字段中，输入“更新有趣时刻描述字段”（唯一名称将自动生成）。 在“要更新的字段”下拉列表中，选择&#x200B;**上一个有趣时刻描述**。 选择&#x200B;**使用公式设置新值**&#x200B;单选按钮，然后单击&#x200B;**显示公式编辑器**。

   ![](assets/eight.png)

1. 单击&#x200B;**插入字段**&#x200B;按钮。

   ![](assets/9a.png)

1. 选择&#x200B;**最后一个Marketo参与描述**，然后单击&#x200B;**插入**。 在下一页，单击&#x200B;**保存**。

   ![](assets/nine.png)

1. 单击&#x200B;**完成**。

   ![](assets/twelve.png)

1. 单击&#x200B;**激活**&#x200B;以打开工作流规则。

   ![](assets/thirteen.png)

   在上一步之后，您可以选择为快速入门部分列出的其他字段克隆工作流规则：说明、类型、Source、日期。 完成Contact对象中的四个工作流规则后，对Lead对象重复相同的操作。
