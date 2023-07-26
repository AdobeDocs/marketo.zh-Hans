---
unique-page-id: 2950578
description: 管理社交个人资料数据 — Marketo文档 — 产品文档
title: 管理社交个人资料数据
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 5%

---

# 管理社交个人资料数据 {#manage-social-profile-data}

当有人与Marketo交互时 [社交应用程序](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)，或授权其社交网络使用预填充Marketo表单 [社交表单填写](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)， Marketo会捕获其社交个人资料中的所有可用数据。 您可以在 [“人员详细信息”页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)，或将其添加为中的列 [智能列表的自定义视图](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

社交表单填写和社交应用程序捕获的字段集略有不同；请参阅下面每个字段的部分。

>[!AVAILABILITY]
>
>并非所有客户都已购买此功能。 有关详细信息，请与您的销售代表联系。

## 通过社交应用程序捕获 {#captured-via-social-app}

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!NOTE]
>
>社交网络提供的附加信息在人员授权后大约五分钟出现在“人员详细信息”页面上。

## 从Twitter： {#from-twitter}

* 名字（从显示名称解析）
* 姓氏（从显示名称解析）
* 信息配置文件照片URL
* 配置文件页面URL
* 社交范围（关注者数量）

>[!NOTE]
>
>社交应用程序不获取用户的电子邮件地址。

## 从Facebook： {#from-facebook}

* 名
* 姓
* 配置文件URL
* 信息配置文件照片URL
* 性别
* 社交范围（朋友数量）

### 通过社交表单填写捕获 {#captured-via-social-form-fill}

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!CAUTION]
>
>社交表单填充所捕获的数据会覆盖匹配字段，除非您 [在表单级别阻止对这些字段的更新](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## 从Twitter： {#from-twitter-1}

* 名字（从显示名称解析）
* 姓氏（从显示名称解析）
* 电子邮件

## 从Facebook： {#from-facebook-1}

* 名
* 姓
* 电子邮件
* 出生日期
* 职务
* 公司

>[!NOTE]
>
>社交表单填写可捕获电子邮件地址 _仅限_ 如果人员在表单中输入。 如果您需要电子邮件地址，您应： [使其成为表单中的必填字段](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>要从表单中捕获此信息，请启用 [社交表单填写](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
