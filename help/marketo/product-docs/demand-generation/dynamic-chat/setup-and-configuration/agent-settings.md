---
description: 代理设置 — Marketo文档 — 产品文档
title: 代理设置
feature: Dynamic Chat
source-git-commit: 9a8f6fe57b585ba0eac6a577bf99e0419d8818a1
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 2%

---

# 代理设置 {#agent-settings}

配置日历并设置会议/实时聊天可用性。

![](assets/agent-settings-1.png)

## 连接日历 {#connect-calendar}

在“日历配置”选项卡中，连接Outlook或Gmail日历，以在聊天机器人中安排约会。

![](assets/agent-settings-2.png)

用户日历连接到Dynamic Chat后，即会添加到队列中，并且网站访客可以使用他们的日历来安排约会。

>[!NOTE]
>
>您可以为每个用户连接一个日历。 如果要在多个日历上接收会议，则必须添加多个用户，并让每个用户连接其日历。

用户还可以在安排用户日历上的约会时自定义发送给访客的邀请的正文。 他们还可以选中底部的复选框，以包含Google会议或Microsoft Teams链接（具体取决于连接的日历）。

![](assets/agent-settings-3.png)

>[!TIP]
>
>使用令牌图标（大括号）可使用人员或公司属性将会议预订确认电子邮件个性化。

### 权限 {#permissions}

使用Outlook配置可授予Dynamic Chat以下权限：

* 完全访问您的日历
* 登录并阅读您的个人资料
* 维护对您已授予其访问权限的数据的访问权限
* 读取您的邮箱设置

使用Google配置可授予Dynamic Chat以下权限：

* 创建、更改或删除日历
* 更新单个日历事件
* 更改您的设置，包括可查看您的活动的人
* 更改与之共享日历的人员
* 访问您的姓名、电子邮件地址、语言首选项和配置文件图片

## 会议预订可用性 {#meeting-booking-availability}

设置您的时区以及每周时间/日期以接收会议预订。

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>会议时长</b></td>
   <td>确定访客在可用会议槽中看到的时间长度。</td>
  </tr> 
  <tr> 
   <td><b>会议之间的缓冲时间</b></td>
   <td>会议后设置为缓冲的时间。 如果您设置30分钟，则没有人能够在您的日历中预定会议结束30分钟之后与您预约会议。</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>您可以在同一天选择多个时间块(例如，星期五从8a到12p _和_ 1p-5p) **+** 在右侧签名。

## 实时聊天可用性 {#live-chat-availability}

设置您的时区以及每周时间/日期以接收实时聊天。

![](assets/agent-settings-5.png)

如果您已登录到应用程序，您将会收到传入聊天的应用内通知。 如果您未登录，将会收到浏览器通知(如果您已 [设置](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"})。

>[!IMPORTANT]
>
>此 [可用性切换](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"} 在Agent收件箱中 **将覆盖** 您在“实时聊天可用性”选项卡中输入的内容。 因此，如果您被安排在1p到5p之间可用，但需要在3p快速休息，则无需更改代理设置。 可用性切换状态将一直保留，直到您手动更改它或到达您的可用性中的下一个时间块为止。

>[!TIP]
>
>您可以在同一天选择多个时间块(例如，星期五从8a到12p _和_ 1p-5p) **+** 在右侧签名。
