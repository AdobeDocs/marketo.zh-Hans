---
description: 使用对话式流量登录页面 — Marketo文档 — 产品文档
title: 使用对话式流量登陆页面
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# 使用对话式流量登陆页面{#use-a-conversational-flow-landing-page}

将Dynamic Chat对话流直接嵌入到Marketo Engage登录页面，使访客无需填写表单或与聊天机器人交互，即可通过Dynamic Chat安排会议。

>[!PREREQUISITES]
>
>创建简单的 [对话流](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md) 只包含 **会议预订** 卡片。

## 引导式登陆页面 {#guided-landing-pages}

在引导式登陆页面模板中嵌入以下代码： `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

在编辑器中打开引导式登陆页面模板，然后选择对话流占位符。

单击对话流量下拉列表，然后选择在步骤1中创建的CF。

始终将投放类型保留为 **嵌入式**. 单击 **插入**.

您刚刚输入的对话流将在右侧显示为元素。

屏幕快照

>[!NOTE]
>
>此时，对话流将不会显示在主预览窗口中。

## 自由格式登陆页面 {#free-form-landing-pages}

文本


来自STEVE MEETING的注释

引导式lp，模板的新增div id，选择conv flow

自由格式lp，带入图标 — 警告：添加注释 — 当您将cf放在编辑器上时，它不会显示预览（没有占位符） — “您将看不到预览” — 在侧边栏上，他们将看到cf位于页面上 — 引导式lp将其列为元素 — 在说明时使用“此时” — 功能可能会在22日这一周正式启用

