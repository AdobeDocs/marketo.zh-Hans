---
description: 在深入了解新的 Marketo Engage 实例之前，您需要完成一些基础步骤以便持续使用。这些步骤包括用户帐户设置、支持管理员设置以及订阅持续的系统更新。
short-description: 完成初始设置步骤后，了解如何建立基础元素以确保持续顺利使用。
title: 用户设置核对清单
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 471a777041361cfebdc8b7139b618ff4dc03e8a8
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 7%

---

# 用户设置核对清单 {#user-setup-checklist}

现在您已完成所有[初始设置步骤](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}，是时候建立一些基础元素以确保顺利进行使用了。 这将为您的Marketo Engage旅程奠定基础，并帮助您充分利用其功能。 让我们开始吧！

>[!NOTE]
>
>您还可以下载此核对清单[以及新实例的最佳实践列表](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)，并随时查看步骤。

## 关于AdobeIdentity Management的Marketo Engage {#marketo-engage-on-adobe-identity-management}

您的新Marketo Engage订阅已载入[AdobeIdentity Management System (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html)。 继续在Adobe Admin Console中进行以下用户管理审查。

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>订阅和Marketo Engage产品管理员</td>
    <td><li>确认您的Adobe组织系统管理员已向您授予Adobe产品管理员角色。</li> 
    <ul>
    <li>请联系Adobe客户团队（您的客户经理）或向<code>marketocares@marketo.com</code>发送电子邮件，以了解贵组织中的哪些人员具有<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console系统管理员</a>权限。</li></ul>
    <li>接受“Marketo Engage产品管理员”邀请以激活您的Adobe ID。 在Adobe Admin Console中分配角色后，将发送<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">欢迎电子邮件</a>。</li></td>
  </tr>
  <tr>
    <td>产品配置文件</td>
    <td><li>将所有所需用户分配给Adobe Admin Console中的Marketo Engage<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">产品配置文件</a>。</li>
    <ul>
    <li>在将用户添加到产品配置文件之前，您无法在“Marketo Engage”&gt;“管理员”&gt;“用户和角色”中分配用户的角色。</li>
    <li>每个订阅都将是一个独立的产品配置文件。 如果将不需要的用户添加到多个产品配置文件（例如，生产和测试沙盒），您必须从所有产品配置文件中删除该用户。 否则，他们仍可以访问Marketo Engage。</li></ul></td>
  </tr>
  <tr>
    <td>用户</td>
    <td><li>创建有关何时<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">创建用户</a>的策略。</li> <li>创建有关何时删除用户的策略。</li>
    <p><img src="assets/note-icon.png" alt="注释图标"> 注意：您必须是系统管理员才能删除用户。
    <li>确定谁应具有<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe的系统管理员和Marketo Engage产品管理员权限。</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">将用户</a>添加到所需的产品配置文件。</li>
    <li>为每个API用例创建一个API用户。</li></td>
  </tr>
  <tr>
    <td>用户管理API（如果适用）</td>
    <td><li>使用<a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe用户管理API</a>来邀请、更新和删除用户。</li>
    <li>使用<a href="https://developer.adobe.com/umapi/">Adobe用户管理API</a>添加或删除角色（例如，管理员、支持管理员、开发人员）。</li>
    </td>
  </tr>
  <tr>
    <td>产品支持管理员</td>
    <td><li>要在Adobe Admin Console</a>中<a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">提交支持工单，您需要让系统管理员为您管理的订阅分配“产品支持管理员”角色。 只有您组织中的系统管理员可以<a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">将您分配给此角色</a>。</li>
    <li>您可能收到了系统管理员的电子邮件，说明您是您Marketo Engage订阅的支持管理员。 如果是这样，请单击电子邮件中的<a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">“开始”</a>以加入组织。</li>
    <li>确定相应的联系人（至少有一个备用联系人），并请求系统管理员相应地分配产品支持管理员角色。</li></td>
  </tr>
</tbody>
</table>

## AdobeIdentity Management设置的Dynamic Chat {#dynamic-chat-on-adobe-identity-management}

若要使用Marketo Engage中的本机对话自动化渠道[Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html)，请按照以下[Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}中的步骤继续设置用户权限。

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>订阅和Dynamic Chat产品管理员（如果适用）</td>
    <td><li>确认您的Adobe组织系统管理员已向您授予Adobe产品管理员角色。</li> 
    <ul><li>请联系Adobe客户团队（您的客户经理）或向<code>marketocares@marketo.com</code>发送电子邮件，以了解贵组织中的哪些人员具有<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console系统管理员</a>权限。</li></ul>
    <li>接受<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">Dynamic Chat的产品管理员</a>邀请。 当您的Marketo Engage实例中启用了Dynamic Chat并且您被指定为系统管理员时，将发送<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">欢迎电子邮件</a>。</li></td>
  </tr>
  <tr>
    <td>产品配置文件</td>
    <td><li>将所有所需用户分配给Adobe Admin Console中的Dynamic Chat产品配置文件。</li> 
    <ul>
    <li>如果将不需要的用户添加到多个产品配置文件，则必须从所有产品配置文件中删除该用户。 否则，他们仍可以访问Dynamic Chat。</li>
    <li>您可以<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">编辑Dynamic Chat</a>中的产品配置文件，并创建一个自定义配置文件，该自定义配置文件具有您的订阅中可用的<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">权限集</a>。</li></td>
  </tr>
  <tr>
    <td>用户</td>
    <td><li>创建有关何时添加和删除聊天用户的策略。</li>
    <li>创建策略以确定谁应具有<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat产品管理员权限。</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">将用户添加到所需的产品配置文件</a>。</li></td>
  </tr>
</tbody>
</table>

## 设置正在进行的系统更新和通信 {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>AdobeMarketo状态更新</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">订阅Adobe Marketo Engage状态更新</a>。</li></td>
  </tr>
  <tr>
    <td>通知</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">订阅管理员通知</a>以了解关键问题，例如智能营销活动中的错误以及CRM同步中发现的严重问题。</li></td>
  </tr>
</tbody>
</table>

<p>

现在您的Marketo Engage帐户已准备就绪，请查看我们的[新Marketo Engage实例最佳实践](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"}部分，以充分利用您的投资并为长期成功做好准备。
