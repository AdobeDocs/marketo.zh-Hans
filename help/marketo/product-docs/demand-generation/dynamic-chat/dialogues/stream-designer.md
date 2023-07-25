---
description: 流设计器 — Marketo文档 — 产品文档
title: 流设计器
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
feature: Dynamic Chat
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 2%

---

# 流设计器 {#stream-designer}

有 _许多_ 可能的流组合。 本文包含一个示例，营销人员在该示例中询问网站访客是否遇到任何产品问题。 如果是，访客可以安排约会。 如果没有，访客可以选择加入邮件列表以备将来通信。 酒店还提供免费PDF。 最终目标是安排约会或收集访客的电子邮件。

>[!PREREQUISITES]
>
>在使用“文档”卡之前，您必须先 [设置](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"} 在您的Adobe帐户中。

## 流设计器信息卡 {#stream-designer-cards}

流设计器包含多个可添加的卡片，以塑造聊天对话。

<table>
 <tr>
  <td><strong>消息</strong></td>
  <td>当您想发表声明而不需要响应时(例如：“Hi！ 使用优惠码SAVE25”，现享所有项目现享25%优惠。
</td>
 </tr>
 <tr>
  <td><strong>问题</strong></td>
  <td>当您要提出多个选择题时，请使用该题来提供可用的回答(例如：您对哪种类型的媒介感兴趣？ 响应= SUV、紧凑、卡车等)。</td>
 </tr>
 <tr>
  <td><strong>文档</strong></td>
  <td>允许在对话框中嵌入PDF文档并跟踪访客的文档参与活动（查看了多少页、文档是否下载以及/或者使用了任何搜索词）。</td>
 </tr>
 <tr>
  <td><strong>信息捕获</strong></td>
  <td>收集信息时使用。 三个字段可供选择：电子邮件地址、电话号码和文本（允许访客编写自己的消息）。</td>
 </tr>
 <tr>
  <td><strong>预约调度程序</strong></td>
  <td>为访客提供一个包含可用日期的日历以安排跟进。 日历可用性反映为 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">下一个排队座席</a>.</td>
 </tr>
 <tr>
  <td><strong>目标</strong></td>
  <td>这是访客不会看到的唯一一张卡。 由您来确定在特定聊天中何时实现目标（例如：如果收集访客的电子邮件是您的目标，则将“目标”卡片放置在流中信息捕获之后紧跟其后）。</td>
 </tr>
</table>

## 流设计器图标 {#stream-designer-icons}

在流设计器的右上角，您会看到几个图标。 这是他们所做的。

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>为喜欢该视图的用户在背景中添加网格</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>放大，创建更大的信息卡</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>缩小，创建较小的卡片</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>打开一个用于测试聊天内容的窗口（按同一按钮关闭）</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>排列您的流中的所有卡片</td>
 </tr>
</table>

## 创建流 {#create-a-stream}

1. 在您 [已创建您的对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}，单击 **流设计器** 选项卡。

   ![](assets/stream-designer-6.png)

1. 拖放问题卡。

   ![](assets/stream-designer-7.png)

1. 在“聊天机器人响应”下，说出您希望如何回答的问题。

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >您可以使用令牌为已知聊天访客个性化体验(例如：Hello `{{lead.leadFirstName:""}}`)。 只需单击右侧的花括号图标即可进行选择。 如果您希望匿名访客看到一些通用内容（例如：Hello），请在引号之间添加默认值 `{{lead.leadFirstName:"there"}}`)。

   >[!NOTE]
   >
   >默认情况下，Poke设置为on，它会在聊天图标旁边显示开始的问题，访客无需单击它即可查看。 Poke仅在对话的第一张卡片中可用。

1. 输入用户响应并单击 **保存**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**编辑存储的值** 对于想要在数据库中存储与聊天机器人中显示的“问题”信息卡中映射属性的值不同的值的人来说，这是一个可选步骤（例如：访客看到“搜索引擎优化”，您将该值存储为“SEO”。）

1. 对于“是”，我们需要安排约会，因此在该选项的下方，将拖到“约会安排器”卡上。

   ![](assets/stream-designer-10.png)

1. 在右侧的列中，单击 **保存**.

   ![](assets/stream-designer-11.png)

1. 由于这是目标，因此请将“目标”卡拖动到“约会计划器”下方。

   ![](assets/stream-designer-12.png)

1. 命名您的目标（或选择现有目标），然后单击 **保存**.

   ![](assets/stream-designer-13.png)

1. 对于“否”，我们想要查看他们是否会加入邮件列表，因此在该选项下拖动到另一个问题卡上。

   ![](assets/stream-designer-14.png)

1. 输入您的响应，并为访客添加响应选项。 单击 **保存** 完成时。

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >您可以通过单击 **添加响应**.

1. 在“是”响应下方，拖动信息捕获卡以收集访客的电子邮件。

   ![](assets/stream-designer-16.png)

1. 单击 **类型** 下拉菜单并选择 **电子邮件**.

   ![](assets/stream-designer-17.png)

1. 输入聊天机器人消息和占位符。 确保将属性映射到Marketo中的相应字段，然后单击 **保存**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td><strong>类型</strong></td>
     <td>要捕获的信息类型：电话、文本、电子邮件。</td>
    </tr>
    <tr>
     <td><strong>聊天机器人消息</strong></td>
     <td>访客看到的提示他们提供信息的消息。</td>
    </tr>
    <tr>
     <td><strong>占位符</strong></td>
     <td>帮助访客查看要输入内容的示例文本。</td>
    </tr>
    <tr>
     <td><strong>将响应映射到属性</strong></td>
     <td>允许您将访客的响应同步到Marketo订阅中其人员记录中对应的字段。</td>
    </tr>
   </table>

1. 由于收集其电子邮件是一个目标，因此请将“目标”信息卡拖动到“信息捕获”下方。

   ![](assets/stream-designer-19.png)

1. 命名您的目标（或选择现有目标），然后单击 **保存**.

   ![](assets/stream-designer-20.png)

1. 如果说“不”，请记得添加回复。 一个选项是将信息卡拖到下面并说“谢谢”。 但在本例中，我们将改为向他们提供免费PDF文档。

   ![](assets/stream-designer-21.png)

1. 在本例中，我们将创建一个新文档。 为其命名，输入已托管PDF的URL，然后单击 **保存**.

   ![](assets/stream-designer-22.png)

1. 选择 **预览** 切换可预览您的对话框。

   ![](assets/stream-designer-23.png)

1. 准备好激活对话框后，单击 **Publish**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>在单击“发布”之前，请记住确保已 [已输入您的目标URL](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}
>* [受众标准](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target="_blank"}
>* [报表](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target="_blank"}
>* [使用文档信息卡](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"}
