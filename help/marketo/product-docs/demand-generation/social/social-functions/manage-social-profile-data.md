---
unique-page-id: 2950578
description: 管理社交配置文件数据 — Marketo文档 — 产品文档
title: 管理社交配置文件数据
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 5%

---

# 管理社交配置文件数据 {#manage-social-profile-data}

当某人与Marketo交互时 [社交应用程序](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)，或授权其社交网络使用 [社交表单填写](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)，则Marketo会捕获其社交配置文件中的所有可用数据。 您可以在 [“人员详细信息”页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)，或将其作为列添加到 [智能列表的自定义视图](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

社交表单填写和社交应用程序会捕获一些略有不同的字段；请参阅下面每个章节的部分。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的销售代表。

## 通过社交应用程序捕获 {#captured-via-social-app}

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!NOTE]
>
>社交网络的其他信息会在人员授权后大约五分钟出现在“人员详细信息”页面上。

## 来自Twitter: {#from-twitter}

* 名字（从显示名称中解析）
* 姓氏（从显示名称解析）
* 个人资料照片URL
* 配置文件页面URL
* 社交访问（关注者数量）

>[!NOTE]
>
>社交应用程序不会获取该人员的电子邮件地址。

## 来自Facebook: {#from-facebook}

* 名
* 姓
* 配置文件URL
* 个人资料照片URL
* 性别
* 社交访问（好友数）

### 通过社交表单填写捕获 {#captured-via-social-form-fill}

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!CAUTION]
>
>由社交表单填充捕获的数据将覆盖匹配字段，除非您 [阻止对表单级别的这些字段进行更新](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## 来自Twitter: {#from-twitter-1}

* 名字（从显示名称中解析）
* 姓氏（从显示名称解析）
* 电子邮件

## 来自Facebook: {#from-facebook-1}

* 名
* 姓
* 电子邮件
* 出生日期
* 职务
* 公司

>[!NOTE]
>
>社交表单填写会捕获电子邮件地址 _仅_ 如果人员在表单中输入。 如果您需要电子邮件地址，您应 [在表单中设置必填字段](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>要从表单中捕获此信息，请启用 [社交表单填写](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
