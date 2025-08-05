---
unique-page-id: 2951259
description: 自定义字段类型术语表 — Marketo文档 — 产品文档
title: 自定义字段类型术语表
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 2%

---

# 自定义字段类型术语表 {#custom-field-type-glossary}

在Marketo中创建自定义字段时，您有一系列类型可供选择。

>[!PREREQUISITES]
>
>[在Marketo中创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>根据字段类型，筛选器/触发器[运算符](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md)将不同。

>[!NOTE]
>
>大多数字段的最大字符数并不是最多，而是字节。 因此，我们无法为每个字段提供明确的字符限制。 异常为&#x200B;**字符串**，其长度上限为255个字符。

## 布尔值 {#boolean}

**示例名称：**&#x200B;是客户 — 将您的人员标记为客户

**示例值：** True （选中） / False （取消选中）

**运算符**：无

## 货币 {#currency}

**示例名称：** Budget — 存储公司预算的编号值

**示例值：** 100

**运算符**： is、is not、between、greater than、less，最多，empty，不为空

## 日期 {#date}

**示例名称：**&#x200B;续订日期 — 存储客户的续订日期

**示例值：** 8/19/14

**运算符**： is、is、not、between、past、before、future、future after、in time frame、after、before、on或after、on或before为空，不为空

## 日期时间 {#datetime}

**示例名称：**&#x200B;创建日期 — 存储创建人员的日期和时间

**示例值：** 8/19/14 2:00

**运算符**： is、is、not、between、past、before、future、future after、in time frame、after、before、on或after、on或before为空，不为空

## 电子邮件 {#email}

**示例名称：**&#x200B;备用电子邮件 — 为您的联系人保留备用电子邮件地址(实际上无法向此字段（如默认电子邮件地址字段，该字段是特殊字段）发送电子邮件)

**示例值：** <name@company.com>

**运算符**： is、is、not、starts with、not starts with、contains、not contains、is empty，不为空

## 浮点值 {#float}

**示例名称：**&#x200B;评级点平均值 — 保留人员的评级点平均值或任何其他具有小数的数值

**示例值：** 2.47

**运算符**： between、greater than、less than、lost、most、empty，不为空

## 公式 {#formula}

**示例名称：**&#x200B;称谓 — 在[解决方案中使用此特殊字段可获得基于性别的正确称谓](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md)

**示例值：**&#x200B;检查链接的解决方案

## 整数 {#integer}

**示例名称：**&#x200B;员工数 — 存储不需要小数的数值

**示例值：** 600

**运算符**： is、is not、between、greater than、less，最多，empty，不为空

## 百分比 {#percent}

**示例名称：**&#x200B;可能购买 — 存储一个百分比值（可能在CRM端计算）

**示例值：** 85%

**运算符**： is、is not、between、greater than、less，最多，empty，不为空

## 电话 {#phone}

**示例名称：**&#x200B;备用电话 — 为你的联系人存储附加电话号码

**示例值：** 650-555-5555

**运算符**： is、is、not、starts with、not starts with、contains、not contains、is empty，不为空

## 得分 {#score}

**示例名称：**&#x200B;行为分数/人口统计分数 — 创建多个分数字段以跟踪不同的属性

**示例值：** 14

**运算符**： is、is not、between、greater than、less，最多，empty，不为空

## 字符串 {#string}

**示例名称：**&#x200B;中间名 — 存储附加文本属性

**示例值：** Rose

**运算符**： is、is、not、starts with、not starts with、contains、not contains、is empty，不为空

## 文本区域 {#text-area}

**示例名称：**&#x200B;注释 — 向表单添加注释字段以允许多行文本输入

**示例值：**&#x200B;这篇文章非常棒！

**运算符**： is、is、not、starts with、not starts with、contains、not contains、is empty，不为空

## URL {#url}

**示例名称：**&#x200B;博客 — 创建字段以存储个人博客URL

**示例值：** &lt;www.myblog.com>

**运算符**： is、is、not、starts with、not starts with、contains、not contains、is empty，不为空
