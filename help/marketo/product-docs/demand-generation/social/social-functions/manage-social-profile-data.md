---
unique-page-id: 2950578
description: 管理社交用户档案数据——营销文档——产品文档
title: 管理社交用户档案数据
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# 管理社交用户档案数据{#manage-social-profile-data}

当某人与Marketo [社交应用](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)交互，或授权其社交网络使用[社交表单填写](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)预填Marketo表单时，Marketo将捕获其社交用户档案中提供的所有数据。 您可以在[“人员详细信息”页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)上视图此信息，或将其添加为智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md)的[自定义视图中的列。

社交表单填写和社交应用程序捕获的字段集略有不同；请参阅以下各节。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请与销售代表联系。

## 通过社交应用程序{#captured-via-social-app}捕获

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!NOTE]
>
>来自社交网络的其他信息会在个人授权后约五分钟出现在“个人详细信息”页面上。

## 来自Twitter:{#from-twitter}

* 名字（从显示名称解析）
* 姓氏（从显示名称解析）
* 用户档案照片URL
* 用户档案页面URL
* 社交触及(关注者数量)

>[!NOTE]
>
>社交应用程序不会获取该人的电子邮件地址。

## 来自Facebook:{#from-facebook}

* 名字
* 姓氏
* 用户档案URL
* 用户档案照片URL
* 性别
* 社交触及（好友数）

### 通过社交表单填写{#captured-via-social-form-fill}捕获

根据网络和用户的隐私设置，将检索以下一个或多个字段：

>[!CAUTION]
>
>社交表单填写捕获的数据将覆盖匹配的字段，除非您[阻止在表单级别](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md)更新这些字段。

## 来自Twitter:{#from-twitter-1}

* 名字（从显示名称解析）
* 姓氏（从显示名称解析）
* 电子邮件

## 来自Facebook:{#from-facebook-1}

* 名字
* 姓氏
* 电子邮件
* 出生日期
* 职务
* 公司

>[!NOTE]
>
>社交表单填写功能仅会在用户在表单中输入电子邮件地址&#x200B;_时捕获电子邮件地址_。 如果需要电子邮件地址，您应[在表单](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)中将其设为必填字段。

>[!MORELIKETHIS]
>
>要从表单中捕获此信息，请启用[社交表单填写](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)。
