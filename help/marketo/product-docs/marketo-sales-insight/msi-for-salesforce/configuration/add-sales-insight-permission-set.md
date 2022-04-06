---
description: 添加销售分析权限集 — Marketo文档 — 产品文档
title: 添加Sales Insight权限集
hide: true
hidefromtoc: true
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 添加Sales Insight权限集 {#add-sales-insight-permission-set}

请按照以下步骤在Salesforce中添加对Sales Insight功能的访问权限。 适用于Salesforce Classic和Layting

>[!PREREQUISITES]
>
>[更新Sales Insight Salesforce包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}到版本1.8000或更高版本，以使用此功能。

>[!IMPORTANT]
>
>如果您之前已为所有用户授予Sales Insight访问所有配置文件的权限和/或实施了Sales Insight，则您必须 [删除配置文件级别访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;}使用此权限集。

## 概述 {#overview}

“Marketo应用程序”权限是Sales Insight Salesforce包的一部分。 它包括对以下所述对象、顶点类和可视化强制页面的访问。 访问所有Sales Insight功能时都需要这些功能。

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

## 向用户添加Marketo应用程序权限集 {#adding-marketo-app-permission-set-to-users}

1. 登录到您的Salesforce帐户。

PICC

1. 单击 **设置**.

PICC

1. 在管理员下，单击以展开 **管理用户**，则 **用户**.

PICC

1. 在所有用户下，选择要提供访问权限的用户，然后单击 **权限集分配**.

PICC

1. 单击 **编辑分配**.

PICC

1. 选择 **Marketo应用程序访问** ，然后 **添加**. 单击 **保存**.

PICC

1. 现在，当您向下滚动“用户详细信息”页面时，您将在“权限集分配”下看到“Marketo应用程序访问”。

PICC

>[!NOTE]
>
>无权访问Sales Insight的用户将看到以下消息：“您没有足够的权限访问此选项卡。”

就这样！ 您已成功添加“销售分析”访问权限。 对要添加访问权限的任何其他用户档案重复相同步骤。
