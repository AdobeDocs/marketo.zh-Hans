---
unique-page-id: 45416698
description: 发行说明 — 1920年7月 — Marketo Docs — 产品文档
title: 发行说明 — ’20年7月
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---


# 发行说明：’20年7月{#release-notes-july}

’20年7月版包含以下功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>请注意，根据您当前的包，带有星形(![(star)](assets/star-yellow.svg))的项目可能需要购买值加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季_** 度版本2020年7月31日将发 **布以下功能**。

## 管理{#administration}

* **[“使用者”在字段管理中导出](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**:管理员现在可以将选定字段的所有“使用者”资产链接导出到CSV文件中。此增强功能可帮助管理员和非管理员清理未使用的字段。 此外，现在还可以在新的浏览器选项卡或窗口中打开资产。

## 基于帐户的营销{#account-based-marketing}

![（星号）](assets/star-yellow.svg)

* **更新了帐户概要分析的UI**:通过一个屏幕简化所有步骤，简化帐户概要分析中目标帐户列表的创建。

<br> 

**_在整个季度内发布_**

以下功能按非季度周期发布，将在未来几个月发布。

* **Forms服务**:我们引入了更强的表单域语法验证功能，以及使用新的安全域阻止常见机器人模式以实现登陆页功能的能力。阻止机器人模式可减少垃圾邮件表单提交次数并提高数据库质量。

>[!NOTE]
>
>增强表单字段语法验证的完全推出已推迟到我们2021年1月版之后。

* **增加了资产API URI大小限制**:在删除&quot;_method&quot;参数之前，统一资源标识符(URI)大小限制从8KB增加到65KB。当执行长查询字符串时，此大小限制的增加将使数据更容易传递。 删除“_method”参数是即将进行的安全升级的一部分。

## 销售分析{#sales-insight}

![（星号）](assets/star-yellow.svg)

* **[为具有非本机Salesforce CRM集成（测试版）的客户启用](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) Sales Insight**:具有非本机Salesforce CRM集成的Marketo Engage客户现在可以使用Sales Insight帮助其销售团队了解、排定优先级并与参与度最高的销售线索和机会互动，从而实现智能销售并加快交易速度。

## Sales Connect {#sales-connect}

![（星号）](assets/star-yellow.svg)

* **[增强了销售呼叫的双方同意：管](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** 理员现在对呼叫记录配置有更大的控制。[确保您](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) 遵守双方同意法，启用电话记录。自动通知正在录制的呼叫，并激活要在呼叫前播放的音频剪辑。

<br> 

## 公告和弃用{#announcements-deprecations}

* **资产API“_method”参数删除**:在2020年9月之后，资产API端点将不再接受“_method”以在查询体中传递POST参数以绕过URI长度限制。为了适应需要此参数的请求，资产API的URI限制将从8KB增加到65KB。
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:随着Munchkin JavaScript客户端版本159的发布，我们将开始弃用Munchkin Associate潜在客户方法。如果被调用，您将收到一条警告，指示将在将来的版本中删除该方法。 删除后，该方法将不再正常工作，尝试使用它将失败。 最近使用此方法的Marketo Engage客户将单独收到其使用的通知。
* **支持Internet Explorer**:如之前宣布的，对Internet Explorer 11的Marketo Engage支持将于2020 **年7月31日终止**。我们将继续支持Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。
* **天空默认体验**:此版本中将删除管理员或用户将Marketo Sky设置为默认体验的选项，以准备对主用户体验进行更新。计划在今年晚些时候进行的主要体验更新的更多详细信息将在7月发布。 已将Marketo Sky设置为默认体验或已获得对Marketo Sky的访问权限的用户可以继续从“我的营销人员”主页上的拼贴访问Marketo Sky。
* **EdgeHTML（非Chromium）Microsoft Edge支持**:Marketo Engage在2020年底将不再支持EdgeHTML版本的Microsoft Edge。从2021年1月1日开始，我们将仅支持最新的Chromium版Microsoft Edge。
