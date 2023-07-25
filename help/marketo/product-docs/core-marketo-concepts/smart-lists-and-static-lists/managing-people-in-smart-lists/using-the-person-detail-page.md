---
unique-page-id: 2953415
description: 使用人员详细信息页面 — Marketo文档 — 产品文档
title: 使用人员详细信息页面
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 22%

---

# 使用人员详细信息页面 {#using-the-person-detail-page}

人员详细信息页面包含Marketo知道的有关人员的所有信息。 您可以直接从此页面编辑数据。

## 转至人员详细信息页面 {#getting-to-person-detail-page}

有许多方法可打开特定人员。 一些示例包括：

* 从 **数据库**，您可以在快速查找中搜索
* 任何智能 **列表** 或列表
* **成员** 项目群选项卡
* **查看营销活动成员** 在智能营销活动中
* 部分 **报告**
  <br> 

1. 双击任意人员或单击左侧的ID。

   ![](assets/one-1.png)

1. 这将打开人员详细信息屏幕。

   ![](assets/two-5.png)

## 页面组织 — Salesforce {#page-organization-salesforce}

人员信息分为以下选项卡：

| 选项卡 | 描述 |
|---|---|
| 信息 | 联系信息和有关人员的自定义字段。 |
| 公司信息 | 人员的公司信息和地址。 |
| 机会信息 | 机会信息已从Salesforce同步。 |
| SFDC潜在客户字段 | 内置Salesforce字段。 |
| SFDC自定义字段 | 自定义Salesforce字段。 |
| 活动日志 | 与人员相关的所有活动。 |

## 页面组织 — Microsoft Dynamics {#page-organization-microsoft-dynamics}

| 选项卡 | 描述 |
|---|---|
| 信息 | 联系信息和有关人员的自定义字段。 |
| 公司信息 | 人员的公司信息和地址。 |
| 机会信息 | 机会信息已从Microsoft同步。 |
| Microsoft自定义字段 | 自定义Microsoft字段。 |
| Microsoft潜在客户字段 | 内置Microsoft字段。 |
| 活动日志 | 与人员相关的所有活动。 |

>[!NOTE]
>
>您还可以看到机会信息 [通过API插入](https://developers.marketo.com/rest-api/lead-database/opportunities/) 用于未与CRM同步的实例。

## 编辑字段 {#editing-a-field}

许多字段都是可编辑的。 要更新人员信息，请键入新值，然后单击字段外部进行保存。

![](assets/image2015-2-27-11-3a14-3a2.png)

## CRM同步之前的Marketo默认字段 {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| 地址 | 年营业额 | 匿名IP | 帐单寄送地址 | 帐单寄送城市 |
| 帐单寄送国家 | 帐单邮政编码 | 帐单寄送州 | 城市 | 公司名称 |
| 国家 | 创建时间 | 出生日期 | 部门 | 请勿来电 |
| 不要调用原因 | 请勿来电的理由 | 电子邮件地址 | 电子邮件无效 | 电子邮件无效原因 |
| 外部公司 ID | 外部销售人员 ID | 传真号码 | 名 | 全名 |
| 行业 | 推断的城市 | 推断公司 | 推断国家 | 推断的都市区 |
| 推断的电话区号 | 推断的邮政编码 | 推断的状态区域 | 匿名 | 是客户 |
| 是合作伙伴 | 职务 | 姓 | 评级 | 得分 |
| 人员来源 | 状态 | 主要电话 | Marketo Social Facebook显示名称 | Marketo Social Facebook Id |
| Marketo Social Facebook照片URL | Marketo Social Facebook配置文件URL | Marketo Social Facebook范围 | Marketo Social Facebook引用的注册 | Marketo Social Facebook反向访问 |
| Marketo社交性别 | Marketo Social上次引用的注册 | Marketo Social上次引荐访问 | Marketo Social LinkedIn显示名称 | Marketo Social LinkedIn Id |
| Marketo Social LinkedIn照片URL | Marketo Social LinkedIn配置文件URL | Marketo Social LinkedIn范围 | Marketo Social LinkedIn引用的注册 | Marketo Social LinkedIn反向访问 |
| Marketo社交联合ID | Marketo Social 反向注册次数总计 | Marketo Social 反向访问次数总计 | Marketo Social Twitter显示名称 | Marketo Social Twitter Id |
| Marketo Social Twitter照片URL | Marketo Social Twitter配置文件URL | Marketo Social Twitter范围 | Marketo Social Twitter引用的注册 | Marketo Social Twitter反向访问 |
| 中间名称 | 手机号码 | 员工数 | 电话号码 | 邮政编码 |
| 优先级 | 相对分数 | 职位 | 称谓 | 标准产业分类(SIC)代码 |
| 现场 | 州 | 退订 | 退订原因 | 更新时间 |
| 紧急 | 网站 |  |  |  |

>[!NOTE]
>
>某些字段为 _非_ 可编辑：
>
>* 活动日志
>* 公司信息
>* SFDC联系人的机会
>* 特定于Marketo的字段，例如“创建日期”和“原始源类型”。
>
>详细了解 [系统管理的字段](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[创建人员详细信息页面的自定义选项卡](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
