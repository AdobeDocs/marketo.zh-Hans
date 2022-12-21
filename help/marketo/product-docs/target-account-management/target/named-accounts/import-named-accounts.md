---
unique-page-id: 12615800
description: 导入指定帐户 — Marketo文档 — 产品文档
title: 导入指定帐户
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# 导入指定帐户 {#import-named-accounts}

是否已拥有一个装满潜在目标帐户的CSV? 直接导入TAM!

1. 单击 **新建** 下拉框并选择 **导入指定帐户**.

   ![](assets/inaone.png)

1. 将打开一个新窗口。 单击 **浏览**，然后选择要导入的已命名帐户的文件。

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >在您的文件中，提供 [信息量](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) 尽可能。 只能添加字母信息；Marketo不会计算任何内容（即管道）。 要根据CRM帐户创建指定帐户，只需将帐户名和CRM ID从您的CRM导出到CSV文件中，使用帐户名称选项，然后在导入过程中映射CRM ID即可。 要将CRM帐户正确关联到指定帐户，您必须提供CRM帐户的确切名称。

1. 从两种重复数据消除模式中进行选择：帐户名称或域名。 在本例中，我们将选择“帐户”。 单击 **模式** 下拉框并选择 **按帐户名称**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >如果您选择 **按域模式**，则必须同时包含命名帐户和域字段。

1. 要选择将您的指定帐户添加到的帐户列表，请单击 **帐户列表** 下拉菜单，然后进行选择。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >您还可以通过在下拉框中键入帐户列表名称来创建全新的帐户列表。

1. 要发送导入通知，请单击 **将警报发送到** 下拉菜单并选择一个Marketo用户。 您 _无法_ 手动输入电子邮件地址。

   ![](assets/inafive-2.png)

1. 单击 **下一个**.

   ![](assets/inasix-2.png)

1. 双击 **Marketo字段** 下拉菜单，然后选择相应的字段。 单击 **下一个** 完成时。

   ![](assets/inaseven.png)

   成功!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >“检查导入状态”仅显示活动的最近三天。

按帐户名称进行重复数据消除时的情景：

<table> 
 <tbody> 
  <tr> 
   <td><strong>正在导入具有现有命名帐户名称的记录</strong></td> 
   <td><p>我们将更新现有记录</p></td> 
  </tr> 
  <tr> 
   <td><strong>正在导入具有新命名帐户名称的记录</strong></td> 
   <td>我们将创造新记录</td> 
  </tr> 
 </tbody> 
</table>

按域名进行重复数据消除时的情景：

<table> 
 <tbody> 
  <tr> 
   <td><strong>使用新帐户名和新域名导入记录</strong></td> 
   <td>我们将使用提供的信息创建一个新的指定帐户</td> 
  </tr> 
  <tr> 
   <td><strong>使用现有帐户名和现有域名导入记录</strong></td> 
   <td>我们将更新现有的指定帐户</td> 
  </tr> 
   <tr> 
   <td><strong>使用新帐户名和现有域名导入记录</strong></td> 
   <td>我们会将新帐户名称附加到与域名匹配的现有命名帐户中，并更新其他信息（如行业、州等）</td> 
  </tr> 
  <tr> 
   <td><strong>使用现有命名帐户名和新域名导入记录</strong></td> 
   <td>我们会将新域名附加到与帐户名称匹配的现有命名帐户中，并更新其他信息（如行业、州等）</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当Marketo附加指定帐户时，我们将更新规则（幕后），以便我们识别应属于指定帐户的人员。 示例：如果将“IBM”更新为“美国IBM”，则具有任一公司名称的人员将关联到指定帐户。

如果Marketo找到我们视为重复项的记录，我们将仅处理第一个记录。
