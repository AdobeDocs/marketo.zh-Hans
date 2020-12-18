---
unique-page-id: 4720232
description: 创建新帐户列表- Marketo Docs —— 产品文档
title: 创建新帐户列表
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# 创建新帐户列表{#create-a-new-account-list}

创建并上传组织和域名列表，用个性化活动目标这些关键帐户。

>[!NOTE]
>
>本文仅适用传统Web ABM客户。 如果您在2016年9月之后获得了Web ABM，请改为按照[本文](http://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList)中的步骤操作。

## 创建新帐户列表{#create-a-new-account-list-1}

1. 转到&#x200B;**帐户列表**。

   ![](assets/dropdown-account-lists-hand.jpg)

1. 选择&#x200B;**新建**。

   ![](assets/create-new-account-list-hand.jpg)

1. 选择&#x200B;**浏览**&#x200B;并上传您的CSV文件（确保csv文件符合条件）。 添加&#x200B;**名称**&#x200B;和&#x200B;**说明**。 单击&#x200B;**保存**。

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**CSV文件的格式是什么？**
   >
   >
   >确保指定帐户的CSV文件满足以下要求：
   >
   >* 另存为CSV格式
   >* 不超过10MB
   >* 标题列A仅有4列：名称，列B:域，列C:国家／地区，D列：美国州。
   >* 上传的文件最长可能需要2个工作日才能获得批准。
   >* 您将在“指定帐户”页面中收到批准电子邮件通知或检查文件状态。
   >* 所有列表上传开始在10K时累积的记录／行总数，其中最大的包总计为100K。


   >[!NOTE]
   >
   >**示例**
   >
   >**CSV文件示例**
   >
   >* 行1列A值=组织
   >* 行1列B值=域
   >* 行1列C值=国家／地区
   >* 行1列D值=美国州
   >* 其中一个列值是必填的。 但是，提供组织和域名可提高帐户列表的匹配率。
   >* 国家／地区和州是可选值。

      >
      >  
   * 对于国家／地区名称，请使用完整的国家／地区名称或缩写代码。 例如 美国或美国。
   >  * 对于美国州，请使用2个字母的缩写代码，即CA。 只有美国各州得到承认。

   >    
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## 编辑帐户列表{#edit-an-account-list}

在&#x200B;**帐户列表**&#x200B;页面上，单击列表上的**编辑**图标。

![](assets/create-new-account-list-edit.jpg)

选择&#x200B;**浏览**&#x200B;并上传新的CSV文件。 此文件将替换原始文件。 单击&#x200B;**保存**。 新上传的文件将处于挂起状态，直到Marketo Support批准为止，如果处于挂起状态，原始文件将保持活动状态。

![](assets/set-account-list-edit-hands.jpg)

CSV文件将替换现有文件。 现有列表将保持活动状态，直到新文件的处理完成。

## 删除指定帐户列表{#delete-a-named-account-list}

1. 在**帐户列表**页上，单击要删除的列表的**删除**图标。

   ![](assets/create-new-account-list-delete.jpg)

1. 系统会显示一条消息，确认是否要删除列表。 单击&#x200B;**确定**。

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>* [使用帐户创建列表](create-a-segment-using-an-account-list.md)
>* [视图指定帐户列表](http://docs.marketo.com/pages/viewpage.action?pageid=4720244)

