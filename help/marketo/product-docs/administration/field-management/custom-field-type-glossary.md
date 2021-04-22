---
unique-page-id: 2951259
description: 自定义字段类型词汇表 — Marketo Docs — 产品文档
title: 自定义字段类型词汇表
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# 自定义字段类型词汇表{#custom-field-type-glossary}

在Marketo中创建自定义字段时，您有一列表类型可供选择。

>[!PREREQUISITES]
>
>[在Marketo中创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>根据字段类型，过滤器/触发器[运算符](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md)将有所不同。

>[!NOTE]
>
>大多数字段不以字符数最大，而是以字节数最大。 因此，我们无法为每个字段提供确定的字符限制。 异常为&#x200B;**String**，最大为255个字符。

## 布尔值{#boolean}

**示例名称：** 是客户 — 将您的人员标记为客户

**示例值：** True（选中）/ False（未选中）

**运算符**:无

## 货币{#currency}

**示例名称：** 预算 — 存储公司预算的数字值

**示例值：** 100

**运算符**:是，不是介于大于，小于，至少是空的，不是空的

## 日期{#date}

**示例名称：** 续订日期 — 存储客户的续订日期

**示例值：** 8/19/14

**运算符**:is， is not bet，在过去，在过去，在将来，在将来，在时间范围内，在之后，在之前，在之前，在之前或之后，在或之前，是空的，不是空的

## 日期时间{#datetime}

**示例名称：** 创建日期 — 存储创建人员的日期和时间

**示例值：** 8/19/14 2:00

**运算符**:is， is not bet，在过去，在过去，在将来，在将来，在时间范围内，在之后，在之前，在之前，在之前或之后，在或之前，是空的，不是空的

## 电子邮件 {#email}

**示例名称：** 替代电子邮件 — 为您的人员保留替代电子邮件地址（实际上无法向此字段发送电子邮件，如默认电子邮件地址字段，该字段是特殊的）

**示例值：** name@company.com

**运算符**:is、is、not、具有、不具有、包含、不包含的开始、为空、不为空

## 浮点{#float}

**示例名称：** 平均等级点 — 保持人员的平均等级点或具有小数的任何其他数值

**示例值：** 2.47

**运算符**:介于，大于，小于，至少，至多是空的，不是空的

## 公式{#formula}

**示例名称：** 问候语 — 在解决方案中使用此 [特殊字段，根据性](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) 别获得正确的问候

**示例值：检** 查链接的解决方案

## 整数{#integer}

**示例名称：** 员工数 — 存储不需要小数的数字值

**示例值：** 600

**运算符**:是，不是介于大于，小于，至少是空的，不是空的

## 百分比{#percent}

**示例名称：** 可能购买 — 存储一个百分比值（可能是在CRM端计算）

**示例值：** 85%

**运算符**:是，不是介于大于，小于，至少是空的，不是空的

## 电话 {#phone}

**示例名称：** 备用电话 — 为您的人员存储一个额外的电话号码

**示例值：** 650-555-5555

**运算符**:is、is、not、具有、不具有、包含、不包含的开始、为空、不为空

## 分数{#score}

**示例名称：** 行为得分/人口统计得分 — 创建多个得分字段以跟踪不同属性。

**示例值：** 14

**运算符**:是，不是介于大于，小于，至少是空的，不是空的

## 字符串{#string}

**示例名称：** 中间名称 — 存储附加的文本属性

**示例值：** Rose

**运算符**:is、is、not、具有、不具有、包含、不包含的开始、为空、不为空

## 文本区域{#text-area}

**示例名称：** 注释 — 向表单中添加一个注释字段以允许多行文本输入

**示例值：** 此文章非常棒！

**运算符**:is、is、not、具有、不具有、包含、不包含的开始、为空、不为空

## URL {#url}

**示例名称：** 博客 — 创建一个字段以存储个人博客URL

**示例值：** www.myblog.com

**运算符**:is、is、not、具有、不具有、包含、不包含的开始、为空、不为空
