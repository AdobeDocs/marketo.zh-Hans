---
unique-page-id: 2951259
description: 自定义字段类型术语表 — Marketo文档 — 产品文档
title: 自定义字段类型术语表
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 1%

---

# 自定义字段类型术语表 {#custom-field-type-glossary}

在Marketo中创建自定义字段时，您有一个可供选择的类型列表。

>[!PREREQUISITES]
>
>[在Marketo中创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>根据字段类型，过滤器/触发器 [运算符](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) 会不同。

>[!NOTE]
>
>大多数字段的最大字符数不是字符数，而是字节数。 因此，我们无法为每个字段提供确定的字符限制。 例外是 **字符串**，最多为255个字符。

## 布尔值 {#boolean}

**示例名称：** 是客户 — 将您的人员标记为客户

**示例值：** True（选中）/ False（未选中）

**运算符**:无

## 货币 {#currency}

**示例名称：** 预算 — 存储公司预算的数字值

**示例值：** 100

**运算符**:is， is not beween than， less than， less than， lass than， last， last mots， is empty，不为空

## 日期 {#date}

**示例名称：** 续订日期 — 存储客户的续订日期

**示例值：** 8/19/14

**运算符**:是，不是过去、过去、将来、以后、过后、前、后、前、前、前、前、后为空

## 日期时间 {#datetime}

**示例名称：** 创建日期 — 存储创建人员的日期和时间

**示例值：** 8/19/14 2点

**运算符**:是，不是过去、过去、将来、以后、过后、前、后、前、前、前、前、后为空

## 电子邮件 {#email}

**示例名称：** 备用电子邮件 — 为您的人员保留备用电子邮件地址（实际上，无法像默认电子邮件地址字段一样，向此字段发送电子邮件，该字段是特殊的）

**示例值：** name@company.com

**运算符**:is， is not， starts with， not starts with， contains， not contains， is empty， not empty

## 浮动 {#float}

**示例名称：** 等级点平均值 — 保持人员的等级点平均值或具有小数的任何其他数值

**示例值：** 2.47

**运算符**:介于、大于、小于、至少至少为空，不为空

## 公式 {#formula}

**示例名称：** 称呼 — 在 [获得正确称呼的解决方案](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) 基于性别

**示例值：** 检查链接的解决方案

## 整数 {#integer}

**示例名称：** 员工数量 — 存储不需要小数的数值

**示例值：** 600

**运算符**:is， is not beween than， less than， less than， lass than， last， last mots， is empty，不为空

## 百分比 {#percent}

**示例名称：** 可能购买 — 存储百分比值（可能在CRM端计算）

**示例值：** 85%

**运算符**:is， is not beween than， less than， less than， lass than， last， last mots， is empty，不为空

## 电话 {#phone}

**示例名称：** 备用电话 — 为您的人员存储额外的电话号码

**示例值：** 650-555-5555

**运算符**:is， is not， starts with， not starts with， contains， not contains， is empty， not empty

## 得分 {#score}

**示例名称：** 行为得分/人口统计得分 — 创建多个得分字段以跟踪不同属性。

**示例值：** 14

**运算符**:is， is not beween than， less than， less than， lass than， last， last mots， is empty，不为空

## 字符串 {#string}

**示例名称：** 中间名称 — 存储附加的文本属性

**示例值：** 罗斯

**运算符**:is， is not， starts with， not starts with， contains， not contains， is empty， not empty

## 文本区域 {#text-area}

**示例名称：** 注释 — 在表单中添加注释字段，以允许多行文本输入

**示例值：** 这篇文章真是太棒了！

**运算符**:is， is not， starts with， not starts with， contains， not contains， is empty， not empty

## URL {#url}

**示例名称：** 博客 — 创建字段以存储个人博客URL

**示例值：** www.myblog.com

**运算符**:is， is not， starts with， not starts with， contains， not contains， is empty， not empty
