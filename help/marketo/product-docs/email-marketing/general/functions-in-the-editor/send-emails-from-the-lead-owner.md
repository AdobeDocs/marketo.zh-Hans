---
unique-page-id: 1147340
description: 从潜在客户所有者发送电子邮件 — Marketo文档 — 产品文档
title: 从潜在客户所有者发送电子邮件
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 从潜在客户所有者发送电子邮件 {#send-emails-from-the-lead-owner}

如果您想代表潜在客户所有者向潜在客户发送电子邮件，该怎么办？  这是方法。

1. 查找您的电子邮件，选择它并单击 **编辑草稿**.

   ![](assets/one.png)

1. 单击 **从** 字段（删除任何现有名称），然后单击 **插入令牌** 按钮。

   ![](assets/two.png)

1. 开始键入“`{{lead.Lead Owner`&quot; ，然后选择 **`{{lead.Lead Owner First Name}}`** 令牌。

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. 如果潜在客户尚未拥有潜在客户所有者，请输入默认值，然后单击 **插入**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. 单击第一个令牌后面的，添加一个空格，然后单击 **插入令牌** 按钮。

   ![](assets/five.png)

1. 开始键入“`{{lead.Lead Owner`&quot; ，然后选择 **`{{lead.Lead Owner Last Name}}`** 令牌。

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. 如果潜在客户尚未拥有潜在客户所有者，请输入默认值，然后单击 **插入**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >确保在名字令牌和姓氏令牌之间添加了空格。

1. 单击发件人电子邮件字段（删除任何现有的电子邮件地址），然后单击插入令牌按钮。

   ![](assets/eight.png)

1. 开始键入“`{{lead.Lead Owner`&quot; ，然后选择 **`{{lead.Lead Owner Email Address}}`** 令牌。

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. 如果潜在客户尚未拥有潜在客户所有者，请输入默认值，然后单击 **插入**.

   ![](assets/ten.png)

1. 确保 **回复** 和 **主题** 填满了字段，你就完了！

   ![](assets/eleven.png)
