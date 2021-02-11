---
unique-page-id: 14352484
description: 如何修复连接到Salesforce - Marketo Docs —— 产品文档时的“We Unable to Authenticate Your Request”
title: 如何在连接到Salesforce时修复“We Unable to Authenticate Your Request”
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# 如何在连接到Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}时修复“We We Unable to Authenticate Your Request”

如果您在尝试将Sales Connect连接到Salesforce时收到错误消息“We unable to authenticate your request”，则可能会限制您对Salesforce API的访问。 请咨询您的Salesforce管理员，确保具备以下各项。

## 在用户权限{#enable-api-in-user-permissions}中启用API

1. 让Salesforce管理员登录SFDC。
1. 选择&#x200B;**设置**。
1. 选择&#x200B;**管理用户**。
1. 选择&#x200B;**用户档案**。
1. 找到ToutApp用户所在的用户档案，然后单击&#x200B;**编辑**。
1. 向下滚动到&#x200B;**管理权限**，并确保选中“已启用API **”。**

## 检查Salesforce是否阻止Sales Connect连接{#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. 让Salesforce管理员登录到SFDC。
1. 选择&#x200B;**设置**。
1. 选择&#x200B;**管理应用程序**。
1. 选择&#x200B;**连接的应用程序OAuth使用情况**。
1. 确保Sales Connect旁边显示“阻止”。 如果看到“取消阻止”，请单击按钮以取消阻止Sales Connect对Salesforce的访问。
