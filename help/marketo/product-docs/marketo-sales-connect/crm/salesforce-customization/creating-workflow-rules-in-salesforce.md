---
unique-page-id: 14745823
description: 在Salesforce中创建工作流规则 — Marketo文档 — 产品文档
title: 在 Salesforce 中创建工作流规则
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 4%

---

# 在 Salesforce 中创建工作流规则 {#creating-workflow-rules-in-salesforce}

并行使用Marketo Sales Insight (MSI)和Marketo Sales Connect (MSC)时，[!DNL Salesforce]中的MSI最佳匹配功能将不会更新。 所有其他MSI功能均可正常使用（查看iFrame中的有趣时刻、发送电子邮件、添加到营销活动等）。 本文提供了使Best Bets再次正常工作的解决方法。

>[!NOTE]
>
>这仅会影响同时使用&#x200B;**1&rbrace; MSI和MSE以及希望在MSI中使用最佳匹配功能的客户。**&#x200B;如果您不需要/使用“最佳匹配”，则可以忽略。

## 快速入门 {#getting-started}

解决方法包括创建新工作流规则，以将新MSE字段中的值复制到旧MSI字段中。 您需要为联系人对象创建四个工作流规则，并为您自己的[!DNL Salesforce]实例中的潜在客户对象创建相同的四个工作流规则。 这可能会要求您拥有CRM管理员权限（具体取决于您在CRM中的角色和设置）。

以下是工作流规则的建议名称和说明。 这些参数适用于[!UICONTROL Contact]和[!UICONTROL Lead]对象：

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

1. 单击&#x200B;**[!UICONTROL Setup]**&#x200B;后，搜索&#x200B;**工作流**&#x200B;并选择&#x200B;**[!UICONTROL Workflow Rules]**。

   ![](assets/one-1.png)

1. 选择 **[!UICONTROL New Rule]**。

   ![](assets/two-1.png)

1. 单击[!UICONTROL Object]下拉菜单并选择&#x200B;**[!UICONTROL Lead]**，然后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/three-1.png)

1. 输入“更新有趣的时刻描述字段”作为[!UICONTROL Rule Name]。 选择单选按钮&#x200B;**[!UICONTROL created, and every time it’s edited]**。 在[!UICONTROL Rule Criteria]下拉列表中选择&#x200B;**[!UICONTROL formula evaluates to true]**。 搜索并选择ISCHANGED函数。 然后，突出显示默认字段值并单击&#x200B;**[!UICONTROL Insert Field]**。

   ![](assets/four-1.png)

1. 在[!UICONTROL Insert Field]弹出窗口中，选择&#x200B;**[!UICONTROL Last Marketo Engagement Desc]**&#x200B;并单击&#x200B;**[!UICONTROL Insert]**。

   ![](assets/five-1.png)

1. 单击 **[!UICONTROL Save & Next]**。

   ![](assets/6.png)

1. 在[!UICONTROL Add Workflow Action]下拉列表中，选择&#x200B;**[!UICONTROL New Field Update]**。

   ![](assets/seven.png)

1. 在[!UICONTROL Name]字段中，输入“更新有趣时刻描述字段”（[!UICONTROL Unique Name]将自动生成）。 在[!UICONTROL Field to Update]下拉列表中，选择&#x200B;**[!UICONTROL Last Interesting Moment Desc]**。 选择&#x200B;**[!UICONTROL Use a formula to set new value]**&#x200B;单选按钮，然后单击&#x200B;**[!UICONTROL Show Formula Editor]**。

   ![](assets/eight.png)

1. 单击&#x200B;**[!UICONTROL Insert Field]**&#x200B;按钮。

   ![](assets/9a.png)

1. 选择&#x200B;**[!UICONTROL Last Marketo Engagement Desc]**，然后单击&#x200B;**[!UICONTROL Insert]**。 在下一页，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/nine.png)

1. 单击 **[!UICONTROL Done]**。

   ![](assets/twelve.png)

1. 单击&#x200B;**[!UICONTROL Activate]**&#x200B;以打开工作流规则。

   ![](assets/thirteen.png)

   在上一步之后，您可以选择克隆[!UICONTROL Getting Started]部分中列出的其他字段的工作流规则： Desc、Type、Source、Date。 在[!UICONTROL Contact]对象中完成四个工作流规则后，对[!UICONTROL Lead]对象重复相同的操作。
