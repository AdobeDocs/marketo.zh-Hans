---
description: 创建流 — Marketo文档 — 产品文档
title: 创建流
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: d2ac03bd01e1dd6998d47aac82383b64ffdd3ee7
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# 创建流 {#create-a-stream}

有 _许多_ 您可以创建的流组合。 本文包含一个示例，营销人员在该示例中询问网站访客是否有任何产品问题。 如果是，则访客可以计划约会。 如果否，则访客可以选择加入邮件列表以备将来通信。 目标是计划约会或收集访客的电子邮件。

![](assets/create-a-stream-0.png)

1. 在 [创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue)，请单击 **流设计器** 选项卡。

   ![](assets/create-a-stream-1.png)

1. 拖放问题卡。

   ![](assets/create-a-stream-2.png)

1. 在“查特机器人响应”下，回答您的问题。

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Poke默认设置为on ，该设置在聊天图标旁边显示开题问题，访客无需单击该图标即可看到该问题。

1. 输入用户响应并单击 **保存**.

   ![](assets/create-a-stream-4.png)

1. 对于“是”，我们要计划日程安排，因此该选项下方会拖动到日程安排计划程序卡上。

   ![](assets/create-a-stream-5.png)

1. 在右侧的列中，单击 **保存**.

   ![](assets/create-a-stream-6.png)

1. 由于这是一个目标，请将目标卡拖动到日程安排计划程序下方。

   ![](assets/create-a-stream-7.png)

1. 命名您的目标（或选择现有目标）并单击 **保存**.

   ![](assets/create-a-stream-8.png)

1. 对于“否”，我们希望了解他们是否将加入邮件列表，因此，在下面，该选项会拖动到另一张问题卡上。

   ![](assets/create-a-stream-9.png)

1. 输入您的响应，并为访客添加响应选项。 单击 **保存** 完成时。

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >您可以通过单击 **添加响应**.

1. 在“是”响应下方，将鼠标拖动到“信息捕获”卡上，以便收集访客的电子邮件。

   ![](assets/create-a-stream-11.png)

1. 单击 **类型** 下拉框并选择 **电子邮件**.

   ![](assets/create-a-stream-12.png)

1. 输入聊天机器人消息和占位符。 确保将属性映射到Marketo中的相应字段，然后单击 **保存**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>类型</strong></td>
     <td>要捕获的信息类型：电话，短信，电子邮件。</td>
    </tr>
    <tr>
     <td><strong>聊天机器人消息</strong></td>
     <td>访客看到的消息提示他们提供信息。</td>
    </tr>
    <tr>
     <td><strong>占位符</strong></td>
     <td>帮助访客查看要输入内容的示例文本。</td>
    </tr>
    <tr>
     <td><strong>将响应映射到属性</strong></td>
     <td>用于将访客的响应同步到其在Marketo订阅中的人员记录中的相应字段。</td>
    </tr>
   </table>

1. 由于收集其电子邮件是一个目标，因此请将目标卡片拖动到“信息捕获”下方。

   ![](assets/create-a-stream-14.png)

1. 命名您的目标（或选择现有目标）并单击 **保存**.

   ![](assets/create-a-stream-15.png)

1. 请记住，如果用户说“否”，请添加响应。 将消息卡拖动到该选项下方。

   ![](assets/create-a-stream-16.png)

1. 输入您的消息并单击 **保存**.

   ![](assets/create-a-stream-17.png)

1. 选择 **预览** 切换以预览对话框。

   ![](assets/create-a-stream-18.png)

1. 准备好激活对话框后，单击 **发布**.

   ![](assets/create-a-stream-19.png)

>[!NOTE]
>
>在单击发布之前，请记得确保 [输入了目标URL](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>[对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
