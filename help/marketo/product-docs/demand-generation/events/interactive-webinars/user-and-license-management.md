---
description: 用户和许可证管理 — Marketo文档 — 产品文档
title: 用户和许可证管理
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# 用户和许可证管理 {#user-and-license-management}

了解如何添加和删除用户以及查看当前许可证。

## 添加用户 {#add-a-user}

1. 转到 **管理员** 区域。

   ![](assets/user-and-license-management-1.png)

1. 单击 **交互式网络研讨会**.

   ![](assets/user-and-license-management-2.png)

1. 单击 **添加/删除用户**.

   ![](assets/user-and-license-management-3.png)

1. 单击可用用户下拉列表，选择要添加的用户，然后单击 **确定**.

   ![](assets/user-and-license-management-4.png)

## 删除用户 {#remove-a-user}

1. 转到 **管理员** 区域。

   ![](assets/user-and-license-management-5.png)

1. 单击 **交互式网络研讨会**.

   ![](assets/user-and-license-management-6.png)

1. 单击 **添加/删除用户**.

   ![](assets/user-and-license-management-7.png)

1. 突出显示要删除的用户，然后按键盘上的Delete键。 单击 **确定** 完成时。

   ![](assets/user-and-license-management-8.png)

## 许可证使用情况 {#license-usage}

交互式网络研讨会提供了用于创建由Adobe Connect提供支持的活动的特定许可证。 每次添加许可证时，都会显示一个新的许可证使用框。 Marketo管理员可以按照以下步骤查看（而不是编辑）许可证。 联系Adobe客户团队（您的客户经理）以获取其他许可证。

1. 转到 **管理员** 区域。

   ![](assets/user-and-license-management-9.png)

1. 单击 **交互式网络研讨会**.

   ![](assets/user-and-license-management-10.png)

1. 向下滚动到“许可证使用”卡。

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>开始日期</b></td>
   <td>许可证开始日期。</td>
  </tr>
  <tr> 
   <td><b>到期日期</b></td>
   <td>许可证到期日期。</td>
  </tr>
  <tr> 
   <td><b>类型</b></td>
   <td>购买的许可证类型。 有三种可用类型：共享事件许可证、共享房间许可证、附加存储许可证。</td>
  </tr>
  <tr> 
   <td><b>事件容量</b></td>
   <td>事件中可容纳的最大参与者数。</td>
  </tr>
  <tr> 
   <td><b>事件总数</b></td>
   <td>已使用此许可证配置的事件总数。</td>
  </tr>
  <tr> 
   <td><b>使用的事件</b></td>
   <td>已完成事件的总数。</td>
  </tr>
  <tr> 
   <td><b>存储容量</b></td>
   <td>可用于存储记录、抵押品、hero images、文档和其他资源的存储量。</td>
  </tr>
  </tbody>
</table>

**注意事项**

* “Additional Storage License”类型仅提供存储，因此每个字段中的值都相同 _此外_ 存储容量将仅以“ — ”形式列出。

* “共享房间许可证”类型有无限数量的事件，“其他存储许可证”仅提供存储，因此这些许可证的“事件总数”字段将简单列为“ — ”。

* 每次创建事件时，它都会从相应的许可证中计为“已使用”（除非它是共享房间许可证）。 如果同时有“共享事件许可证”和“共享房间许可证”的容量相同，则将优先选择“共享事件许可证”。 如果事件尚未交付，并且在计划时间之前删除了事件程序，则通过从使用的事件中减去一个事件来补充事件计数。

* 许可证用完后，其图块会保留在“管理员”部分的“交互式网络研讨会”屏幕上，“总事件”和“消费的事件”具有相同的值。 只有当许可证过期时，才会将其从屏幕中删除。
