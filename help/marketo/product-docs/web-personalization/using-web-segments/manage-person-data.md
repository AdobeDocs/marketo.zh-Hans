---
unique-page-id: 7504051
description: 管理人员数据 — Marketo文档 — 产品文档
title: 管理人员数据
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 7%

---

# 管理人员数据 {#manage-person-data}

通过选择要在分段中使用的人员字段，利用人员数据进行Web个性化。

1. 转到 **帐户设置**.

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. 转到 **数据库**.

   ![](assets/account-settings-dropdown-database.jpg)

## 添加新人员字段 {#adding-a-new-person-field}

1. 选择 **要添加的字段** 从下拉列表中添加人员数据字段。

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >新字段会以待处理状态添加，激活过程最长可能需要24小时。

## 删除人员字段 {#deleting-a-person-field}

1. 单击删除图标( ![—](assets/image2015-3-24-13-3a45-3a56.png))，以从列表中删除字段。 单击 **是** 以确认您要删除该字段。

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**管理人员数据字段**
   >
   >* 只能包含人员数据字段
   >* 您最多可以添加30个人数据字段
   >* 添加新字段最多需要24小时才能激活
   >* 字符串类型的最大长度为255个字符
   >* 隐藏字段将自动删除

<table> 
 <tbody> 
  <tr> 
   <th><p>REST API名称</p></th> 
   <th><p>SOAP API名称</p></th> 
   <th><p>友好名称</p></th> 
  </tr> 
  <tr> 
   <td><p>部门</p></td> 
   <td><p>部门</p></td> 
   <td><p>部门</p></td> 
  </tr> 
  <tr> 
   <td><p>标题</p></td> 
   <td><p>标题</p></td> 
   <td><p>职务</p></td> 
  </tr> 
  <tr> 
   <td><p>评级</p></td> 
   <td><p>评级</p></td> 
   <td><p>评级</p></td> 
  </tr> 
  <tr> 
   <td><p>商机得分</p></td> 
   <td><p>商机得分</p></td> 
   <td><p>得分</p></td> 
  </tr> 
  <tr> 
   <td><p>商机状态</p></td> 
   <td><p>潜在客户状态</p></td> 
   <td><p>状态</p></td> 
  </tr> 
  <tr> 
   <td><p>优先级</p></td> 
   <td><p>优先级</p></td> 
   <td><p>优先级</p></td> 
  </tr> 
  <tr> 
   <td><p>leadRole</p></td> 
   <td><p>潜在客户角色</p></td> 
   <td><p>职位</p></td> 
  </tr> 
  <tr> 
   <td><p>已取消订阅</p></td> 
   <td><p>退订</p></td> 
   <td><p>退订</p></td> 
  </tr> 
 </tbody> 
</table>

为新的Web个性化帐户提供的现成可用商机字段如下：

>[!MORELIKETHIS]
>
>[使用已知人员数据创建区段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
