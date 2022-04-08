---
description: 删除销售分析访问 — Marketo文档 — 产品文档
title: 删除销售分析访问权限
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# 删除销售分析访问权限 {#remove-sales-insight-access}

请按照以下步骤删除对Salesforce中Sales Insight功能的访问权限。 适用于Salesforce Classic和Lightning。

## 概述 {#overview}

要访问所有Sales Insight功能，需要具有对以下对象、顶级类和可视化强制页面的权限。 删除这些项将删除对Sales Insight的访问权限。

**对象设置**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>最佳视图详细信息</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>最佳视图</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>InterestedMomentsCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>Marketo Sales Insight配置</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>值</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
 </tbody> 
</table>

* Apex类访问：159个与“mkto_si”一起的Apex类
* 可视化强制页面访问：64可视化强制包含“mkto_si”的页面
* 自定义设置定义：mkto_si.Marketo设置和mkto_si.用户首选项

## 删除对Sales Insight的访问权限 {#removing-access-to-sales-insight}

1. 登录到您的Salesforce帐户。

1. 单击 **设置**.

   ![](assets/remove-sales-insight-access-1.png)

1. 在“Administrator（管理员）”下，单击 **管理用户**，则 **用户档案**.

1. 单击要更新的用户档案，然后 **编辑**.

1. 向下滚动到“选项卡设置”下的“自定义选项卡设置”。

1. 从下拉菜单中，为Marketo Sales Insight Config和MSI Marketo Sales Outbox选择“隐藏选项卡”选项。

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. 向下滚动到“自定义对象权限”。

1. 从以下对象中删除“读取、创建、编辑、删除”访问：

   * BestBetsCache
   * 最佳视图详细信息
   * 最佳视图
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestedMomentsCache
   * Marketo Sales Insight配置
   * ScoringCache
   * 值
   * WebActivityCache

1. 向下滚动到“已启用Apex类访问”部分。 单击 **编辑**.

1. 从“已启用的Apex类”部分中，选择以“mkto_si”开头的所有类。 这最多应该有159个类。

1. 单击 **删除**，则 **保存**.

   ![](assets/remove-sales-insight-access-4.png)

1. 向下滚动到“已启用可视化强制页面访问”部分。 单击 **编辑**.

1. 从“启用的可视化强制页面”部分中，选择以“mkto_si”开头的所有页面。 这最多可以包含64页。

1. 单击 **删除**，则 **保存**.

   ![](assets/remove-sales-insight-access-5.png)

1. 向下滚动到“启用自定义设置定义访问”部分。 单击 **编辑**.

1. 选择“Marketo Sales Insight.mkto_si.Marketo设置”和“Marketo Sales Insight.mkto_si.User Preferences”。

1. 单击 **删除**，则 **保存**.

   ![](assets/remove-sales-insight-access-6.png)

就这样！ 您已成功删除了Sales Insight访问权限。 对要删除其访问权限的任何其他配置文件重复相同步骤。
