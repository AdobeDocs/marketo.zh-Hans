---
unique-page-id: 2951884
description: 了解Revenue Explorer中的Opportunity Analysis - Marketo文档 — 产品文档
title: 了解Revenue Explorer中的Opportunity分析
exl-id: 2ef45d3e-7640-4c47-86ae-d7ae45ed1dd4
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 5%

---

# 了解Revenue Explorer中的Opportunity分析 {#understanding-opportunity-analysis-in-revenue-explorer}

Revenue Explorer中的Opportunity Analysis允许您更深入地检查您的机会。 根据任何潜在客户/公司属性（如潜在客户来源、行业或地理位置）对数据进行切片和切块。 根据名称、阶段或概率分析机会的创建和关闭。 了解营销对管道的贡献。

## 示例分析 {#example-analysis}

以下是您可以在Opportunity Analysis区域中创建的一些报告。

1. 营销对所创建机会的影响

   您的营销计划影响了您公司的管道的百分比？ 这份报告会给出答案。 以下饼图显示了营销计划获得的所有机会的数量和机会金额的百分比。

   ![](assets/image2015-7-21-16-3a21-3a4.png)

1. 营销影响机会关闭并获胜。

   此报表按数量及金额显示获得及受营销影响之收入。

   ![](assets/image2015-7-21-16-3a41-3a55.png)

1. 由潜在客户Source关闭的机会

   此报表按销售线索来源划分所有已关闭的销售机会，并让您清楚地了解哪些来源正在工作，哪些没有工作。

   ![](assets/image2015-7-21-10-3a34-3a50.png)

1. 由Source关闭的时间

   此报表演示了关闭商机的平均天数与商机来源之间的关系。

   ![](assets/image2015-7-21-10-3a35-3a3.png)

1. 打开机会和阶段

   此报表显示每个收入周期阶段中打开的商机数量。

   ![](assets/image2015-7-21-10-3a35-3a32.png)

1. 按行业列出的机会数量

   这份报告回答的问题是，“我们每年从某些行业获得的机会是否越来越多？”

   ![](assets/image2015-7-21-10-3a35-3a45.png)

## Opportunity AnalysisDimension和衡量标准 {#opportunity-analysis-dimensions-and-measures}

Opportunity Analysis使您能够访问所有与销售线索、公司和销售机会相关的维度和与销售机会相关的衡量标准。 使用这些机会分析维度和指标回答报告中的具体问题。

1. 公司属性

   | 维度 | 描述 |
   |---|---|
   | 年收入 | 公司年收入 |
   | 城市 | 公司所在的城市 |
   | 国家 | 公司所在的县 |
   | 行业 | 该公司所处的行业 |
   | 公司名称 | 公司名称 |
   | 员工数 | 公司员工人数 |
   | 邮政编码 | 公司的邮政编码 |
   | SIC 代码 | 公司的SIC代码 |
   | 州 | 公司所在的州 |

1. 商机属性

   | 维度 | 描述 |
   |---|---|
   | 已列入阻止列表 | 列入阻止列表铅是的 |
   | 已转换为机会 | 商机已转换为商机 |
   | 电子邮件无效 | 商机是否具有有效的电子邮件地址 |
   | 营销暂停 | 潜在客户是否已从营销电子邮件中停用 |
   | 电子邮件地址 | 商机的电子邮件地址 |
   | 职务 | 潜在客户的工作职位 |
   | 全名 | 商机的全名 |
   | 原始来源类型 | 潜在客户的原始来源类型 |
   | 注册Source类型 | 商机的已注册源类型 |
   | 潜在客户所有者电子邮件地址 | 潜在客户所有者的电子邮件地址 |
   | 潜在客户所有者职务 | 潜在客户所有者的职务 |
   | 潜在客户所有者名称 | 潜在客户所有者的姓名 |
   | 潜在客户来源 | 商机来源 |
   | 潜在客户状态 | 潜在客户状态 |

1. 潜在客户创建时间范围

   | 维度 | 描述 |
   |---|---|
   | 潜在客户创建年份 | 创建商机的年份 |
   | 潜在客户创建的季度 | 创建商机的季度 |
   | 商机创建月份 | 创建商机的月份 |
   | 商机创建周 | 创建潜在客户的周 |
   | 商机创建日期 | 创建商机的日期 |

1. 机会属性

   | 维度 | 描述 |
   |---|---|
   | 机会已关闭 | 机会是否已结束 |
   | 机会预测类别 | 机会预测类别 |
   | 机会名称 | 机会名称 |
   | 机会阶段 | 机会阶段 |
   | 机会类型 | 机会类型 |
   | 赢得的机会 | 此机会是否已结束并获胜 |
   | 受营销影响的机会 | 此标记指示任何潜在客户/联系人是否由任何营销计划获得或在任何营销计划中获得成功。 只考虑定义了期间成本的方案。 |

1. 机会已结束时间范围

   | 维度 | 描述 |
   |---|---|
   | 商机结束年份 | 机会关闭的年份 |
   | 商机已结束的季度 | 机会关闭的季度 |
   | 商机结束月份 | 商机结束的月份 |
   | 商机已关闭周 | 机会关闭的周 |
   | 商机结束日期 | 商机结束的日期 |

1. 机会创建时间范围

   | 维度 | 描述 |
   |---|---|
   | 机会创建年份 | 创建机会的年份 |
   | Opportunity创建的季度 | 创建机会的季度 |
   | 机会创建月份 | 创建机会的月份 |
   | 每周创建的机会数 | 创建机会的周 |
   | 机会创建日期 | 创建机会的日期 |

1. 测量

   | 衡量 | 描述 |
   |---|---|
   | 关闭商机的平均天数 | 关闭机会的平均天数 |
   | 关闭机会的平均天数（丢失） | 丢失机会的平均天数 |
   | 关闭商机的平均天数(Won) | 获胜商机的平均天数 |
   | 所有机会的数量 | 所有机会总数 |
   | 机会数（已关闭） | 已关闭（成功或失败）的机会总数 |
   | 机会数（丢失） | 丢失的机会的总数 |
   | 机会数（未结） | 仍然未完成的机会总数 |
   | 机会数(Won) | 赢得的机会总数 |
   | 机会金额 | 机会总金额。 如果多个销售线索与业务机会关联，则分配金额基于销售线索得分。 |
   | 机会金额（丢失） | 丢失的机会的总金额。 如果多个销售线索与业务机会关联，则分配金额基于销售线索得分。 |
   | 机会金额（未结） | 未结业务机会的总金额。 如果多个销售线索与业务机会关联，则分配金额基于销售线索得分。 |
   | 机会金额(Won) | 成功的机会的总金额。 如果多个销售线索与业务机会关联，则分配金额基于销售线索得分。 |

>[!MORELIKETHIS]
>
>* [创建收入资源管理器报告](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
>* [将字段添加到收入资源管理器报表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/adding-fields-to-a-revenue-explorer-report.md)
>* [订阅Revenue Explorer报表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/subscribe-to-a-revenue-explorer-report.md)
