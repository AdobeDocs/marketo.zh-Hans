---
unique-page-id: 14352484
description: 如何修复连接到Salesforce - Marketo Docs —— 产品文档时的“We Unable to Authenticate Your Request”
title: 如何在连接到Salesforce时修复“We Unable to Authenticate Your Request”
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# 如何在连接到Salesforce时修复“We Unable to Authenticate Your Request” {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在尝试将Sales Connect连接到Salesforce时收到错误消息“We unable to authenticate your request”，则可能会限制您对Salesforce API的访问。 请咨询您的Salesforce管理员，确保具备以下各项。

## 在用户权限中启用API {#enable-api-in-user-permissions}

1. 让Salesforce管理员登录SFDC。
1. 选择 **设置**。
1. 选择 **管理用户**。
1. 选择 **用户档案**。
1. 找到ToutApp用户所在的用户档案，然后单击“编 **辑”**。
1. 向下滚动到 **“管理权限** ”，并确保 **选中“启用API** ”。

## 检查Salesforce是否阻止Sales Connect连接 {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. 让Salesforce管理员登录到SFDC。
1. 选择 **设置**。
1. 选择“ **管理应用程序**”。
1. 选择“ **已连接的应用程序OAuth使用情况**”。
1. 确保Sales Connect旁边显示“阻止”。 如果看到“取消阻止”，请单击按钮以取消阻止Sales Connect对Salesforce的访问。

