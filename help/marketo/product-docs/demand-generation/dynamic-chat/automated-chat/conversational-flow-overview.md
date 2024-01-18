---
description: 对话流概述 — Marketo文档 — 产品文档
title: 对话流概述
feature: Dynamic Chat
exl-id: c741886d-d672-471f-8902-208d25898afa
source-git-commit: 492a43045bdf77243e4600eeb2223e750a35859b
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 对话流概述 {#conversational-flow-overview}

设计对话流，并根据特定操作（例如，单击行动号召按钮、页面加载时、页面逗留时间等）将其触发给任何访客。

![](assets/conversational-flow-overview-1.png)

>[!NOTE]
>
>对话流和实时聊天是共享试用功能，Dynamic ChatSelect程序包上的参与的总生命周期限制为100次。 当达到此限制时，所有发布的对话流将停止触发，并且请求与实时代理进行聊天的访客将收到全局回退消息。 要增加此限制，请联系您的客户代表以讨论包升级选项。

## 对话框与对话流 {#dialogues-vs-conversational-flows}

虽然对话流和对话流具有许多相似之处，但它们是两个独立的特征。

<table> 
 <tbody> 
  <tr> 
   <th style="width:50%">对话</th> 
   <th style="width:50%">会话流</th>
  </tr> 
  <tr> 
   <td>对话框具有针对性 — 您可以根据实施的参数为特定页面和受众设计对话。</td> 
   <td>触发对话流 — 您设计可以根据访客的操作（如填写表单、单击链接等）触发的对话。</td>
  </tr>
   <tr> 
   <td>仅在聊天机器人界面中受支持。</td> 
   <td>当前在弹出界面中受支持，计划提供更多界面。</td>
  </tr>
  </tr>
   <tr> 
   <td>可以为同一潜在客户区段创建多个对话框，每个访客按优先级顺序查看对话框，以便他们能够继续参与。</td> 
   <td>对话流没有优先级顺序，并且可以根据行动号召确定的由同一潜在客户触发任意次数。</td>
  </tr>
  <tr>
   <td>聊天机器人对话由对话框提供支持。</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">对话式Forms</a> Marketo Engage由对话流提供支持。</td>
  </tr>
 </tbody> 
</table>

## “流设计器”选项卡 {#stream-designer-tab}

用于对话流的流设计器与用于对话框的流设计器几乎相同。 [在此处了解所有相关信息](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}.

![](assets/conversational-flow-overview-2.png)

## “报表”选项卡 {#reports-tab}

在“报表”选项卡中，您将能够查看有关您的对话流表现的量度。

![](assets/conversational-flow-overview-3.png)

查看参与率、转化率、按已知和/或未知访客过滤等。

![](assets/conversational-flow-overview-4.png)

## “设置”选项卡 {#settings-tab}

![](assets/conversational-flow-overview-5.png)

在“设置”选项卡的上半部分，您可以更新对话流的名称、添加可选描述以及更改语言。

![](assets/conversational-flow-overview-6.png)

>[!NOTE]
>
>选择其他语言只会更改系统文本的语言。 您负责翻译内容。

### 对话SDK {#conversations-sdk}

在“设置”选项卡的下半部分，自定义“对话”触发器（也称为“对话SDK”）。 您可以决定是在访客单击任意链接时还是在页面加载时在您的网站上触发对话。

![](assets/conversational-flow-overview-7.png)

>[!TIP]
>
>请参阅 [对话SDK](https://experienceleague.adobe.com/tools/marketo-dynamic-chatbot/conversations-sdk/){target="_blank"} 行动起来！

>[!MORELIKETHIS]
>
>[创建对话流](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md){target="_blank"}
