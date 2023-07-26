---
unique-page-id: 12615800
description: 导入指定帐户 — Marketo文档 — 产品文档
title: 导入指定帐户
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# 导入指定帐户 {#import-named-accounts}

CSV中已经满是潜在的目标帐户吗？ 将它们直接导入TAM！

1. 单击 **新建** 下拉并选择 **导入指定帐户**.

   ![](assets/inaone.png)

1. 此时将打开一个新窗口。 单击 **浏览**，然后选择要导入的命名帐户的文件。

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >在您的文件中，提供 [尽可能多的信息](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) 尽可能。 您只能添加固件信息；Marketo不计算任何内容（如Pipeline）。 要基于CRM帐户创建命名帐户，只需将帐户名和CRM ID从CRM导出到CSV文件中，使用帐户名选项，并在导入过程中映射CRM ID即可。 要将CRM帐户正确链接到指定帐户，您必须提供CRM帐户的准确名称。

1. 从两种重复数据消除模式中选择：帐户名或域名。 在本例中，我们将选择“帐户”。 单击 **模式** 下拉并选择 **按帐户名称**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >如果您选择 **按域模式**，命名帐户和域字段都必须包含在内。

1. 要选择将指定帐户添加到哪个帐户列表，请单击 **帐户列表** 下拉菜单并进行选择。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >您还只需在下拉框中键入帐户列表的名称，即可创建全新的帐户列表。

1. 要发送导入通知，请单击 **发送警报到** 下拉列表，然后选择Marketo用户。 您 _无法_ 手动输入电子邮件地址。

   ![](assets/inafive-2.png)

1. 单击 **下一个**.

   ![](assets/inasix-2.png)

1. 通过双击 **Marketo字段** 并选择相应的字段。 单击 **下一个** 完成时。

   ![](assets/inaseven.png)

   成功!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >“检查导入状态”仅显示活动的最近三天。

按帐户名称进行重复数据删除的情况：

<table> 
 <tbody> 
  <tr> 
   <td><strong>使用现有的指定帐户名称导入记录</strong></td> 
   <td><p>我们将更新现有记录</p></td> 
  </tr> 
  <tr> 
   <td><strong>使用新的指定帐户名称导入记录</strong></td> 
   <td>我们将创建一个新记录</td> 
  </tr> 
 </tbody> 
</table>

按域名进行重复数据删除的情况：

<table> 
 <tbody> 
  <tr> 
   <td><strong>正在导入具有新帐户名和新域名的记录</strong></td> 
   <td>我们将使用提供的信息创建一个新的指定帐户</td> 
  </tr> 
  <tr> 
   <td><strong>正在导入具有现有帐户名称和现有域名的记录</strong></td> 
   <td>我们将更新现有的指定帐户</td> 
  </tr> 
   <tr> 
   <td><strong>使用新帐户名称和现有域名导入记录</strong></td> 
   <td>我们将新帐户名称附加到与域名匹配的现有指定帐户并更新其他信息（即行业、州等）</td> 
  </tr> 
  <tr> 
   <td><strong>正在导入具有现有命名帐户名称和新域名的记录</strong></td> 
   <td>我们会将新域名附加到现有的指定帐户中，使其与帐户名称匹配并更新其他信息（即行业、州等）</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当Marketo附加指定帐户时，我们将更新规则（在后台），该规则允许我们识别应成为指定帐户一部分的人员。 示例：如果将“IBM”更新为“IBM，美国”，则具有任一公司名称的人员将与指定帐户相关联。

如果Marketo找到我们视为重复项的记录，我们将仅处理第一个记录。
