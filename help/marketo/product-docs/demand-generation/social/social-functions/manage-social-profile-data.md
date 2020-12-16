---
unique-page-id: 2950578
description: 管理社交用户档案数据——营销文档——产品文档
title: 管理社交用户档案数据
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# 管理社交用户档案数据 {#manage-social-profile-data}

当某人与Marketo社交应用 [程序交互](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)，或授权其社交网络用社交表单填写Marketo表单时， [Marketo将捕获其社交用户档案中提供的所有数据](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)。 您可以在“人员详细信 [息”页面上视图](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)，或将其添加为智能列表 [的自定义视图中的列](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)。

社交表单填写和社交应用程序捕获的字段集略有不同；请参阅以下各节。

>[!NOTE]
>
>**可用性**
>
>并非所有客户都购买了此功能。 有关详细信息，请与销售代表联系。

## 通过社交应用程序捕获 {#captured-via-social-app}

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!NOTE]
>
>来自社交网络的其他信息会在个人授权后约五分钟出现在“个人详细信息”页面上。

## 来自Twitter: {#from-twitter}

* 名字（从显示名称解析）
* 姓氏（从显示名称解析）
* 用户档案照片URL
* 用户档案页面URL
* 社交触及(关注者数量)

>[!NOTE]
>
>社交应用程序不会获取该人的电子邮件地址。

## 来自Facebook: {#from-facebook}

* 名字
* 姓氏
* 用户档案URL
* 用户档案照片URL
* 性别
* 社交触及（好友数）

### 通过社交表单填写获取 {#captured-via-social-form-fill}

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!CAUTION]
>
>社交表单填写捕获的数据将覆盖匹配的字段，除 [非您阻止在表单级别更新这些字段](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)。

## 来自Twitter: {#from-twitter-1}

* 名字（从显示名称解析）
* 姓氏（从显示名称解析）
* 电子邮件

## 来自Facebook: {#from-facebook-1}

* 名字
* 姓氏
* 电子邮件
* 出生日期
* 职务
* 公司

>[!NOTE]
>
>社交表单填写功能仅在 *人员* 在表单中输入时捕获电子邮件地址。 如果需要电子邮件地址，您应 [将其作为表单中的必填字段](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)。

>[!MORELIKETHIS]
>
>要从表单中捕获此信息，请启用社 [交表单填写](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)。

>[!NOTE]
>
>**深潜**
>
>进一步了解如何在Forms深 [入](http://docs.marketo.com/display/docs/forms) 、处理表单。

