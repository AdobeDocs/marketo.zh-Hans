---
description: 取消订阅概述 — Marketo文档 — 产品文档
title: 取消订阅概述
hide: true
hidefromtoc: true
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 取消订阅概述 {#unsubscribe-overview}

对于组织来说，遵守电子邮件隐私法变得越来越重要。 为此，我们对取消订阅体验进行了一些增强。

* 取消订阅链接会放置在从Marketo Sales and Salesforce发送的所有电子邮件中（这不适用于从Outlook或Gmail发送的自定义电子邮件）
* 管理员可以编辑其整个团队的取消订阅消息传送
* 取消订阅信息存储在PDV中
* 取消订阅可以手动完成：点击了链接、Salesforce同步和跳出
* 新的取消订阅链接登陆页面

## 取消订阅链接登陆页面 {#unsubscribe-link-landing-page}

当用户单击您的取消订阅链接时，他们将被转到取消订阅登陆页面，从中可以选择他们希望取消订阅的内容以及取消订阅的原因。

![](assets/unsubscribe-overview-1.png)

此信息将保存到“人员详细信息”视图，以供日后查看。

## 取消订阅组 {#unsubscribe-group}

在一个位置查看和管理所有未订阅的人员。

![](assets/unsubscribe-overview-2.png)

使用搜索栏查找任何未订阅的人员。

![](assets/unsubscribe-overview-3.png)

如果您是管理员，则可以转到取消订阅组以按帐户取消订阅进行过滤，并查看在人员数据库中收集的所有取消订阅。

![](assets/unsubscribe-overview-4.png)

## 取消订阅历史记录卡 {#unsubscribe-history-card}

取消订阅历史记录卡可帮助管理员和用户获取其联系人取消订阅历史记录的上下文信息。 通过转到人员选项卡并选择人员，可在此处导航。 它位于“人员详细信息”视图中“关于”选项卡的底部。

>[!NOTE]
>
>只有当用户拥有 _已订阅_ 在某个时候。

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>日期</strong></td> 
   <td><p>显示取消订阅/重新订阅的发生日期。</p></td> 
  </tr> 
  <tr> 
   <td><strong>详细信息</strong></td> 
   <td><p>重新订阅：Sales Connect管理员手动从联系记录中删除了取消订阅。 它还可能显示与联系人取消订阅的原因相关的一些详细信息。</p><p>取消订阅：联系人已退订。</p></td> 
  </tr> 
  <tr> 
   <td><strong>源</strong></td> 
   <td><p>Salesforce同步：已通过与Salesforce的同步捕获取消订阅。</p><p>手动：用户单击取消订阅按钮以选择退出。</p><p>点击的链接：电子邮件的收件人已单击取消订阅链接。</p><p>"管理员名称":管理员的姓名将显示操作何时为联系人重新订阅。 这可让用户知道是谁删除了取消订阅。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[自定义取消订阅链接消息](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
