---
description: 默认 [!DNL Veeva] 字段映射 — Marketo文档 — 产品文档
title: 默认 [!DNL Veeva] 字段映射
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 36%

---

# 默认[!DNL Veeva]字段映射 {#default-veeva-field-mapping}

当您最初将Marketo Engage帐户与[!DNL Veeva]同步时，Marketo会自动在内置[!DNL Veeva]和Marketo字段之间关联这些关联。 Marketo还将同步您的“帐户”和“联系人”中的自定义字段。

## 联系人字段 {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC字段</th>
      <th>Marketo字段</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>出生日期</td>
      <td>出生日期</td>
    </tr>
    <tr>
      <td>创建日期</td>
      <td>SFDC创建日期</td>
    </tr>
    <tr>
      <td>联系人描述</td>
      <td>人员备注</td>
    </tr>
    <tr>
      <td>电子邮件</td>
      <td>电子邮件地址</td>
    </tr>
    <tr>
      <td>公司传真</td>
      <td>传真号码</td>
    </tr>
    <tr>
      <td>名字</td>
      <td>名字</td>
    </tr>
    <tr>
      <td>电子邮件选择退出</td>
      <td>退订</td>
    </tr>
    <tr>
      <td>已删除</td>
      <td>已删除 SFDC</td>
    </tr>
    <tr>
      <td>姓氏</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>潜在客户来源</td>
      <td>来源</td>
    </tr>
    <tr>
      <td>潜在客户分数</td>
      <td>得分</td>
    </tr>
    <tr>
      <td>邮寄城市</td>
      <td>城市</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>国家/地区</td>
    </tr>
    <tr>
      <td>MailingPostCode</td>
      <td>邮政编码</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>State</td>
    </tr>
    <tr>
      <td>邮寄街</td>
      <td>地址</td>
    </tr>
    <tr>
      <td>手机</td>
      <td>手机号码</td>
    </tr>
    <tr>
      <td>公司电话</td>
      <td>电话号码</td>
    </tr>
    <tr>
      <td>称谓</td>
      <td>称谓</td>
    </tr>
    <tr>
      <td>标题</td>
      <td>职务</td>
    </tr>
  </tbody>
</table>

## 帐户字段 {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC字段</th>
      <th>Marketo字段</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>年收入</td>
      <td>年收入</td>
    </tr>
    <tr>
      <td>帐单寄送城市</td>
      <td>帐单寄送城市</td>
    </tr>
    <tr>
      <td>帐单寄送国家</td>
      <td>帐单寄送国家</td>
    </tr>
    <tr>
      <td>帐单邮编</td>
      <td>帐单邮政编码</td>
    </tr>
    <tr>
      <td>记帐省/市/自治区</td>
      <td>帐单寄送州</td>
    </tr>
    <tr>
      <td>帐单街道</td>
      <td>帐单寄送地址</td>
    </tr>
    <tr>
      <td>帐户说明</td>
      <td>公司注释</td>
    </tr>
    <tr>
      <td>行业</td>
      <td>行业</td>
    </tr>
    <tr>
      <td>已删除</td>
      <td>已删除 SFDC</td>
    </tr>
    <tr>
      <td>帐户名称</td>
      <td>公司名称</td>
    </tr>
    <tr>
      <td>员工</td>
      <td>员工数</td>
    </tr>
    <tr>
      <td>帐户电话</td>
      <td>主要电话</td>
    </tr>
    <tr>
      <td>SIC 代码</td>
      <td>SIC 代码</td>
    </tr>
    <tr>
      <td>帐户站点</td>
      <td>地点</td>
    </tr>
    <tr>
      <td>帐户类型</td>
      <td>SFDC 类型</td>
    </tr>
    <tr>
      <td>网站</td>
      <td>网站</td>
    </tr>
  </tbody>
</table>

## Marketo中与[!DNL Veeva]相关的系统字段（只读） {#veeva-related-system-fields-in-marketo}

这些字段是在Marketo中创建的，但无法由客户调整。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>字段</th>
      <th>描述</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[!DNL Veeva] Id</td>
      <td>由18个字符组成的[!DNL Salesforce] ID</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] 类型</td>
      <td>联系。 如果为空，则商机在Marketo中仅作为人员存在</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] 创建日期</td>
      <td>在SFDC中创建的日期(可以不同于在Marketo中创建的日期)</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] 已删除</td>
      <td>此人以前在SFDC中，但现在已被删除，仅居住在Marketo中</td>
    </tr>
  </tbody>
</table>
