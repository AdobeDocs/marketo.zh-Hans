---
unique-page-id: 7504051
description: 了解如何在Marketo Engage中管理人员数据，包括管理人员数据。 使用本指南完成您的下一步。
title: 管理人员数据
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
TQID: https://experienceleague.adobe.com/rIiC-JXLkaMByk7GizVOcCEcUHN8AL-8Hy66-U2GZhs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 209
ht-degree: 12%

---

# 管理人员数据 {#manage-person-data}

通过选择要在分段中使用的人员字段来利用[!DNL Web Personalization]的人员数据。

1. 前往 **[!UICONTROL Account Settings]**。

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. 前往 **[!UICONTROL Database]**。

   ![](assets/account-settings-dropdown-database.jpg)

## 添加新人员字段 {#adding-a-new-person-field}

1. 从下拉列表中选择&#x200B;**要添加的字段**&#x200B;以将人员数据字段添加到列表。

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >新字段会以待处理状态添加，激活过程最长可能需要24小时。

## 删除人员字段 {#deleting-a-person-field}

1. 单击删除图标(![—](assets/image2015-3-24-13-3a45-3a56.png))可从列表中删除字段。 单击&#x200B;**[!UICONTROL Yes]**&#x200B;确认要删除该字段。

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**管理您的人员数据字段**
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
   <td><p>角色</p></td>
  </tr>
  <tr>
   <td><p>已取消订阅</p></td>
   <td><p>取消订阅</p></td>
   <td><p>取消订阅</p></td>
  </tr>
 </tbody>
</table>

为新[!DNL Web Personalization]帐户现成提供了以下潜在客户字段：

>[!MORELIKETHIS]
>
>[使用已知人员数据创建区段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
