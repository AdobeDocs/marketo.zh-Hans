---
unique-page-id: 2950578
description: 管理社交个人资料数据 — Marketo文档 — 产品文档
title: 管理社交个人资料数据
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# 管理社交个人资料数据 {#manage-social-profile-data}

当有人与Marketo [社交应用程序](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)交互，或授权其社交网络预填充Marketo表单并填充[社交表单填充](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)时，Marketo会捕获其社交配置文件中的所有可用数据。 您可以在[人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)上查看此信息，或将其添加为智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md)的[自定义视图中的列。

>[!IMPORTANT]
>
>2024年7月31日，我们开始了弃用此功能的过程。 无法再创建新资产。 现有资产将继续使用到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

社交表单填写和社交应用程序捕获的字段集略有不同；请参阅下面每个字段的部分。

>[!AVAILABILITY]
>
>并非所有Marketo Engage用户都已购买此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

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
>社交表单填写所捕获的数据将覆盖匹配字段，除非您[阻止表单级别](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md)对这些字段的更新。

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
>社交表单填写捕获电子邮件地址&#x200B;_仅_（如果人员在表单中输入）。 如果需要电子邮件地址，应[将其设为表单中的必填字段](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)。

>[!MORELIKETHIS]
>
>若要从表单中捕获此信息，请启用[社交表单填写](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)。
