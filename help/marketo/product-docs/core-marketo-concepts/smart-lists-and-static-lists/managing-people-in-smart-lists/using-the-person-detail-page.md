---
unique-page-id: 2953415
description: 使用人员详细信息页面 — Marketo Docs — 产品文档
title: 使用“人员详细信息”页
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---


# 使用“人员详细信息”页{#using-the-person-detail-page}

人员详细信息页面包含Marketo了解的有关人员的所有信息。 您可以直接从此页编辑数据。

## “人员详细信息”页{#getting-to-person-detail-page}

有很多方法可以打开特定的人。 例如：

* 在&#x200B;**Database**&#x200B;中，可以在“快速查找”中搜索
* 任何智能&#x200B;**列表**&#x200B;或列表
* **** 项目
* **视图** 活动智能活动
* 某些&#x200B;**报告**

   <br> 

1. 多次单击任何人，或单击左侧的ID。

   ![](assets/one-1.png)

1. 这将打开人物详细信息屏幕。

   ![](assets/two-5.png)

## 页面组织 — Salesforce {#page-organization-salesforce}

人员信息分为以下选项卡：

| 选项卡 | 说明 |
|---|---|
| 信息 | 联系人信息和自定义字段。 |
| 公司信息 | 人员的公司信息和地址。 |
| 机会信息 | 业务机会信息已从Salesforce同步。 |
| SFDC潜在客户字段 | 内置的Salesforce字段。 |
| SFDC自定义字段 | 自定义Salesforce字段。 |
| 活动日志 | 所有与此人相关的活动。 |

## 页面组织 — Microsoft Dynamics {#page-organization-microsoft-dynamics}

| 选项卡 | 说明 |
|---|---|
| 信息 | 联系人信息和自定义字段。 |
| 公司信息 | 人员的公司信息和地址。 |
| 机会信息 | 从Microsoft同步的业务机会信息。 |
| Microsoft自定义字段 | 自定义Microsoft字段。 |
| Microsoft潜在客户字段 | 内置的Microsoft字段。 |
| 活动日志 | 所有与此人相关的活动。 |

>[!NOTE]
>
>您还可以看到未与CRM同步的实例通过API](http://developers.marketo.com/rest-api/lead-database/opportunities/)插入的业务机会信息[。

## 编辑字段{#editing-a-field}

许多字段都可编辑。 要更新人员的信息，请键入新值，然后单击字段外部以进行保存。

![](assets/image2015-2-27-11-3a14-3a2.png)

## CRM同步{#marketo-default-fields-prior-to-crm-sync}之前的Marketo默认字段

|  |  |  |  |  |
|---|---|---|---|---|
| 地址 | 年收入 | 匿名IP | 帐单地址 | 比利尼城 |
| 帐单国 | 帐单邮政编码 | 帐单状态 | 城市 | 公司名称 |
| 国家/地区 | 创建时间 | 出生日期 | 部门 | 不拨叫 |
| 不致电原因 | 不致电原因 | 电子邮件地址 | 电子邮件无效 | 电子邮件无效原因 |
| 外部公司ID | 外部销售人员ID | 传真号码 | 名字 | 全名 |
| 行业 | 推断城市 | 推断公司 | 推断国家 | 推断的都市区 |
| 推断出的电话区号 | 推断的邮政编码 | 推断的州 | 是匿名 | 客户 |
| 是合作伙伴 | 职务 | 姓氏 | 评级 | 得分 |
| 人员来源 | 状态 | 主电话 | Marketo Social Facebook显示名称 | Marketo Social Facebook Id |
| Marketo Social Facebook照片URL | Marketo Social Facebook用户档案URL | Marketo Social Facebook访问 | Marketo Social Facebook引荐登记 | Marketo Social Facebook引荐的访问 |
| Marketo社会性别 | Marketo Social上次引荐登记 | Marketo Social上次引荐的访问 | Marketo Social LinkedIn显示名称 | Marketo Social LinkedIn Id |
| Marketo Social LinkedIn照片URL | Marketo Social LinkedIn用户档案URL | Marketo Social LinkedIn触及范围 | Marketo Social LinkedIn引荐登记 | Marketo Social LinkedIn引荐访问 |
| Marketo Social联合ID | Marketo Social引荐登记总数 | Marketo Social引荐访问总数 | Marketo社交Twitter显示名称 | Marketo社交Twitter Id |
| Marketo社交Twitter照片URL | Marketo社交Twitter用户档案URL | Marketo社交Twitter访问 | Marketo Social Twitter引荐登记 | Marketo Social Twitter引荐的访问 |
| 中间名 | 手机号码 | 员工人数 | 电话号码 | 邮政编码 |
| 优先级 | 相对得分 | 角色 | 问候 | SIC代码 |
| 网站 | 州 | 取消订阅 | 取消订阅原因 | 更新日期 |
| 紧急 | 网站 |  |  |  |

>[!NOTE]
>
>某些字段&#x200B;_不_&#x200B;可编辑：
>
>* 活动日志
>* 公司信息
>* SFDC联系人的机会
>* 特定于Marketo的特定字段，如“创建日期”和“原始源类型”。

>
>
了解有关[系统管理字段](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md)的更多信息。

>[!MORELIKETHIS]
>
>[为“人员详细信息”页面创建自定义选项卡](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
