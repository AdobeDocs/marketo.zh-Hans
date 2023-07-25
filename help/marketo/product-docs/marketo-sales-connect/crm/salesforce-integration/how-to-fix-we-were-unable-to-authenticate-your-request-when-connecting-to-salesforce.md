---
unique-page-id: 14352484
description: 如何修复在连接到Salesforce时“我们无法验证您的请求” — Marketo文档 — 产品文档
title: 如何修复连接到Salesforce时“我们无法验证您的请求”的问题
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# 如何修复连接到Salesforce时“我们无法验证您的请求”的问题 {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在尝试将Sales Connect连接到Salesforce时收到错误消息“我们无法验证您的请求”，则您对Salesforce API的访问权限可能存在限制。 请咨询您的Salesforce管理员，确保具备以下条件。

## 在用户权限中启用API {#enable-api-in-user-permissions}

1. 让Salesforce管理员登录SFDC。
1. 选择 **设置**.
1. 选择 **管理用户**.
1. 选择 **配置文件**.
1. 查找ToutApp用户位于下的配置文件，然后单击 **编辑**.
1. 向下滚动到 **管理权限** 并确保 **API已启用** 已选中。

## 检查Salesforce是否阻止Sales Connect连接 {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. 让Salesforce管理员登录到SFDC。
1. 选择 **设置**.
1. 选择 **管理应用程序**.
1. 选择 **连接的应用程序OAuth使用情况**.
1. 确保Sales Connect旁边显示“阻止”。 如果您看到“取消阻止”，请单击按钮以取消阻止Sales Connect访问Salesforce。
