---
description: 早期设置核对清单 — Marketo文档 — 产品文档
title: 早期设置核对清单
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 新领域：早期设置核对清单 {#early-setup-checklist}

介绍文本。

## 关于AdobeIdentity Management的Marketo Engage {#marketo-engage-on-adobe-identity-management}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>订阅和Marketo Engage产品管理员 </td>
    <td><li>确认您的Adobe组织系统管理员已向您授予Adobe产品管理员角色。</li>  
    <ul>
    <li>联系人 <a href="https://helpx.adobe.com/contact.html">Adobe客户关怀</a> 了解贵组织中的人员 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console系统管理员</a> 权限。</li></ul>
    <li>接受“Marketo Engage产品管理员”邀请以激活您的Adobe ID。 此 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">欢迎电子邮件</a> 在Adobe Admin Console中分配角色后发送。</li></td>
  </tr>
  <tr>
    <td>产品配置文件</td>
    <td><li>将所有适当的用户分配给Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">产品配置文件</a> 在Adobe Admin Console中。</li>
    <ul>
    <li>在将用户的Marketo Engage/管理员/用户和角色添加到产品配置文件之前，您无法在这些角色中分配用户角色。</li>
    <li>每个订阅都将是一个独立的产品配置文件。 如果将不需要的用户添加到多个产品配置文件（例如，生产和测试沙盒），您必须从所有产品配置文件中删除该用户。 否则，他们仍可以访问Marketo Engage。</li></ul></td>
  </tr>
  <tr>
    <td>用户</td>
    <td><li>创建策略时间 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">创建用户</a>.</li> <li>创建有关何时删除用户的策略。</li>
    <li>确定谁应该拥有 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe系统管理员和Marketo Engage产品管理员权限。</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">添加用户</a> 到所需的产品配置文件。</li>
    <li>为每个API用例创建一个API用户。</li></td>
  </tr>
  <tr>
    <td>产品支持管理员 </td>
    <td><li>至 <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">在Adobe Admin Console中提交支持工单</a>，您需要由系统管理员为您管理的订阅分配“产品支持管理员”角色。 只有组织中的系统管理员才可以 <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">将您分配给此角色</a>.</li>
    <li>您可能收到了系统管理员的电子邮件，说明您是您Marketo Engage订阅的支持管理员。 如果是这样，请单击 <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">电子邮件中的“开始使用”</a> 加入组织。</li>
    <li>确定相应的联系人（至少有一个备用联系人），并让系统管理员预先相应地分配产品支持管理员角色。</li></td>
  </tr>
</tbody>
</table>

## AdobeIdentity Management设置的Dynamic Chat {#dynamic-chat-on-adobe-identity-management}

文本

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>订阅和Dynamic Chat产品管理员（如果适用） </td>
    <td><li>确认您的Adobe组织系统管理员是否向您授予Adobe产品管理员角色。 联系人 <a href="https://helpx.adobe.com/contact.html">Adobe客户关怀</a> 以了解贵组织中的哪些人员具有控制台中的管理员权限。</li>
    <li>Accept <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">“Dynamic Chat产品管理员”邀请</a>. 此 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">欢迎电子邮件</a> 当您在Marketo Engage实例中启用了Dynamic Chat并且您被指定为系统管理员时，将会发送此事件。</li></td>
  </tr>
  <tr>
    <td>产品配置文件 </td>
    <td><li>在Adobe Admin Console中为Dynamic Chat的产品配置文件分配所有适当的用户。</li> 
    <ul>
    <li>如果将不需要的用户添加到多个产品配置文件，则必须从所有产品配置文件中删除该用户。 否则，他们仍可以访问Dynamic Chat。</li>
    <li>您可以 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">在Dynamic Chat中编辑产品配置文件</a> 并创建具有自定义集的自定义配置文件 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">您的订阅中可用的权限</a>.</li></td>
  </tr>
  <tr>
    <td>用户 </td>
    <td><li>创建有关何时添加和删除聊天用户的策略。</li>
    <li>创建策略以确定谁应该拥有 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">产品管理员权限Adobe Dynamic Chat。</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">将用户添加到所需的产品配置文件</a>.</li></td>
  </tr>
</tbody>
</table>

## 设置正在进行的系统更新和通信

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>AdobeMarketo状态更新 </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">订阅Adobe Marketo Engage状态更新</a>.</li></td>
  </tr>
  <tr>
    <td>通知 </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">订阅管理员通知</a> 以解决Smart Campaigns中的错误、CRM同步中发现的严重问题等关键问题。</li></td>
  </tr>
</tbody>
</table>
