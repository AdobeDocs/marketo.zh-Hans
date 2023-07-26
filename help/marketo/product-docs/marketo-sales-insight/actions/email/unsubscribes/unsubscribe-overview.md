---
description: 取消订阅概述 — Marketo文档 — 产品文档
title: 取消订阅概述
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 取消订阅概述 {#unsubscribe-overview}

组织遵守电子邮件隐私法律越来越重要。 为了帮助解决此问题，我们对取消订阅体验进行了一些增强。

* 从Marketo Sales和Salesforce发送的所有电子邮件上都会放置取消订阅链接（这不适用于从Outlook或Gmail发送的自定义电子邮件）
* 管理员可以编辑其整个团队的取消订阅消息
* 取消订阅信息存储在PDV中
* 取消订阅可以手动完成：点击链接、Salesforce同步和退回
* 新的取消订阅链接登陆页面

## 取消订阅链接登陆页面 {#unsubscribe-link-landing-page}

当某人单击您的取消订阅链接时，将会转到取消订阅登陆页面，其中用户可以选择要取消订阅的内容及其原因。

![](assets/unsubscribe-overview-1.png)

此信息将保存到人员详细信息视图以供稍后查看。

## 取消订阅组 {#unsubscribe-group}

在一个位置查看和管理所有已取消订阅的人员。

![](assets/unsubscribe-overview-2.png)

使用搜索栏查找任何已取消订阅的人员。

![](assets/unsubscribe-overview-3.png)

如果您是管理员，则可以转到取消订阅组以按帐户取消订阅进行筛选，并查看已在人员数据库中收集的所有取消订阅。

![](assets/unsubscribe-overview-4.png)

## 取消订阅历史记录卡 {#unsubscribe-history-card}

取消订阅历史记录卡可帮助管理员和用户获取有关其联系人的取消订阅历史记录的上下文信息。 通过转到“人员”选项卡并选择人员来导航到此处。 它位于“人员详细信息”视图中的“关于”选项卡底部。

>[!NOTE]
>
>仅当人员符合以下条件时，才会显示“取消订阅历史记录”卡 _已重新订阅_ 在某个时候。

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>日期</strong></td> 
   <td><p>显示取消订阅/重新订阅的日期。</p></td> 
  </tr> 
  <tr> 
   <td><strong>详细信息</strong></td> 
   <td><p>重新订阅： Sales Connect管理员从联系人记录中手动删除了取消订阅。 它也可能显示与联系人取消订阅原因相关的一些详细信息。</p><p>取消订阅：联系人已取消订阅。</p></td> 
  </tr> 
  <tr> 
   <td><strong>源</strong></td> 
   <td><p>Salesforce同步：取消订阅是由Salesforce中的同步捕获的。</p><p>手动：用户单击取消订阅按钮以选择退出。</p><p>已单击链接：电子邮件收件人已单击取消订阅链接。</p><p>“管理员姓名”：在操作重新订阅联系人时，将显示管理员姓名。 这使用户知道谁删除了取消订阅。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[自定义取消订阅链接消息](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
