---
description: Dynamic Chat 发行说明 - Marketo Docs - 产品文档
title: Dynamic Chat 发行说明
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 342d52439a21668a3bf94e5149710b20e4ddb83f
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 3%

---

# TEMPDynamic Chat发行说明 {#dynamic-chat-release}

## 2024年9/10月版 {#august-release}

### 增强实时聊天分析 {#enhanced-live-chat-analytics}

对Analytics功能板进行了一些增强，包括：

* 请求的实时聊天总数：“与代理聊天”请求的访客数

* 已连接的实时聊天总数：已连接的访客数与“与代理聊天”请求的总数

* 错过的实时聊天请求总数：“与代理聊天”的无人参与访客数与请求总数

* 以分钟为单位的平均聊天时长：分析访客与代理之间的“平均聊天时长”

* 平均座席响应时间（以秒为单位）：分析座席响应其实时聊天问答的“平均所用时间”

* 每日仪表板：实时聊天请求连接成功，实时聊天请求丢失，排序和筛选最近的实时聊天活动

屏幕快照

### 对话得分

根据潜在客户聊天交互的质量对其量化并将该指标用作Marketo Engage智能营销活动中的触发器/过滤器。 在下列活动中使用新属性&#x200B;_对话分数_：

* 参与对话
* 已参与会话流
* 与代理接洽

**注意事项：**

* 得分值将介于0、1、2、3之间（默认值为null）

* 完成或删除对话后，在活动中保存评分值并发布无法编辑的帖子????????????????????????????????（这是什么意思）

* 设置得分：

   * 在代理收件箱中 — 在实时聊天期间，代理能够更新或设置对话的分数，该分数存储在对话活动中

   * 在流设计器中 — 在目标卡片中，用户能够更新或设置对话的分数

屏幕快照

屏幕快照

屏幕快照

### 新的潜在客户创建逻辑 {#new-lead-creation-logic}

如果某个商机使用电子邮件`abc@test.com`填写表单并作为xyz进行Cookie，然后使用电子邮件`def@test.com`填写同一表单，则会创建新商机，但Cookie xyz会与新商机关联并从商机`abc@test.com`中删除。

从那时起，`abc@test.com`将成为无Cookie的潜在客户。 匿名线索??

因此，当具有Cookie abc的访客登陆页面并提供电子邮件ID为`abc@p.com`时：

表
