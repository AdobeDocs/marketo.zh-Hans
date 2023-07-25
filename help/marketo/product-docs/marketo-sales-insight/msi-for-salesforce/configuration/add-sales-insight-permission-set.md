---
description: 添加销售分析权限集 — Marketo文档 — 产品文档
title: 添加Sales Insight权限集
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# 添加Sales Insight权限集 {#add-sales-insight-permission-set}

使用以下步骤可添加对Salesforce中Sales Insight功能的访问权限。 适用于Salesforce Classic和Lighting

>[!PREREQUISITES]
>
>[更新Sales Insight Salesforce包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} 版本1.8000或更高版本，以便使用此功能。

>[!IMPORTANT]
>
>如果您以前授予了Sales Insight对所有用户档案的访问权限和/或为所有用户实施了Sales Insight ，您必须 [删除配置文件级别访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} 以使用此权限集。

## 概述 {#overview}

“Marketo应用程序”权限是Sales Insight Salesforce包的一部分。 它包括访问以下提及的对象、顶点类和visualforce页面。 要访问所有Sales Insight功能，必须具备这些权限。

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

* Apex类访问：159个以“mkto_si”开头的类
* Visualforce页面访问：64个以“mkto_si”开头的Visualforce页面
* 自定义设置定义：mkto_si.Marketo设置和mkto_si.User首选项

## 将Marketo应用程序权限集添加到用户 {#adding-marketo-app-permission-set-to-users}

1. 登录到您的Salesforce帐户。

1. 单击 **设置**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. 在“管理员”下，单击以展开 **管理用户**，则 **用户**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. 在所有用户下，选择要提供访问权限的用户，然后单击 **权限集分配**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. 单击 **编辑分配**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. 选择 **Marketo应用程序访问权限** 从可用权限集中，然后 **添加**. 单击 **保存**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. 现在，当您向下滚动“用户详细信息”页面时，您将在“权限集分配”下看到“Marketo应用程序访问权限”。

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>无权访问Sales Insight的用户将看到以下消息：“您没有足够的权限访问此选项卡。”

就是这样！ 您已成功添加了Sales Insight访问权限。 对要为其添加访问权限的任何其他配置文件重复相同的步骤。
