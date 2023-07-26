---
unique-page-id: 1147340
description: 发送来自潜在客户所有者的电子邮件 — Marketo文档 — 产品文档
title: 从潜在客户所有者发送电子邮件
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 从潜在客户所有者发送电子邮件 {#send-emails-from-the-lead-owner}

如果要代表Lead Owner向Lead发送电子邮件，该怎么办？  具体方法如下。

1. 查找您的电子邮件，选择它并单击 **编辑草稿**.

   ![](assets/one.png)

1. 单击 **从** 字段（删除任何现有名称），然后单击 **插入令牌** 按钮。

   ![](assets/two.png)

1. 开始键入&#39;&#39;`{{lead.Lead Owner`”并选择 **`{{lead.Lead Owner First Name}}`** 令牌。

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. 输入默认值，以防潜在客户还没有潜在客户责任人，然后单击 **插入**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. 在第一个令牌之后单击，添加空格，然后单击 **插入令牌** 按钮。

   ![](assets/five.png)

1. 开始键入&#39;&#39;`{{lead.Lead Owner`”并选择 **`{{lead.Lead Owner Last Name}}`** 令牌。

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. 输入默认值，以防潜在客户还没有潜在客户责任人，然后单击 **插入**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >确保在名字和姓氏令牌之间添加了空格。

1. 单击从电子邮件字段（删除任何现有的电子邮件地址），然后单击插入令牌按钮。

   ![](assets/eight.png)

1. 开始键入&#39;&#39;`{{lead.Lead Owner`”并选择 **`{{lead.Lead Owner Email Address}}`** 令牌。

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. 输入默认值，以防潜在客户还没有潜在客户责任人，然后单击 **插入**.

   ![](assets/ten.png)

1. 确保 **回复** 和 **主题** 字段已填充，操作已完成！

   ![](assets/eleven.png)
