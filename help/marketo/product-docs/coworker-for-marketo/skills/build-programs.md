---
description: 使用适用于Marketo Engage的CX Enterprise Coworker通过调整现有模板来构建Marketo程序。 让智能营销活动、计划和资产占位符准备好进行审查和优化。
title: 构建程序
source-git-commit: 148a0ec13abef0658048346f034ff72d9f4012b6
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 0%
---
# 构建程序 {#build-programs}

使用纯语言描述营销活动，并且CX Enterprise Coworker for Marketo Engage会调整现有项目模板以满足您的需求，自动更新电子邮件内容并通过复制模板结构创建其他资源。

贵组织的[组织规则](/help/marketo/product-docs/coworker-for-marketo/organizational-rules.md){target="_blank"}指导适用于Marketo Engage的CX Enterprise Coworker如何在创建过程中构建并验证项目。 这些规则确保新程序与您的命名惯例、所需令牌、文件夹结构和合规性标准保持一致。

>[!PREREQUISITES]
>
>* 若要使用此功能，您必须首先同意[Core Gen-AI条款和补充条款](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}。 有关详细信息，请联系Adobe客户团队（您的客户经理）。
>
>* 您必须有权在Marketo帐户中创建程序，并且必须至少有一个现有的Marketo程序才能用作模板。 模板程序应至少包含一个电子邮件和一个智能营销活动。

## 使用方法 {#how-to-use}

1. 在“我的Marketo”中，单击&#x200B;**CX Enterprise Coworker for Marketo Engage**&#x200B;磁贴。

1. 选择模板项目。 选择与您的活动类型匹配的现有项目（例如，电子邮件、网络研讨会、Nurture）。

1. 在提示窗口中，键入要创建的活动的说明。 根据需要尽可能具体或笼统（您可随时优化）。

1. 适用于Marketo Engage的CX Enterprise Coworker确认其对您的简介的解释，并列出其计划创建的内容。 请在构建之前查看此内容。

1. 确认，然后适用于Marketo Engage的CX Enterprise Coworker会在您的环境中创建项目。

1. 在Marketo中打开新创建的项目并查看结构。

1. 将占位符电子邮件资源替换为您的实际内容。

1. 验证Smart Campaign过滤器和流程步骤是否与预期受众和逻辑匹配。

1. 完成所有手动细化（配置Smart Campaign逻辑、完成过滤器、自定义电子邮件内容）后，运行[验证程序](/help/marketo/product-docs/coworker-for-marketo/skills/validate-programs.md)，确保在激活之前更改符合组织规则。

## 用例 {#use-cases}

**网络研讨会注册计划**：营销活动经理键入“为我们8月份的产品演示创建网络研讨会注册计划”。 发送邀请电子邮件、前一天提醒，以及之后对录制链接的跟进。” CX Enterprise Coworker for Marketo Engage创建了一个项目，该项目包含三个智能营销活动（邀请、提醒、跟进）、每个活动的占位符电子邮件，以及基于活动日期的计划。

**商机得分触发器促销活动**：营销运营专家键入，“构建商机达到50分时触发的项目并将它们发送到MQL智能列表。” 适用于Marketo Engage的CX Enterprise Coworker创建了该项目，其触发活动侦听得分更改，并包含一个流程步骤，将商机添加到MQL列表。

**重新参与培养**：需求一般经理请求通过3封电子邮件重新参与系列来定位未参与90天的潜在客户。 适用于Marketo Engage的CX Enterprise Coworker使用非活动过滤器创建批量营销活动，在三个电子邮件发送步骤之间执行适当的等待步骤，以及在某人重新参与时更新潜在客户状态的流程步骤。

**活动跟进计划**：在贸易展后，经理要求CX Enterprise Coworker的Marketo Engage创建活动后跟进计划，以向与会者发送感谢邮件，并向未显示的注册者发送错过的电子邮件。 适用于Marketo Engage的CX Enterprise Coworker创建两个智能营销活动，每个区段各一个，并使用正确的过滤器和电子邮件占位符。

>[!NOTE]
>
>在上面的每个示例中，Co-worker均克隆现有计划模板（具有基本结构的简单电子邮件或事件计划），并通过复制模板资产并更新其内容来创建其他电子邮件和营销策划。 尽可能调整智能营销活动流程步骤和过滤器，但可能需要手动细化以匹配特定的营销活动逻辑。

## 注意事项 {#things-to-note}

* 清楚地了解活动应该做什么、受众是谁、触发它的操作是什么（或是否为批量发送）以及目标是什么。
* 需要模板选择。 选择至少具有一个电子邮件和一个智能营销活动的模板。 该工具不能用于空模板。
* 电子邮件内容是自动生成的，但Smart Campaign过滤器和流量步骤仍以手动方式执行。 您必须在创建后配置逻辑以匹配营销活动的预期行为。
* 通过复制创建额外资源。 如果您的简要请求显示4封电子邮件，但您的模板只有1封，则该工具会创建3个重复项。 审核它们的一致性情况；它们继承了模板的设计和结构。
* 适用于Marketo Engage的CX Enterprise Coworker无法自动访问您现有的受众列表。 在创建程序后，必须手动配置智能列表筛选器以定向实际区段。
* 具有高级分支逻辑的复杂多步骤程序在创建后可能需要手动细化。
* 如果您的Marketo环境使用命名惯例或文件夹结构，请在简介中指定它们，以便在正确的位置创建程序。
