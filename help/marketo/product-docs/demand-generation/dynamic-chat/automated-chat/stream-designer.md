---
description: Designer流 — Marketo文档 — 产品文档
title: 流设计器
feature: Dynamic Chat
exl-id: 310b1dff-dd93-48a6-85c2-64c58494ce48
source-git-commit: d73ff37236abbd0d97631ad66b8eb34473650554
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 2%

---

# 流设计器 {#stream-designer}

可能有&#x200B;_多个_&#x200B;流组合。 本文包含一个示例，其中营销人员询问网站访客是否对产品有任何疑问。 如果是，访客可以安排约会。 如果没有，访客可以选择加入邮件列表以备将来通信。 酒店还提供免费的PDF。 最终目标是安排约会或收集访客的电子邮件。

>[!PREREQUISITES]
>
>必须先在您的Adobe帐户中[设置文档卡](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"}，然后才能使用文档卡。

## Designer卡片流 {#stream-designer-cards}

Stream Designer包含多个卡，您可以添加这些卡来塑造聊天对话。

<table>
 <tr>
  <td style="width:25%"><strong>消息</strong></td>
  <td style="width:75%">当您想在不做任何响应的情况下发表声明时(例如：“您好！ 使用优惠码SAVE25”，现享所有项目现享25%优惠)。
</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>问题</strong></td>
  <td>当您想询问多选问题时使用，您可以提供其中可用的回答(例如：您感兴趣的车辆类型是什么？ 响应= SUV、紧凑型、卡车等)。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>文档</strong></td>
  <td>允许您将PDF文档嵌入对话框并跟踪访客的文档参与活动（查看了多少页面、是否下载了文档以及/或者使用了任何搜索词）。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>信息捕获</strong></td>
  <td>在要收集信息（例如，姓名、电子邮件地址、职务等）时使用。 选择要将访客的响应归因到哪个字段后，您可以选择允许访客键入其响应，或从您确定的选择列表中选择选项（提示：后者有助于保持数据库清洁）。 您还可以选择用用户的响应覆盖当前为其列出的任何数据，或者完全跳过问题（如果您已经为其指定了值）。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>会议预订</strong></td>
  <td>为访客提供可用于安排会议的日期的日历。 通过循环调度法、特定代理或使用自定义规则选择日历可用性。 如果要捕获代理的名称或电子邮件地址，并将其分配给聊天访客的个人记录以供将来查询，请单击<b>添加属性</b>(提示：创建一个<a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">自定义字段</a>以将代理的信息映射到以便不覆盖标准Marketo Engage字段)。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>目标</strong></td>
  <td>这是访客不会看到的唯一一张卡。 由您来确定在特定聊天中实现目标的时间（例如：如果收集访客的电子邮件是您的目标，则将“目标”卡片放在流中信息捕获后的紧跟位置）。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>操作*</strong></td>
  <td>与表单中的隐藏字段类似，使用操作卡，您可以用要针对潜在客户记录捕获的隐式值填充任何潜在客户或公司属性（具有<a href="/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md#string">字符串数据类型</a>）。 您可以在对话的任何位置添加操作卡，并使用自动填充相应值的值或本机令牌更新相应的属性。
  <p><i>*此卡需要使用Dynamic Chat Prime。 有关详细信息，请联系Adobe客户团队（您的客户经理）。</i></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>实时聊天</strong></td>
  <td>当您希望访客与实时座席聊天时，可使用实时聊天卡。
  <li>实时聊天卡必须是分支中的最后一张卡。</li>
  <li>访客一旦在流中到达此信息卡就会被路由到代理，因此建议在此信息卡之前添加一个问题卡，询问访客是否愿意与实时代理聊天。</li></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>生成的响应*</strong></td>
  <td>为访客在对话中到达某个时间点时创建消息。 设置他们一次可以提出的一系列问题，以获得您所需的关键绩效指标。
  <p><i>*此卡需要使用Dynamic Chat Prime。 有关详细信息，请联系Adobe客户团队（您的客户经理）。</i></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>条件分支</strong></td>
  <td>根据不同的条件，在对话框流中创建分支。 根据Marketo Engage中的商机和公司属性，在同一对话框中向不同人员展示不同的内容。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>会话流</strong></td>
  <td>使用对话流卡简化对话框中流中的多个步骤。</td>
 </tr>
</table>

## 流式传输Designer图标 {#stream-designer-icons}

在Stream Designer的右上角，您会看到几个图标。 这是他们所做的。

<table>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-1.png"></td>
  <td>放大，创建更大的卡片</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-2.png"></td>
  <td>缩小，创建较小的卡片</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-3.png"></td>
  <td>打开一个用于测试聊天内容的窗口（按同一按钮关闭）</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-4.png"></td>
  <td>允许您在流中搜索卡片类型或内容</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-5.png"></td>
  <td>排列您的流中的所有卡片</td>
 </tr>
</table>

## 创建流 {#create-a-stream}

您可以为对话框或[对话Forms](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}创建流。 在本例中，我们将为对话框创建一个。

1. 在[创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}后，单击&#x200B;**[!UICONTROL Stream Designer]**&#x200B;选项卡。

   ![](assets/stream-designer-6.png)

1. 拖放&#x200B;_[!UICONTROL Question]_&#x200B;信息卡。

   ![](assets/stream-designer-7.png)

1. 在[!UICONTROL Chatbot Response]下，说出您想怎么回答的问题。

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >您可以自定义聊天访客的体验！
   >
   >* 单击“插入HTML”图标`</>`可插入您自己的HTML，以了解所需的对话外观。
   >
   >* 使用已知聊天访客的令牌来个性化其体验（例如： Hello `{{lead.leadFirstName:""}}`）。 单击花括号图标`{}`并进行选择。 如果您希望匿名访客看到一些通用内容（例如： Hello `{{lead.leadFirstName:"there"}}`），请在引号之间添加默认值。

   >[!NOTE]
   >
   >默认情况下，Poke设置为on，它会在聊天图标旁边显示开始的问题，访客无需单击该图标即可查看。 Poke仅在对话的第一张卡片中可用。

1. 输入您的用户响应并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**[!UICONTROL Edit Stored Values]**&#x200B;是可选步骤，适用于那些想要在数据库中存储与聊天机器人针对问题卡中的映射属性显示的值不同的值（例如：访客看到“搜索引擎优化”，您将该值存储为“SEO”。）

1. 对于“是”，我们希望预订会议，因此在该选项下方，拖动到&#x200B;_会议预订_&#x200B;卡片。

   ![](assets/stream-designer-10.png)

1. 在右侧的列中，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/stream-designer-11.png)

1. 由于这是目标，请将[!UICONTROL Goal]卡拖动到约会计划程序下。

   ![](assets/stream-designer-12.png)

1. 命名您的目标（或选择现有目标），然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/stream-designer-13.png)

