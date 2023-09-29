---
description: 权限 — Marketo文档 — 产品文档
title: 权限
feature: Dynamic Chat
exl-id: e05308fe-b8b7-40a3-8099-cec937e1961c
source-git-commit: 2dab494bd897bf1030b8c2253831e7626dfe6e67
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 8%

---

# 权限 {#permissions}

有五个默认配置文件具有预定义权限，您可以在Dynamic Chat中编辑。 您还可以创建具有自定义权限集的自定义用户档案。 我们来看看这两个。

## 编辑现有权限 {#edit-existing-permissions}

1. 在 [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}，单击 **Dynamic Chat**.

   ![](assets/permissions-1.png)

1. 在 **产品配置文件** 选项卡，选择要编辑的配置文件。 在本例中，我们选择 **实时代理**.

   ![](assets/permissions-2.png)

1. 单击 **权限** 选项卡。

   ![](assets/permissions-3.png)

1. 选择要编辑的配置文件的区域。 在本例中，我们选择“实时聊天”。 单击铅笔图标。

   ![](assets/permissions-4.png)

1. 左侧列出了可用的权限项。 您可以选择逐个添加权限，也可以一次添加所有权限。 在本例中，只有一个可用，因此我们将添加该一个。 单击 **+** 签名。

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >启用自动包含会将所有权限项添加到包含的列表。 当新的权限项可用时，将自动包含在该产品配置文件中。

1. 单击&#x200B;**保存**。

   ![](assets/permissions-6.png)

您现在可以对任何/所有其他Dynamic Chat区域重复此过程。

![](assets/permissions-7.png)

## 创建配置文件 {#create-a-profile}

1. 在 [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}，单击 **Dynamic Chat**.

   ![](assets/permissions-8.png)

1. 在 **产品配置文件** 选项卡，单击 **新建配置文件**.

   ![](assets/permissions-9.png)

1. **名称** 您的产品配置文件。 （可选）您可以为其提供显示名称和/或描述，并选择在添加/删除用户时通知用户。 单击 **保存** 完成时。

   ![](assets/permissions-10.png)

1. 您的新配置文件将显示在产品配置文件选项卡中。 选择它。

   ![](assets/permissions-11.png)

1. 现在，请按照中的步骤3-6操作 [上一节](#edit-existing-permissions) 适用于每个所需区域。

## 权限列表 {#list-of-permissions}

在下方，您将找到每个区域的所有可用权限列表。

<table>
<thead>
  <tr>
    <th style="width:30%">Dynamic Chat区域</th>
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
    <li>查看帐户列表 <b>*</b></li>
    <li>管理帐户（添加、编辑、删除） <b>*</b></li>
    <li>管理聊天机器人设置</li>
    <li>管理对话流设置</li>
    <li>管理隐私和安全性</li>
    <li>管理集成</li>
    <li>管理代理</li>
    <li>查看代理团队 <b>*</b></li>
    <li>管理代理团队（添加、编辑、删除） <b>*</b></li></td>
  </tr>
</tbody>
</table>

**&#42;** 目前仅适用于Dynamic Prime用户

<p>

## 默认配置文件权限 {#default-profile-permissions}

以下是默认启用的五个默认配置文件和权限。

<table>
<thead>
  <tr>
    <th style="width:30%">用户档案</th>
    <th>默认权限</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>营销用户</td>
    <td><i>对话管理</i>
    <p>
    <li>查看对话框</li>
    <li>管理对话框（创建、删除）</li>
    <li>发布对话框</li>
    <li>查看对话流</li>
    <li>管理对话流（创建、删除）</li>
    <li>发布对话流</li>
    <p>
    <p><i>实时聊天</i></p>
    <li>不适用</li>
    <p>
    <p><i>会议</i></p>
    <li>不适用</li>
    <p>
    <p><i>Analytics</i></p>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <p>
    <p><i>代理设置</i></p>
    <li>不适用</li>
    <p>
    <p><i>管理员设置</i></p>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>查看帐户列表 <b>*</b></li>
    <li>查看代理团队 <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>实时代理</b></td>
    <td><i>对话管理</i>
    <p>
    <li>查看对话框</li>
    <li>查看对话流</li>
    <p>
    <p><i>实时聊天</i></p>
    <li>查看我的对话</li>
    <p>
    <p><i>会议</i></p>
    <li>不适用</li>
    <p>
    <p><i>Analytics</i></p>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <p>
    <p><i>代理设置</i></p>
    <li>管理实时聊天可用性</li>
    <li>连接日历</li>
    <li>管理日历可用性</li>
    <p>
    <p><i>管理员设置</i></p>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>查看帐户列表 <b>*</b></li>
    <li>查看代理团队 <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>日历代理</b></td>
    <td><i>对话管理</i>
    <p>
    <li>查看对话框</li>
    <li>查看对话流</li>
    <p>
    <p><i>实时聊天</i></p>
    <li>不适用</li>
    <p>
    <p><i>会议</i></p>
    <li>不适用</li>
    <p>
    <p><i>Analytics</i></p>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <p>
    <p><i>代理设置</i></p>
    <li>连接日历</li>
    <li>管理日历可用性</li>
    <p>
    <p><i>管理员设置</i></p>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>查看帐户列表 <b>*</b></li>
    <li>查看代理团队 <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>营销管理员</b></td>
    <td><i>对话管理</i>
    <p>
    <li>查看对话框</li>
    <li>管理对话框（创建、删除）</li>
    <li>发布对话框</li>
    <li>查看对话流</li>
    <li>管理对话流（创建、删除）</li>
    <li>发布对话流</li>
    <p>
    <p><i>实时聊天</i></p>
    <li>不适用</li>
    <p>
    <p><i>会议</i></p>
    <li>不适用</li>
    <p>
    <p><i>Analytics</i></p>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <li>导出报告</li>
    <p>
    <p><i>代理设置</i></p>
    <li>不适用</li>
    <p>
    <p><i>管理员设置</i></p>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>管理自定义规则（添加、编辑、删除）</li>
    <li>查看帐户列表 <b>*</b></li>
    <li>管理帐户（添加、编辑、删除） <b>*</b></li>
    <li>管理聊天机器人设置</li>
    <li>管理对话流设置</li>
    <li>管理隐私和安全性</li>
    <li>管理集成</li>
    <li>查看代理团队 <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>销售管理员</b></td>
    <td><i>对话管理</i>
    <p>
    <li>查看对话框</li>
    <li>查看对话流</li>
    <p>
    <p><i>实时聊天</i></p>
    <li>查看我的对话</li>
    <li>查看所有对话</li>
    <p>
    <p><i>会议</i></p>
    <li>管理所有会议</li>
    <p>
    <p><i>Analytics</i></p>
    <li>查看全局性能报表</li>
    <li>查看实时聊天报告</li>
    <li>查看会议报告</li>
    <li>导出报告</li>
    <p>
    <p><i>代理设置</i></p>
    <li>管理实时聊天可用性</li>
    <li>连接日历</li>
    <li>管理日历可用性</li>
    <p>
    <p><i>管理员设置</i></p>
    <li>查看循环调度程序</li>
    <li>查看自定义规则</li>
    <li>管理自定义规则（添加、编辑、删除）</li>
    <li>查看帐户列表 <b>*</b></li>
    <li>管理帐户（添加、编辑、删除） <b>*</b></li>
    <li>管理代理</li>
    <li>查看代理团队 <b>*</b></li>
    <li>管理代理团队 <b>*</b></li>
    </td>
  </tr>
</tbody>
</table>

**&#42;** 目前仅适用于Dynamic Prime用户
