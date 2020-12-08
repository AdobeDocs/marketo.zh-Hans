---
unique-page-id: 45416698
description: 发行说明- 2020年7月- Marketo Docs —— 产品文档
title: 发行说明- 2020年7月
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# 发行说明：2020年7月 {#release-notes-july}

2020年7月版包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!NOTE]
>
>**可用性**
>
>请注意，根据您当前的包装，带有星形(( ![星形)](assets/star-yellow.svg))的物品可能需要购买增值附件。 请联系您的Marketo Engage代表以了解更多信息。

***季度版本*** 2020年7月31日将发布 **以下功能**。

## 管理 {#administration}

* ** [现场管理中的“使用者”导出](https://docs.marketo.com/x/hAK1Ag)**:管理员现在可以将选定字段的所有“使用者”资产链接导出到CSV文件中。 此增强功能可帮助管理员和非管理员清理未使用的字段。 此外，现在还可以在新的浏览器选项卡或窗口中打开资产。

**基于帐户的营 ![销（星型）](assets/star-yellow.svg)

**

* **更新的帐户概要分析UI:**通过在单个屏幕中简化所有步骤，简化“帐户分析”中目标帐户列表的创建。

<br> 

**

***整季度发布***

以下功能在非季度周期中发布，并将在未来几个月中发布。

* **Forms服务：**我们引入了更强的表单字段语法验证功能，并借助新的安全域功能阻止常见机器人模式实现登陆页功能。 阻止程序模式可以减少垃圾邮件表单提交次数并提高数据库质量。
* **增加了资产API URI大小限制**:在删除“_method”参数之前，统一资源标识符(URI)大小限制从8KB增加到65KB。 执行长查询字符串时，此大小限制的增加将使数据更容易传递。 删除“_method”参数是即将进行的安全升级的一部分。

**销售 ![分析（星型）](assets/star-yellow.svg)

**

* **为 [具有非本机Salesforce CRM集成（测试版）的客户启用](https://docs.marketo.com/x/pQK1Ag)Sales Insight*:Marketo Engage客户现在可以使用Sales Insight与非本机Salesforce CRM集成，从而帮助其销售团队了解、排定优先级并与参与度最高的销售线索和机会互动，从而实现智能销售和更快的交易。

**Sales Connect( ![星形)](assets/star-yellow.svg)

**

* **增 [强了销售电话的双方同意：](https://docs.marketo.com/x/dgC1Ag)**管理员现在可以更好地控制电话录制配置。 [确保您遵守](https://docs.marketo.com/x/dAC1Ag) 《双方同意法》，即可启用电话录制。 自动通知正在录制的呼叫，并激活要在呼叫前播放的音频剪辑。

<br> 

## 公告和弃用 {#announcements-deprecations}

* **删除资产API“_method”参数**:2020年9月之后，资产API端点将不再接受“_method”以在查询主体中传递POST参数以绕过URI长度限制。 为了适应需要此参数的请求，资产API的URI限制将从8KB增加到65KB。
* ** [Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:随着Munchkin JavaScript客户端版本159的发布，我们将开始弃用Munchkin Associate Lead方法。 如果被调用，您将收到一条警告消息，指明该方法将在将来的版本中删除。 删除后，该方法将不再有效，尝试使用它将失败。 Marketo Engage最近使用此方法的客户将单独收到其使用通知。
* **支持Internet Explorer**:如之前所宣布的，对Internet Explorer 11的Marketo Engage支 **持将于2020年7月31日结束**。 我们将继续支持Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。

* **天空默认体验**:此版本中将删除管理员或用户将Marketo Sky设置为默认体验的选项，以准备对主用户体验进行更新。 计划在今年晚些时候更新主体验的更多详细信息将在7月提供。 已将Marketo Sky设置为默认体验或已授予Marketo Sky访问权限的用户可以继续从“我的营销人员”主页上的拼贴访问Marketo Sky。
* **EdgeHTML（非Chromium）Microsoft Edge支持**:Marketo Engage在2020年底将不再支持EdgeHTML版本的Microsoft Edge。 从2021年1月1日开始，我们将仅支持最新的Chromium版Microsoft Edge。

