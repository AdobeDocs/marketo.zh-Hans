---
description: Salesforce同步状态 — Marketo文档 — 产品文档
title: Salesforce同步状态
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 2%

---

# Salesforce同步状态 {#salesforce-sync-status}

使用同步状态功能板可查看同步步骤及其成功状态中的同步状态。

同步步骤反映对象架构和数据本身按每个对象类型执行的推送或拉取操作。 统计资料涵盖同步期间的新记录、更新、删除和失败计数。 用户可以按日期、操作类型或对象类型进行过滤。 同步状态功能板显示过去五天的同步周期状态。

>[!NOTE]
>
>需要管理员权限

## 查看同步状态 {#view-sync-status}

1. 单击 **管理员**.

   ![](assets/salesforce-sync-status-1.png)

1. 在“集成”下，单击Salesforce，然后单击“同步状态”选项卡。

   ![](assets/salesforce-sync-status-2.png)

默认情况下，统计资料将按最近开始的顺序排序。 您可以通过单击排序图标，按从最近到最旧的开始时间或结束时间进行排序。

![](assets/salesforce-sync-status-3.png)

## 筛选器同步状态 {#filter-sync-status}

1. 要过滤数据，请单击页面最右侧的过滤器图标。

   ![](assets/salesforce-sync-status-4.png)

1. 选择日期和时间范围，然后单击下拉列表，以按对象类型、操作类型和/或状态类型进行筛选。

   ![](assets/salesforce-sync-status-5.png)

1. 单击 **应用**.

   ![](assets/salesforce-sync-status-6.png)

**可选步骤**:要导出同步错误，请单击 **导出**. 数据将导出为CSV格式。

![](assets/salesforce-sync-status-7.png)

## 同步状态字段 {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>字段</th> 
   <th>描述</th> 
   <th>枚举值</th> 
  </tr> 
  <tr> 
   <td colspan="1">开始于</td> 
   <td colspan="1">同步周期开始日期/时间（用户的时区）</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">结束日期</td> 
   <td colspan="1">同步周期结束日期/时间（用户的时区）</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">对象</td> 
   <td colspan="1">对象类型</td> 
   <td colspan="1">联系人、人员、任务、机会、潜在客户等，如下所示</td> 
  </tr>  
  <tr> 
   <td colspan="1">操作</td> 
   <td colspan="1">操作类型</td> 
   <td colspan="1">操作类型如下</td> 
  </tr>  
  <tr> 
   <td colspan="1">状态</td> 
   <td colspan="1">批的状态</td> 
   <td colspan="1">成功、失败、不完整、正在处理、已清理*</td> 
  </tr>
  <tr> 
   <td colspan="1">新</td> 
   <td colspan="1">新记录计数</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">已更新</td> 
   <td colspan="1">更新记录计数</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">已删除</td> 
   <td colspan="1">已删除记录的计数</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">失败的项目</td> 
   <td colspan="1">同步失败的记录数</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">已跳过</td> 
   <td colspan="1">已跳过记录计数，因为同步的目标字段没有更改</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

&#42;数据在同步步骤失败后还原为以前的完整性状态。

## 对象类型 {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">帐户</td> 
  </tr>  
  <tr> 
   <td colspan="1">帐户类型</td> 
  </tr> 
  <tr> 
   <td colspan="1">自定义对象</td> 
  </tr>  
  <tr> 
   <td colspan="1">Campaign</td> 
  </tr>  
  <tr> 
   <td colspan="1">营销活动成员状态</td> 
  </tr>
  <tr> 
   <td colspan="1">联系人</td> 
  </tr>  
  <tr> 
   <td colspan="1">电子邮件模板</td> 
  </tr>  
  <tr> 
   <td colspan="1">Event</td> 
  </tr> 
  <tr> 
   <td colspan="1">人员（潜在客户）</td> 
  </tr>  
  <tr> 
   <td colspan="1">机会</td> 
  </tr>  
  <tr> 
   <td colspan="1">机会联系角色</td> 
  </tr>  
  <tr> 
   <td colspan="1">任务</td> 
  </tr>  
  <tr> 
   <td colspan="1">用户</td> 
  </tr>  
 </tbody> 
</table>

## 操作类型 {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>操作类型</th> 
   <th>针对这些对象找到</th> 
   <th>备注</th> 
   <th>操作类型</th>
  </tr> 
  <tr> 
   <td colspan="1">Init链接与程序</td> 
   <td colspan="1">Campaign</td> 
   <td colspan="1">将营销活动关联到项目</td> 
   <td colspan="1">更新</td>
  </tr>  
  <tr> 
   <td colspan="1">提取转化</td> 
   <td colspan="1">人员（领导）*</td> 
   <td colspan="1">将转换操作从SFDC提取到Marketo。 件数（数字）是转换为联系人的潜在客户</td> 
   <td colspan="1">更新、失败项目或跳过项目</td>
  </tr> 
  <tr> 
   <td colspan="1">提取删除</td> 
   <td colspan="1">联系人、人员（潜在客户）、机会、营销活动、营销活动成员、商机联系人、自定义对象、营销活动、营销活动成员状态、商机联系人角色</td> 
   <td colspan="1">删除了正在同步到Marketo的SFDC记录</td> 
   <td colspan="1">已删除、失败的项目或已跳过的项目</td>
  </tr>  
  <tr> 
   <td colspan="1">提取更新</td> 
   <td colspan="1">任务、人员（潜在客户）、人员（潜在客户）队列、联系人、事件、机会、帐户、帐户类型、促销活动成员、自定义对象、促销活动、促销活动成员状态、事件、人员状态、机会、机会联系角色</td> 
   <td colspan="1">SFDC中的更新或新记录会同步到Marketo，将事件作为活动提取</td> 
   <td colspan="1">新建、已更新、失败的项目或已跳过的项目</td>
  </tr>  
  <tr> 
   <td colspan="1">推送新</td> 
   <td colspan="1">任务、电子邮件模板</td> 
   <td colspan="1">推送任务（活动）</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">推送更新</td> 
   <td colspan="1">任务、电子邮件模板、人员、联系人、营销活动</td> 
   <td colspan="1">将更新推送到SFDC并删除</td> 
   <td colspan="1">更新、失败项目或跳过项目</td>
  </tr>  
  <tr> 
   <td colspan="1">同步模式</td> 
   <td colspan="1">促销活动成员、自定义对象、促销活动、促销活动成员状态、任务、人员、机会、机会联系角色、用户</td> 
   <td colspan="1">同步不同对象的元数据，以决定在下一个周期中同步哪些新字段</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">与程序同步</td> 
   <td colspan="1">促销活动</td> 
   <td colspan="1">将Marketo计划与SFDC促销活动同步</td> 
   <td colspan="1">新增、更新、失败或跳过</td>
  </tr> 
  <tr> 
   <td colspan="1">更新活动</td> 
   <td colspan="1">任务</td> 
   <td colspan="1">从Salesforce提取活动</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">更新FKS</td> 
   <td colspan="1">全部</td> 
   <td colspan="1">更新所有对象的外键</td> 
   <td colspan="1">不适用</td>
  </tr>  
 </tbody> 
</table>

&#42;订阅级别的品牌配置决定了报表中的标签 — “潜在客户”或“人员”。
