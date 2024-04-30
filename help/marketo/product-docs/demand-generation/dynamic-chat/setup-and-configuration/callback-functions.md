---
description: 回调函数 — Marketo文档 — 产品文档
title: 回调函数
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 30deeb59cd70b42af38cd1e047833394f9341a5c
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 3%

---

# 回调函数 {#callback-functions}

您可以使用Dynamic Chat小组件回调函数将对话事件发送到任何第三方平台。

## 快速入门 {#getting-started}

此事件表示Dynamic Chat构件已准备就绪，可在网页中加载与Dynamic Chat相关的所有脚本时触发。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
});
```

## 对话事件 {#conversation-events}

这些事件与针对特定访客的特定页面的对话相关。

### 已触发对话

解析针对网站访客的对话（例如，对话框），并向他们显示聊天机器人。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 

    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
// code here will execute when chatbot is loaded for a visitor 
   });
});
```

### 已参与对话 {#conversation-engaged}

访客参与了（例如，提供了他们的第一个响应）聊天机器人。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when visitor engages with chatbot 
    });
});
```

### 对话已完成 {#conversation-completed}

访客已到达对话的结尾。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when conversation is completed 
    });
});
```

### 对话已关闭

访客在到达结尾之前已关闭对话。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when conversation is closed 
    });
});
```

事件中的“event”参数是一个包含与对话相关的元数据的对象。 您可以按event.data访问元数据

以下是您可以访问的一些关键元数据值：

<table>
<thead>
  <tr>
    <th style="width:75%">元数据</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>对话名称</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>对话ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会话类型（对话框/会话流）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI类型（弹出窗口/聊天机器人/内联）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>会话ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## 访客输入事件

当参与对话的访客提供其联系信息（例如，电话号码或电子邮件地址）时，将触发这些事件。 以下是属于此类别的事件。

### 电话号码 {#phone-number}

当访客在对话期间提供电话号码时，将触发此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
  // code here will execute when a visitor provides their phone number 
    }); 
}); 
```

### 电子邮件ID {#email-id}

当访客在对话期间提供其电子邮件地址时，将触发此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
});
```

事件中的“event”参数是一个包含与对话相关的元数据的对象。 您可以按event.data访问元数据

以下是您可以访问的一些关键元数据值。

<table>
<thead>
  <tr>
    <th style="width:75%">元数据</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>对话名称</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>对话ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会话类型（对话框/会话流）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI类型（弹出窗口/聊天机器人/内联）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>会话ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## 会议预订事件 {#meeting-booking-events}

当访客与您的业务代表预约会议时，将触发这些事件。

以下是属于此类别的事件。

### 已预订的会议 {#meeting-booked}

当访客在座席日历上预订会议时，将触发此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
});
```

事件中的“event”参数是一个包含与对话相关的元数据的对象。 您可以按event.data访问元数据

以下是您可以访问的一些关键元数据值。

<table>
<thead>
  <tr>
    <th style="width:75%">元数据</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>对话名称</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>对话ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会话类型（对话框/会话流）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI类型（弹出窗口/聊天机器人/内联）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>会话ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>代理名称</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>代理ID</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>会议信息</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## 实时聊天活动 {#live-chat-events}

当访客在与聊天机器人互动期间与实时代理连接时，将触发这些事件。

以下是属于此类别的事件。

### 已请求实时聊天 {#live-chat-requested}

当访客选择与实时代理聊天并解析可用代理时，将触发此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests for live chat 
    }); 
});
```

### 实时聊天已启动 {#live-chat-initiated}

当访客选择与实时座席聊天且座席接受聊天时，将触发此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepted the chat 
    }); 
});
```

### 实时聊天已结束 {#live-chat-ended}

此事件在访客与实时代理之间的对话结束时触发。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
});
```

### 实时聊天超时 {#live-chat-timeout}

当实时聊天对话因访客停止响应或放弃而超时时，将触发此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandoned live chat 
    }); 
});
```

事件中的“event”参数是一个包含与对话相关的元数据的对象。 您可以按event.data访问元数据

以下是您可以访问的一些关键元数据值。

<table>
<thead>
  <tr>
    <th style="width:75%">元数据</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>对话名称</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>对话ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会话类型（对话框/会话流）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI类型（弹出窗口/聊天机器人/内联）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>会话ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>代理名称</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>代理ID</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

如果您希望将任意这些事件发送到Adobe Analytics或Google Analytics等第三方平台，则需要在这些Dynamic Chat事件中添加各自的跟踪调用。 它类似于下面的示例。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // Enter Adobe Analytics or Google Analytics function here 
    ga('send', 'event', { 
      eventCategory: Dynamic Chat Conversations', 
      eventAction: 'Conversation Triggered', 
      eventLabel: event.data.payload.id, 
    }); 
    }); 
});
```
