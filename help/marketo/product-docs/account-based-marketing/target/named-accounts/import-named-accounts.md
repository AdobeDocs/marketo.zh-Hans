---
unique-page-id: 12615800
description: 导入指定帐户- Marketo Docs —— 产品文档
title: 导入指定帐户
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# 导入命名帐户{#import-named-accounts}

是否已经拥有装满潜在目标帐户的CSV? 直接导入ABM!

1. 单击&#x200B;**新建**&#x200B;下拉框并选择&#x200B;**导入命名帐户**。

   ![](assets/inaone.png)

1. 将打开一个新窗口。 单击&#x200B;**浏览**，然后选择要导入的已命名帐户的文件。

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >在文件中，尽可能提供[信息](/help/marketo/product-docs/account-based-marketing/target/named-accounts/named-account-overview.md#named-account-attributes)。 只能添加图片信息；Marketo不会计算任何内容（即管道）。 要创建基于CRM帐户的指定帐户，只需将帐户名和CRM ID从CRM导出到CSV文件中，使用“帐户名”选项，然后在导入过程中映射CRM ID。 要将CRM帐户正确链接到指定帐户，必须提供CRM帐户的确切名称。

1. 从两种重复数据消除模式中进行选择：帐户名或域名。 在此示例中，我们将选择帐户。 单击“**模式**”下拉框并选择“按帐户名称&#x200B;**”。**

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >如果选择&#x200B;**按域模式**，则必须同时包含指定的帐户和域字段。

1. 要选择将您的指定帐户添加到哪个帐户列表，请单击&#x200B;**帐户列表**&#x200B;下拉框，然后进行选择。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >您还可以通过在下拉框中键入帐户列表名称来创建全新的帐户帐户。

1. 要发送导入通知，请单击&#x200B;**将警报发送到**&#x200B;下拉框，然后选择Marketo用户。 _不能_&#x200B;手动输入电子邮件地址。

   ![](assets/inafive-2.png)

1. 单击&#x200B;**下一步**。

   ![](assets/inasix-2.png)

1. 通过多次单击&#x200B;**Marketo Field**&#x200B;下拉框并选择相应的字段，映射每个字段。 完成后，单击&#x200B;**Next**。

   ![](assets/inaseven.png)

   成功！

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >“检查导入状态”仅显示最近三天的活动。

按帐户名称进行重复数据消除时的情形：

<table> 
 <tbody> 
  <tr> 
   <td><strong>导入具有现有命名帐户名称的记录</strong></td> 
   <td><p>我们将更新现有记录</p></td> 
  </tr> 
  <tr> 
   <td><strong>导入具有新命名帐户名称的记录</strong></td> 
   <td>我们将创造新记录</td> 
  </tr> 
 </tbody> 
</table>

通过域名进行重复消除时的情形：

<table> 
 <tbody> 
  <tr> 
   <td><strong>使用新帐户名和新域名导入记录</strong></td> 
   <td>我们将使用提供的信息新建一个指定帐户</td> 
  </tr> 
  <tr> 
   <td><strong>使用现有帐户名和现有域名导入记录</strong></td> 
   <td>我们将更新现有的指定帐户</td> 
  </tr> 
   <tr> 
   <td><strong>使用新帐户名和现有域名导入记录</strong></td> 
   <td>我们将在与域名匹配的现有指定帐户后面附加新帐户名称，并更新其他信息（如行业、州等）</td> 
  </tr> 
  <tr> 
   <td><strong>导入具有现有命名帐户名和新域名的记录</strong></td> 
   <td>我们将在与帐户名称匹配的现有指定帐户后面附加新域名，并更新其他信息（如行业、州等）</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当Marketo附加一个指定帐户时，我们将更新一条规则（幕后），允许我们识别应该属于指定帐户的人员。 示例：如果将“IBM”更新为“IBM, USA”，则具有任一公司名的人员都将关联到指定帐户。

如果Marketo找到我们视为重复的记录，我们只会处理第一个记录。
