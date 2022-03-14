---
description: 如何修复在连接到Salesforce - Marketo文档 — 产品文档时“我们无法验证您的请求”的问题
title: 如何修复在连接到Salesforce时“我们无法验证您的请求”的问题
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 如何修复在连接到Salesforce时“我们无法验证您的请求”的问题 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在尝试将Sales Insight Actions连接到Salesforce时收到错误消息“We wae unable to authenticate your request”，则可能会限制您对Salesforce API的访问。 请咨询您的Salesforce管理员，确保具备以下条件。

## 在用户权限中启用API {#enable-api-in-user-permissions}

1. 让Salesforce管理员登录SFDC。
1. 选择 **设置**.
1. 选择 **管理用户**.
1. 选择 **用户档案**.
1. 找到ToutApp用户所在的配置文件，然后单击 **编辑**.
1. 向下滚动到 **管理权限** 确保 **已启用API** 复选框。

## 检查Salesforce是否阻止Sales Insight操作连接 {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. 让Salesforce管理员登录到SFDC。
1. 选择 **设置**.
1. 选择 **管理应用程序**.
1. 选择 **连接的应用程序OAuth使用情况**.
1. 确保“销售分析操作”旁边显示“块”。 如果您看到“取消阻止”，请单击按钮以取消阻止Sales Insight Actions对Salesforce的访问。
