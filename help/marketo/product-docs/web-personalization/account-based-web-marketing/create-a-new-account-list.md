---
unique-page-id: 4720232
description: 新建帐户列表 — Marketo文档 — 产品文档
title: 创建新的帐户列表
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 创建新的帐户列表 {#create-a-new-account-list}

创建并上传组织和域名列表，以通过个性化的促销活动定位这些关键帐户。

>[!NOTE]
>
>本文仅适用于旧版Web ABM客户。 如果您是在2016年9月之后获得Web ABM，请按照[本文](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList)中的步骤进行操作。

## 创建新的帐户列表 {#create-a-new-account-list-1}

1. 转到&#x200B;**[!UICONTROL Account Lists]**。

   ![](assets/dropdown-account-lists-hand.jpg)

1. 选择 **[!UICONTROL Create New]**。

   ![](assets/create-new-account-list-hand.jpg)

1. 选择&#x200B;**[!UICONTROL Browse]**&#x200B;并上传CSV文件（确保csv文件符合条件）。 添加&#x200B;**[!UICONTROL List Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**。 单击 **[!UICONTROL Save]**。

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**CSV文件的格式是什么？**
   >
   >确保指定帐户CSV文件满足以下要求：
   >
   >* 另存为CSV格式
   >* 不超过10MB
   >* 只有标题列A：名称，列B：域，列C：国家/地区，列D：美国州4列。
   >* 上传的文件最多可能需要两个工作日才能获得批准。
   >* 您将在指定帐户页面中收到批准电子邮件通知或检查文件的状态。
   >* 针对所有已上传列表累计的记录数/行数从1万开始计数，最大程序包总计为10万。

   >[!NOTE]
   >
   >**CSV文件示例**
   >
   >* 行1列A值=组织
   >* 行1列B值=域
   >* 行1列C值=国家/地区
   >* 行1列D值=美国州
   >* 其中一个列值是必需的。 但是，同时提供组织和域名可以提高帐户列表的匹配率。
   >* “国家/地区”和“州/省”为可选值。
   >
   >   * 对于国家/地区名称，请使用完整的国家/地区名称或缩写代码。 例如 美国或美国。
   >   * 对于美国各州，使用两个字母的缩写代码，即CA。 只有美国的州才被承认。
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## 编辑帐户列表 {#edit-an-account-list}

在&#x200B;**帐户列表**&#x200B;页面上，单击列表上的&#x200B;**编辑**&#x200B;图标。

![](assets/create-new-account-list-edit.jpg)

选择&#x200B;**[!UICONTROL Browse...]**&#x200B;并上传新的CSV文件。 此文件将替换原始文件。 单击&#x200B;**[!UICONTROL Save]**。 新上传的文件将处于待处理状态，直到Marketo支持批准为止，当处于待处理状态时，原始文件将保持活动状态。

![](assets/set-account-list-edit-hands.jpg)

CSV文件将替换现有文件。 在新文件处理完成之前，现有列表将保持活动状态。

## 删除指定帐户列表 {#delete-a-named-account-list}

1. 在&#x200B;**[!UICONTROL Account Lists]**&#x200B;页面上，单击要删除的列表的“删除”图标。

   ![](assets/create-new-account-list-delete.jpg)

1. 此时将显示一条消息，确认您是否要删除该列表。 单击 **[!UICONTROL OK]**。

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[使用帐户列表创建区段](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