1. 对于“否”，我们希望查看他们是否会加入邮件列表，因此在该选项下拖动到另一个[!UICONTROL Question]卡片上。

   ![](assets/stream-designer-14.png)

1. 输入您的响应，并为访客添加响应选项。 完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >您可以通过单击&#x200B;**[!UICONTROL Add Response]**&#x200B;添加更多响应。

1. 在“是”响应下方，将拖到“信息捕获”卡上，以便收集访客的电子邮件。

   ![](assets/stream-designer-16.png)

1. 单击&#x200B;**[!UICONTROL Type]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL Email]**。

   ![](assets/stream-designer-17.png)

1. 输入聊天机器人消息和占位符。 确保该属性映射到Marketo Engage中的相应字段，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td style="width:30%"><strong>类型</strong></td>
     <td>要捕获的信息类型：电话、文本、电子邮件。</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>聊天机器人消息</strong></td>
     <td>访客看到的提示他们提供信息的消息。</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>占位符</strong></td>
     <td>帮助访客查看要输入内容的示例文本。</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>将响应映射到属性</strong></td>
     <td>允许您将访客的响应同步到Marketo Engage订阅中其人员记录中的相应字段。</td>
    </tr>
   </table>

1. 由于收集其电子邮件是一个目标，因此请将[!UICONTROL Goal]信息卡拖动到“信息捕获”下方。

   ![](assets/stream-designer-19.png)

1. 命名您的目标（或选择现有目标），然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/stream-designer-20.png)

1. 如果回答“否”，请记得添加响应。 一种选择是将信息卡拖到下面并说“谢谢”。 但在本例中，我们将向他们提供免费的PDF文档。

   ![](assets/stream-designer-21.png)

1. 在本例中，我们将创建一个新文档。 为其命名，输入已托管的PDF的URL，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/stream-designer-22.png)

1. 选择&#x200B;**[!UICONTROL Preview]**&#x200B;切换可预览您的对话框。

   ![](assets/stream-designer-23.png)

1. 准备好激活对话框后，请单击&#x200B;**[!UICONTROL Publish]**。

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>在单击[!UICONTROL Publish]之前，请记住确保已[输入您的目标URL](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md#target){target="_blank"}。

>[!MORELIKETHIS]
>
>* [创建对话框](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [受众条件](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md){target="_blank"}
>* [Adobe PDF嵌入API](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"}
