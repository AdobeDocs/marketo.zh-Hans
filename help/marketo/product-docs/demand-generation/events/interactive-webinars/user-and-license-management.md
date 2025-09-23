---
description: 用户和许可证管理 — Marketo文档 — 产品文档
title: 用户与许可证管理
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 2%

---

# 用户与许可证管理 {#user-and-license-management}

了解如何添加和删除用户以及查看当前许可证。

## 添加用户 {#add-a-user}

1. 转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/user-and-license-management-1.png)

1. 单击&#x200B;**交互式网络研讨会**。

   ![](assets/user-and-license-management-2.png)

1. 单击&#x200B;**添加/删除用户**。

   ![](assets/user-and-license-management-3.png)

1. 单击“可用用户”下拉列表，选择要添加的用户，然后单击“**确定**”。

   ![](assets/user-and-license-management-4.png)

## 删除用户 {#remove-a-user}

1. 转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/user-and-license-management-5.png)

1. 单击&#x200B;**交互式网络研讨会**。

   ![](assets/user-and-license-management-6.png)

1. 单击&#x200B;**添加/删除用户**。

   ![](assets/user-and-license-management-7.png)

1. 突出显示要删除的用户，然后按键盘上的Delete键。 完成后单击&#x200B;**确定**。

   ![](assets/user-and-license-management-8.png)

## 许可证使用情况 {#license-usage}

交互式网络研讨会提供了用于创建由Adobe Connect提供支持的活动的特定许可证。 每次添加许可证时，都会显示一个新的许可证使用框。 Marketo管理员可以按照以下步骤查看（而不是编辑）许可证。 联系Adobe客户团队（您的客户经理）以获取其他许可证。

1. 转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/user-and-license-management-9.png)

1. 单击&#x200B;**交互式网络研讨会**。

   ![](assets/user-and-license-management-10.png)

1. 向下滚动到“许可证使用”卡。

   ![](assets/user-and-license-management-11.png)

<table>
  <tr>
   <td width="20%"><b>开始日期</b></td>
   <td width="80%">许可证开始日期。</td>
  </tr>
  <tr>
   <td width="20%"><b>到期日期</b></td>
   <td width="80%">许可证到期日期。</td>
  </tr>
  <tr>
   <td width="20%"><b>类型</b></td>
   <td width="80%">购买的许可证类型。 有三种可用类型：共享事件许可证、共享房间许可证、附加存储许可证。</td>
  </tr>
  <tr>
   <td width="20%"><b>事件容量</b></td>
   <td width="80%">事件中可容纳的最大参与者数。</td>
  </tr>
  <tr>
   <td width="20%"><b>事件总数</b></td>
   <td width="80%">已使用此许可证配置的事件总数。</td>
  </tr>
  <tr>
   <td width="20%"><b>使用的事件</b></td>
   <td width="80%">所有已完成和当前计划的事件。 <a href="#things-to-note">了解详情</a></td>
  </tr>
  <tr>
   <td width="20%"><b>存储容量</b></td>
   <td width="80%">可用于存储录制、抵押品、主页图像、文档和其他资源的存储量。</td>
  </tr>
  </tbody>
</table>

### 注意事项 {#things-to-note}

* 每次创建事件时，它都会从相应的许可证中计为“已使用”（除非它是共享房间许可证）。 如果同时有“共享事件许可证”和“共享房间许可证”的容量相同，则优先选择“共享事件许可证”。 如果事件尚未传递，且在计划时间之前删除了事件程序，则会补充事件计数。 如果未交付该事件，并且在计划时间之前未删除事件程序，则不会补充该事件。

* 类型“额外存储许可证”仅提供存储，因此&#x200B;_存储容量之外的每个字段_&#x200B;中的值将仅列为“ — ”。

* “共享房间许可证”类型有无限数量的事件，“其他存储许可证”仅提供存储，因此这些许可证的“事件总数”字段将简单列为“ — ”。

* 许可证用完后，其图块会保留在“管理员”部分的“交互式网络研讨会”屏幕上，“总事件”和“消费的事件”具有相同的值。 只有当许可证过期时，才会将其从屏幕中删除。

## 用户访问 {#user-access}

交互式网络研讨会具有管理使用情况的功能，其方法是向Marketo Engage用户授予创建和提供交互式网络研讨会的权限。 但是，交互式网络研讨会用户（或非用户）仍然可以读取/编辑其他用户创建的交互式网络研讨会事件程序。

具有交互式网络研讨会权限并且拥有特定交互式网络研讨会活动计划的Marketo用户将能够执行与该计划相关的所有交互式网络研讨会功能。 这包括：创建、访问、修改、克隆、移动和删除该程序。 但是，一旦该用户不再是交互式网络研讨会用户，项目的所有者将能够访问和移动项目，但不能执行任何其他功能。

已获得交互式网络研讨会权限并且不是特定交互式网络研讨会活动计划的&#x200B;_所有者_&#x200B;的Marketo用户将能够在这些计划上执行有限的功能。 Marketo的非管理员用户将能够访问和克隆程序，但如果他们具有交互式网络研讨会的权限，则将无法执行任何其他功能。 但是，Marketo管理员用户&#x200B;_将_&#x200B;能够执行所有功能，例如访问、修改、克隆、移动和删除该程序（只要他们有权参加交互式网络研讨会）。 在撤销对Marketo管理员和非管理员用户的此权限后，他们将只能访问交互式网络研讨会事件计划，而不能执行任何其他功能。

可操作函数的限制将通过灰显的操作按钮和悬停消息指示。 以“设计您的网络研讨会”或“输入您的网络研讨会”为例，此类操作按钮呈灰显状态。 对于不可操作的功能，将提供一条强调限制的消息。 请参阅以下示例：

![](assets/user-and-license-management-12.png)
