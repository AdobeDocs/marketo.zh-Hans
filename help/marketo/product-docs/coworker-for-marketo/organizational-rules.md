---
description: 此处提供描述。
title: 组织规则
source-git-commit: 0949e5193333d56943a5c9a52c1715ecbcb274f3
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%
---
# 组织规则 {#organizational-rules}

组织规则在一个文档中定义了您的营销运营标准和治理要求，该文档在项目创建、活动规划和验证工作流中指导同事。

## 什么是组织规则？ {#what-are-organizational-rules}

组织规则是基于Markdown的配置文档，可捕获您组织的营销活动标准：

* 项目、电子邮件和智能营销活动的命名约定
* 必需的资源和结构（文件夹、令牌、报表）
* 合规性要求（取消订阅链接、UTM参数、排除过滤器）
* 最佳实践（电子邮件设计、智能列表配置）

每个Marketo实例都包含默认的组织规则。 您可以对其进行自定义以反映组织的特定治理需求。

## 使用组织规则的位置 {#where-organizational-rules-are-used}

组织规则跨三种技能为同事提供指导：

| 技能 | 规则的应用方式 |
| --- | --- |
| 生成项目 | 规则指导程序结构的创建、命名和初始设置。 在创建项目之前，同事会在您的简报中标记所有合规性问题。 |
| 计划活动 | 规则告知同事如何根据您的标准构建智能营销活动、过滤器和流程步骤。 |
| 验证程序 | 规则定义了在激活前验证程序时Co-worker执行的检查。 |

## 如何访问和自定义组织规则 {#how-to-access-and-customize-organizational-rules}

1. 在“我的Marketo”中，单击&#x200B;**Marketo Engage同事**&#x200B;图块。
1. 单击齿轮图标。
1. 选择&#x200B;**组织规则**&#x200B;选项卡。
1. 查看默认规则（这些规则中预先填充了营销操作最佳实践）。
1. 编辑规则以匹配组织的：

   * 命名惯例（项目、电子邮件、营销策划）
   * 所需的文件夹结构
   * 必需令牌和字段
   * 法规遵从性和排除标准

1. 进行更改时更新版本号。
1. 保存更改。 所有同事技能都将立即使用您的自定义规则。

## 组织规则结构 {#organizational-rules-structure}

组织规则的格式为带有YAML frontmatter的Markdown：

```markdown
---
name: Your Organization Name — Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## ⚠️ REQUIRED Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## 组织规则的最佳实践 {#best-practices-for-organizational-rules}

* **以默认值开始**：在自定义之前查看默认规则。 它们反映了营销运营的行业最佳实践。
* **使规则重点突出**：仅包含对您的组织重要的要求。 不必要的规则会产生干扰，并且会不必要地降低合规性分数。
* **同时使用自动和手动检查**：

  * 自动检查 — 命名约定、所需文件夹、令牌使用（同事可以验证这些内容）
  * 手动检查 — 电子邮件可视化设计、品牌合规性、活动逻辑（同事会将这些标记为手动审查步骤）

* **灵活平衡严格性**：规则太严格可能会减慢程序创建速度。 过于宽松的规则不会发现重要的合规问题。
* **更新您的规则**：在进行重大更改时更新版本号，以便您的团队知道治理标准已更新。
* **传达更改**：当您更新组织规则时，请让您的营销运营团队知道更改了哪些内容以及更改原因。

## 哪些同事可以验证哪些内容，哪些无法验证 {#what-coworker-can-and-cannot-validate}

协同工作CAN验证（自动检查）：

* 命名惯例与您的模式相匹配
* 存在所需的文件夹结构
* 已设置所需令牌
* 电子邮件具有取消订阅链接和所需的页脚元素
* 外部链接包括UTM参数
* 智能营销活动名称遵循惯例

无法验证同事（需要手动审查）：

* 智能列表筛选器逻辑（API限制 — 您必须手动配置筛选器）
* Smart Campaign流步骤逻辑（API限制 — 您必须手动配置流）
* 电子邮件可视化呈现和响应能力（需要可视化检查）
* 品牌合规性和消息传递基调（需要人为判断）
* 动态内容分段规则（API限制）

当同事遇到无法验证的内容时，它会在工作流中将其标记为手动审阅步骤。

## 合规性评分 {#compliance-scoring}

在使用“验证程序”时，Co-worker将根据以下各项计算相容性分数：

* **通过检查** — 同事已验证合规性并且未找到任何问题
* **失败的检查** — 同事发现违反您的组织规则
* **手动审核步骤** — 需要人工验证的项目（这些不会计入您的分数）

一个程序可以具有100%的合规性，但仍需要手动审查步骤 — 它们被排除在分数计算之外。

## 组织规则自定义示例 {#examples-of-organizational-rules-customization}

**示例1：严格的命名约定**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

如果您的组织要求跨地区和业务部门进行严格管理，请使用此选项。

**示例2：具有所需前缀的灵活命名**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

如果您希望区域代码保持一致，而其他区域代码具有灵活性，请使用此选项。

**示例3：最小规则（侧重于合规性）**

```markdown
# Email Compliance — REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

如果贵组织优先重视合规性而不是命名/结构一致性，请使用此选项。

## 故障排除 {#troubleshooting}

**问：我更新了组织规则，但同事仍在使用旧规则。**

答：更改会立即对新程序和验证生效。 如果您正在处理现有项目，请刷新浏览器或启动新的同事工作流程以查看更新的规则。

**问：能否还原为默认规则？**

答：是的。 转到&#x200B;**设置** > **组织规则**，然后单击&#x200B;**重置为默认值**。 您的自定义规则将被默认规则替换。

**问：我的合规性得分很低，即使项目看起来不错。**

答：检查哪些检查失败。 查看您的组织规则，了解这些规则对于当前工作流是否过于严格，或者您是否需要调整项目以满足您的标准。
