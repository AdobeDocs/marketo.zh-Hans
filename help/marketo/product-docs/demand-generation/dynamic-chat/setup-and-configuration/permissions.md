---
description: 权限 — Marketo文档 — 产品文档
title: 权限
feature: Dynamic Chat
exl-id: 06798ac4-636b-476e-bbb1-498062844406
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 4%

---

# 权限 {#permissions}

在Dynamic Chat中有五个默认配置文件具有预定义权限，您可以编辑它们。 您还可以创建具有自定义权限集的自定义用户档案。 我们来看看这两个。

## 编辑现有权限 {#edit-existing-permissions}

1. 在[Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}中，单击&#x200B;**Dynamic Chat**。

   ![](assets/permissions-1.png)

1. 在&#x200B;**产品配置文件**&#x200B;选项卡中，选择要编辑的配置文件。 在此示例中，我们选择&#x200B;**实时代理**。

   ![](assets/permissions-2.png)

1. 单击&#x200B;**权限**&#x200B;选项卡。

   ![](assets/permissions-3.png)

1. 选择要编辑的配置文件的区域。 在本例中，我们选择“实时聊天”。 单击铅笔图标。

   ![](assets/permissions-4.png)

1. 左侧列出了可用的权限项。 您可以选择逐个添加权限，也可以一次添加所有权限。 单击&#x200B;**+**&#x200B;符号。

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >启用自动包含会将所有权限项添加到包含的列表。 当新的权限项可用时，将自动包含在该产品配置文件中。

1. 单击&#x200B;**保存**。

   ![](assets/permissions-6.png)

您现在可以对任何/所有其他Dynamic Chat区域重复此过程。

![](assets/permissions-7.png)

## 创建配置文件 {#create-a-profile}

1. 在[Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}中，单击&#x200B;**Dynamic Chat**。

   ![](assets/permissions-8.png)

1. 在&#x200B;**产品配置文件**&#x200B;选项卡中，单击&#x200B;**新建配置文件**。

   ![](assets/permissions-9.png)

1. **名称**&#x200B;您的产品配置文件。 （可选）您可以为其提供显示名称和/或描述，并选择在添加/删除用户时通知用户。 完成后单击&#x200B;**保存**。

   ![](assets/permissions-10.png)

1. 您的新配置文件将显示在产品配置文件选项卡中。 选择它。

   ![](assets/permissions-11.png)

