---
unique-page-id: 12983280
description: 发行说明-2017年秋季版- Marketo文档——产品文档
title: 发行说明- 1917年秋季版本
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# 发行说明：秋17 {#release-notes-fall}

1917年秋季版本包含以下功能。 检查您的Marketo版本以了解功能可用性。

请单击标题链接，以视图每个功能的详细文章。 注意：此版本中包含的某些功能没有相关文章。 如果一个主题有多个子标题，则链接会放在该位置。

## 系统可靠性{#system-reliability}

我们对核心Marketo基础架构做了进一步改进，包括更好的顺序、更少的错配，以及改进Munchkin的稳定性。

## SFDC同步性能{#sfdc-sync-performance}

充分利用Marketo和Salesforce之间更丰富、更快速的同步。 需要对帐户或潜在客户进行批量更新的数据更改可以拆分为并行队列以避免积压日志。 事件和任务现在同步速度提高了50%。

## 分析性能改进{#analytics-performance-improvements}

最近的基础架构改进优惠提高了Marketo报告和分析工具中的正常运行时间和稳定性，使您能够更快地构建专门报告。

## [收件人时区](https://docs.marketo.com/x/_xvG) {#recipient-time-zone}

利用此新功能，您现在可以根据当地时区保留和发送电子邮件。 可以将电子邮件和参与项目配置为在收件人的时区中发送，从而无需创建多个项目-发送一次，营销人员将自动保存电子邮件，直到正确的本地时间。 通过在全球范围内使用单一项目来提升电子邮件指标、观察本地实践并节省时间。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>如果您还无法为电子邮件和参与收件人启用项目时区，请不要恐慌！ 我们正在逐步向所有客户启用此功能。

## [按区段查看示例电子邮件](https://docs.marketo.com/x/2IER) {#review-sample-emails-by-segment}

Marketo在发送示例电子邮件以供审阅时有一个新选项来选择区段。 您不再需要手动确定潜在客户属于哪个区段，从而更轻松地向不同区段发送包含动态内容的电子邮件。

## [LinkedIn潜在客户代定制问题](https://docs.marketo.com/x/ngLG) {#linkedin-lead-gen-custom-questions}

自定义LinkedIn潜在客户生成表单以收集自定义潜在客户属性。 现在，您最多可以为每个表单提出三个自定义问题，从单行文本输入或多选题中进行选择，然后映射回“营销人员”潜在客户字段。

## [Slack集成](../../product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

作为新Slack集成的一部分，我们发布了两个功能：

* 系统通知：获取有关Marketo实例中重要事件的Slack通知，如有关当前活动状态和任何需要立即注意的问题的警报。
* 有趣的时刻：当Marketo Insight由销售帐户中的已知个人触发时，可通过Slack通知潜在客户所有者。 通知包括潜在客户信息以及有关销售帐户的详细信息。

## ABM增强{#abm-enhancements}

** [显示无联系人的帐户](https://docs.marketo.com/x/fKCt)**

Marketo ABM现在无需联系即可同步并显示CRM帐户。 包括以前没有销售或营销历史的新帐户，并通过将后续潜在客户匹配到帐户来跟踪进度。

## 内容`<sup>AI </sup>`分析{#contentai-analytics}

** [新的ABM帐户列表过滤器](https://docs.marketo.com/x/1BPG) **

视图并比较ABM客户列表的内容性能，以优化现有内容。 内容`<sup>AI</sup>`显示：

* 查看的内容
* 顶部转换的内容
* 面向营销活动的基于人工智能的建议内容

## Web个性化增强{#web-personalization-enhancements}

** [Web活动令牌](https://docs.marketo.com/x/SwJI)**

令牌现在可用于Web活动。 利用令牌提供个性化消息和内容，提高Web活动的参与度。

![](assets/image2017-11-16-11-3a25-3a7.png)

** [在Web活动编辑器中设计Studio图像](https://docs.marketo.com/x/SwJI)**

在Marketo内跨多个渠道重新使用创意资源和图像，从而节省时间。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 集成{#integration}

** [电子邮件预览API](https://developers.marketo.com/rest-api/assets/emails/)**

您现在可以远程预览Marketo之外的电子邮件，简化电子邮件内容本地化的流程并减少错误。

** [替换HTML API](https://developers.marketo.com/rest-api/assets/emails/)**

开发人员可以远程更新电子邮件资源的HTML内容，使他们能够在单个系统中工作以维护资源。
