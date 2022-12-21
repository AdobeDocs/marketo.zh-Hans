---
description: 设置ON24与Marketo的集成 — Marketo文档 — 产品文档
title: 设置ON24与Marketo的集成
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
source-git-commit: 3e0823976e8b837fcb2fdbbf03f26da48cbd74b7
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---

# 设置ON24与Marketo的集成{#set-up-the-on24-integration-with-marketo}

以下是如何设置ON24事件集成。

## 创建仅限API的角色 {#create-an-api-only-role}

1. 在我的Marketo中，单击 **管理员**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. 在“安全”下，单击 **用户和角色**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. 单击 **角色** 选项卡，然后 **新角色**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. 输入角色名称。 打开 **访问API** 菜单，然后选择“读写自定义对象”和“读写人员”。 单击&#x200B;**创建**。

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## 创建新用户 {#create-a-new-user}

1. 仍然在用户和角色中，单击 **用户** 选项卡，单击 **邀请新用户**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. 输入新用户的信息并单击 **下一个**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. 选择您刚刚创建的ON24 API仅角色。 选择 **仅限API** 复选框。 单击 **下一个**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. 单击 **发送**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>仅API用户不需要邀请。

## 设置ON24连接 {#set-up-on24-connection}

1. 仍在“管理员”部分，单击 **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. 单击 **新建** then **新服务**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. 选择显示名称。 单击 **服务** 下拉框并选择 **自定义**. 输入描述。 单击仅API用户下拉列表，然后选择您创建的用户 [在上述步骤中](#create-a-new-user). 单击&#x200B;**创建**。

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. 找到您刚刚创建的自定义LaunchPoint服务，然后单击查看详细信息。

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. 突出显示、右键单击、复制并保存客户端ID（您稍后将需要它）。 重复执行客户端密钥。

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. 在左侧的树中，单击“Web服务”。

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. 在“REST API”下，突出显示、右键单击并复制身份的第一部分并保存该部分（直到.com中的“m”为止）。

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. 使用保存的客户端ID、客户端密钥和身份，导航到您的ON24帐户。 其余步骤将在该处执行，并且 [此处](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target=&quot;_blank&quot;}。
