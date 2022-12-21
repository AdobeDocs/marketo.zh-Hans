---
description: 默认Veeva字段映射 — Marketo文档 — 产品文档
title: 默认Veeva字段映射
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 30%

---

# 默认Veeva字段映射 {#default-veeva-field-mapping}

当您最初将Marketo Engage帐户与Veeva同步时，Marketo会自动在您内置的Veeva字段和Marketo字段之间进行这些关联。 Marketo还将在您的帐户和联系人上同步您的自定义字段。

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
      <td>人员说明</td>
    </tr>
    <tr>
      <td>电子邮件</td>
      <td>电子邮件地址</td>
    </tr>
    <tr>
      <td>商务传真</td>
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
      <td>已删除SFDC</td>
    </tr>
    <tr>
      <td>姓氏</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>潜在客户来源</td>
      <td>源</td>
    </tr>
    <tr>
      <td>潜在客户分数</td>
      <td>得分</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>城市</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>国家</td>
    </tr>
    <tr>
      <td>MailingPostalCode</td>
      <td>邮政编码</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>州</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>地址</td>
    </tr>
    <tr>
      <td>手机</td>
      <td>手机号码</td>
    </tr>
    <tr>
      <td>商业电话</td>
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
      <td>帐单邮政编码</td>
      <td>帐单邮政编码</td>
    </tr>
    <tr>
      <td>账单州/省</td>
      <td>帐单寄送州</td>
    </tr>
    <tr>
      <td>比利街</td>
      <td>帐单寄送地址</td>
    </tr>
    <tr>
      <td>帐户描述</td>
      <td>公司说明</td>
    </tr>
    <tr>
      <td>行业</td>
      <td>行业</td>
    </tr>
    <tr>
      <td>已删除</td>
      <td>已删除SFDC</td>
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
      <td>帐户网站</td>
      <td>网站</td>
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

## Marketo中与Veeva相关的系统字段（只读） {#veeva-related-system-fields-in-marketo}

这些字段在Marketo中创建，但客户无法调整。

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
      <td>Veeva Id</td>
      <td>18个字符的Salesforce Id</td>
    </tr>
    <tr>
      <td>Veeva类型</td>
      <td>联系。 如果为空，则潜在客户仅作为人员存在在Marketo</td>
    </tr>
    <tr>
      <td>Veva创建日期</td>
      <td>在SFDC中创建的日期(可以与在Marketo中创建的日期不同)</td>
    </tr>
    <tr>
      <td>Veeva已删除</td>
      <td>以前在SFDC工作的人员已被删除，现在只能在Marketo工作</td>
    </tr>
  </tbody>
</table>
