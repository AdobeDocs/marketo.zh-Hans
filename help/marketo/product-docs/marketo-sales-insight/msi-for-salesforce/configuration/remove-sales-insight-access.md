---
description: 删除销售分析访问权限 — Marketo文档 — 产品文档
title: 删除销售分析访问权限
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# 删除销售分析访问权限 {#remove-sales-insight-access}

使用以下步骤可删除对Salesforce中Sales Insight功能的访问权限。 适用于Salesforce Classic和Lightning。

## 概述 {#overview}

访问所有Sales Insight功能需要下面提到的对象、 Apex类和Visualforce页面的权限。 删除这些项目将删除对Sales Insight的访问权限。

**对象设置**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>最佳匹配视图详细信息</td> 
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
   <td>InterestedMentsCache</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>Marketo销售分析配置</td> 
   <td>读取、创建、编辑、删除、查看全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>评分缓存</td> 
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

* Apex类访问：以“mkto_si”开头的159个Apex类
* Visualforce页面访问：64个以“mkto_si”开头的Visualforce页面
* 自定义设置定义：mkto_si.Marketo设置和mkto_si.User首选项

## 删除对Sales Insight的访问权限 {#removing-access-to-sales-insight}

1. 登录到您的Salesforce帐户。

1. 单击 **设置**.

   ![](assets/remove-sales-insight-access-1.png)

1. 在Administrator下，单击 **管理用户**，则 **配置文件**.

1. 单击要更新的用户档案，然后 **编辑**.

1. 向下滚动到“选项卡设置”下的“自定义选项卡设置”。

1. 从Marketo Sales Insight Config和MSI Marketo Sales Outbox的下拉列表中选择“Tab Hidden”选项。

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. 向下滚动至“自定义对象权限”。

1. 删除以下对象的“读取、创建、编辑、删除”权限：

   * BestBetsCache
   * 最佳匹配视图详细信息
   * 最佳视图
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestedMentsCache
   * Marketo销售分析配置
   * 评分缓存
   * 值
   * WebActivityCache

1. 向下滚动到“已启用Apex类访问”部分。 单击 **编辑**.

1. 从“已启用的Apex类”部分，选择以“mkto_si”开头的所有类。 这最多可添加159个类。

1. 单击 **移除**，则 **保存**.

   ![](assets/remove-sales-insight-access-4.png)

1. 向下滚动到“已启用Visualforce页面访问”部分。 单击 **编辑**.

1. 从“启用的Visualforce页面”部分，选择以“mkto_si”开头的所有页面。 最多可加64页。

1. 单击 **移除**，则 **保存**.

   ![](assets/remove-sales-insight-access-5.png)

1. 向下滚动到“启用的自定义设置定义访问权限”部分。 单击 **编辑**.

1. 选择“Marketo Sales Insight.mkto_si.Marketo设置”和“Marketo Sales Insight.mkto_si.User首选项”。

1. 单击 **移除**，则 **保存**.

   ![](assets/remove-sales-insight-access-6.png)

就是这样！ 您已成功移除销售分析访问权限。 对要删除其访问权限的任何其他配置文件重复相同的步骤。