1. 现在，对每个所需区域执行上述[部分](#edit-existing-permissions)中的步骤3-6。

## 权限列表 {#list-of-permissions}

在下方，您将找到每个区域的所有可用权限列表。

<table>
<thead>
  <tr>
    <th style="width:25%">Dynamic Chat区域</th>
    <th>权限</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>对话管理</td>
    <td><li>查看对话框</li>
    <li>管理对话框（创建、删除）</li>
    <li>发布对话框</li>
    <li>查看对话流</li>
    <li>管理对话流（创建、删除）</li>
    <li>发布对话流</li></td>
  </tr>
  <tr>
    <td>实时聊天</td>
    <td><li>查看我的对话</li>
    <li>查看所有对话</li>
  </tr>
  <tr>
    <td>会议</td>
    <td><li>管理所有会议</li>
  </tr>
  <tr>
    <td>Analytics</td>
    <td><li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <li>导出报告</li></td>
  </tr>
  <tr>
    <td>代理设置</td>
    <td><li>管理实时聊天可用性</li>
    <li>连接日历</li>
    <li>管理日历可用性</li></td>
  </tr>
  <tr>
    <td>管理员设置</td>
    <td><li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>管理自定义规则（添加、编辑、删除）</li>
    <li>查看帐户列表<b>*</b></li>
    <li>管理帐户（添加、编辑、删除）<b>*</b></li>
    <li>管理聊天机器人设置</li>
    <li>管理对话流设置</li>
    <li>管理隐私和安全性</li>
    <li>管理集成</li>
    <li>管理代理</li>
    <li>查看代理团队<b>*</b></li>
    <li>管理代理团队（添加、编辑、删除）<b>*</b></li></td>
  </tr>
</tbody>
</table>

**&#42;**&#x200B;当前仅适用于Dynamic Prime用户

<p>

## 默认配置文件权限 {#default-profile-permissions}

以下是默认启用的五个默认配置文件和权限。

<table>
<thead>
  <tr>
    <th style="width:25%">轮廓</th>
    <th>默认权限</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>营销用户</td>
    <td><i>对话管理</i>
    <li>查看对话框</li>
    <li>管理对话框（创建、删除）</li>
    <li>发布对话框</li>
    <li>查看对话流</li>
    <li>管理对话流（创建、删除）</li>
    <li>发布对话流</li>
    <br>
    <i>实时聊天</i>
    <li>不适用</li>
    <br>
    <i>会议</i>
    <li>不适用</li>
    <br>
    <i>分析</i>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <br>
    <i>代理设置</i>
    <li>不适用</li>
    <br>
    <i>管理员设置</i>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>查看帐户列表<b>*</b></li>
    <li>查看代理团队<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>实时代理</b></td>
    <td><i>对话管理</i>
    <li>查看对话框</li>
    <li>查看对话流</li>
    <br>
    <i>实时聊天</i>
    <li>查看我的对话</li>
    <br>
    <i>会议</i>
    <li>不适用</li>
    <br>
    <i>分析</i>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <br>
    <i>代理设置</i>
    <li>管理实时聊天可用性</li>
    <li>连接日历</li>
    <li>管理日历可用性</li>
    <br>
    <i>管理员设置</i>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>查看帐户列表<b>*</b></li>
    <li>查看代理团队<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>日历代理</b></td>
    <td><i>对话管理</i>
    <li>查看对话框</li>
    <li>查看对话流</li>
    <br>
    <i>实时聊天</i>
    <li>不适用</li>
    <br>
    <i>会议</i>
    <li>不适用</li>
    <br>
    <i>分析</i>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <br>
    <i>代理设置</i>
    <li>连接日历</li>
    <li>管理日历可用性</li>
    <br>
    <i>管理员设置</i>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>查看帐户列表<b>*</b></li>
    <li>查看代理团队<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>营销管理员</b></td>
    <td><i>对话管理</i>
    <li>查看对话框</li>
    <li>管理对话框（创建、删除）</li>
    <li>发布对话框</li>
    <li>查看对话流</li>
    <li>管理对话流（创建、删除）</li>
    <li>发布对话流</li>
    <br>
    <i>实时聊天</i>
    <li>不适用</li>
    <br>
    <i>会议</i>
    <li>不适用</li>
    <br>
    <i>分析</i>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <li>导出报告</li>
    <br>
    <i>代理设置</i>
    <li>不适用</li>
    <br>
    <i>管理员设置</i>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>管理自定义规则（添加、编辑、删除）</li>
    <li>查看帐户列表<b>*</b></li>
    <li>管理帐户（添加、编辑、删除）<b>*</b></li>
    <li>管理聊天机器人设置</li>
    <li>管理对话流设置</li>
    <li>管理隐私和安全性</li>
    <li>管理集成</li>
    <li>查看代理团队<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>销售管理员</b></td>
    <td><i>对话管理</i>
    <li>查看对话框</li>
    <li>查看对话流</li>
    <br>
    <i>实时聊天</i>
    <li>查看我的对话</li>
    <li>查看所有对话</li>
    <br>
    <i>会议</i>
    <li>管理所有会议</li>
    <br>
    <i>分析</i>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <li>导出报告</li>
    <br>
    <i>代理设置</i>
    <li>管理实时聊天可用性</li>
    <li>连接日历</li>
    <li>管理日历可用性</li>
    <br>
    <i>管理员设置</i>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>管理自定义规则（添加、编辑、删除）</li>
    <li>查看帐户列表<b>*</b></li>
    <li>管理帐户（添加、编辑、删除）<b>*</b></li>
    <li>管理代理</li>
    <li>查看代理团队<b>*</b></li>
    <li>管理代理团队<b>*</b></li>
    </td>
  </tr>
</tbody>
</table>

**&#42;**&#x200B;当前仅适用于Dynamic Prime用户
