---
description: '[!DNL Dynamic Chat]活动 — Marketo文档 — 产品文档'
title: '[!DNL Dynamic Chat]活动'
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# [!DNL Dynamic Chat]活动 {#dynamic-chat-activities}

[!DNL Dynamic Chat]提供了多个筛选器和触发器以用于您的智能列表。

![](assets/dynamic-chat-activities-1.png)

## 定义 {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>已触发</b></td>
    <td>当访客满足对话框或对话流的定位标准并向对话框显示时，会发生触发事件。
    <br>每个访客、每个会话一个触发器事件。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>已参与会话流/对话</b></td>
    <td>Web访客首次单击对话框或对话流中的提示时（单击多选选项、提交信息、预订会议、打开文档等），就会发生参与。 如果访客打开了对话框或对话流，但未单击提示，则将<b>未记录参与情况</b>。 
    <br>每个访客、每个会话一个参与事件。</td>
  </tr>
   <tr>
    <td style="width:25%"><b>与代理接洽</b></td>
    <td>当访客成功连接到实时聊天代理时发生。
    <br>每个访客、每个会话的代理事件参与人。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>与文档交互</b></td>
    <td>当访客单击文档信息卡中的文档时发生。
    <br>每个访客、每个会话可能存在多个文档交互。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>已实现的目标</b></td>
    <td>当访客实现目标时发生。 <br>每个访客、每个会话可以有多个目标实现的事件。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>已安排的会议</b></td>
    <td>在访客预订与Dynamic Chat代理的会议时发生。
    <br>每个访客、每个会话可以有多个会议预约事件。</td>
  </tr>
</tbody>
</table>

## 注意事项 {#things-to-note}

* [!DNL Dynamic Chat]流程步骤中支持条件
* [!DNL Dynamic Chat]活动可以同步到[[!DNL Marketo Sales Insight]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* 您可以在人员记录的活动日志中查看单个[!DNL Dynamic Chat]活动
