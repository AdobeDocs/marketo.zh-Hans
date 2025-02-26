---
description: Adobe IMS疑难解答指南 — Marketo文档 — 产品文档
title: Adobe IMS疑难解答指南
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e5c6ac7df0f8f6e7726de1ced598d390a6cf1deb
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Adobe IMS疑难解答指南 {#adobe-ims-troubleshooting-guide}

在IMS用户迁移过程中，将为每个要迁移的Adobe用户创建一个Marketo Engage用户。 有时不会创建它（由于各种原因，与Active Directory中的用户记录或电子邮件地址问题有关）。 发生这种情况时，Marketo Engage管理员将在自迁移控制台的用户迁移状态字段中看到原因。 请参阅以下内容，了解如何解决各种Adobe用户创建问题。

## 错误消息 {#error-messages}

* <a href="#not-in-directory">不在目录</a>中
* <a href="#gmail-invalid-character">Gmail无效字符</a>
* <a href="#inactive-user">非活动用户</a>
* <a href="#not-in-domain">不在域</a>中
* <a href="#create-failure">创建失败</a>
* <a href="#type2e-user-failure">Type2e用户失败</a>

<table>
<thead>
  <tr>
    <th style="width:20%">错误消息</th>
    <th style="width:40%">根本原因</th>
    <th style="width:40%">分辨率</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">不在目录中</a></i></td>
    <td>Active Directory (AD)中不存在该用户。 对于已启用AD同步且具有SSO的任何组织，只允许通过身份提供程序(IdP)创建用户。 因此，在用户迁移期间无法通过Admin Console添加用户。</td>
    <td>迁移 — 需要将用户添加到具有适当权限的Active Directory中。 Marketo管理员可从迁移控制台为此用户重新运行用户迁移。 
    <br>不迁移 — Marketo管理员在迁移控制台中跳过用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击该图标以结束用户迁移过程。</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Gmail无效字符</a></i></td>
    <td>根据Adobe的安全策略，“。” 仅在Gmail域的电子邮件地址中不允许使用和“+”符号  
    <br>非Gmail域电子邮件地址中允许使用两个特殊字符。 </td>
    <td>迁移 — 电子邮件地址需要在Marketo Engage中更新，以符合Adobe的安全策略。 Marketo管理员可从迁移控制台为此用户重新运行用户迁移。<br>不迁移 — Marketo管理员在迁移控制台中跳过用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击该图标以结束用户迁移过程。</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">非活动用户</a></i></td>
    <td>已启用AD同步，并且用户的联合帐户存在，但处于非活动/禁用状态。</td>
    <td>迁移 — 需要恢复用户的状态和适当的权限。 Marketo管理员可从迁移控制台为此用户重新运行用户迁移。
    <br>不迁移 — Marketo管理员在迁移控制台中跳过用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击该图标以结束用户迁移过程。</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">不在域中</a></i></td>
    <td>Admin Console中已启用域实施，但用户电子邮件地址的域不是允许的域之一。 
    <br>域实施策略在目录级别设置。</td>
    <td>迁移 — 电子邮件地址需要在Marketo Engage中更新以符合域实施策略，或者系统管理员可以<a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    将域移动到另一个域强制(DE)禁用的目录</a>或<a href="https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html">创建一个不在DE策略下的新目录</a>。 Marketo管理员可从迁移控制台为此用户重新运行用户迁移。 <br>不迁移 — Marketo管理员在迁移控制台中跳过用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击该图标以结束用户迁移过程。</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">创建失败</a></i></td>
    <td>后端存在各种原因。</td>
    <td>请提交支持案例。</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Type2e用户失败</a></i></td>
    <td>后端存在各种原因。</td>
    <td>请提交支持案例。</td>
  </tr>
</tbody>
</table>
