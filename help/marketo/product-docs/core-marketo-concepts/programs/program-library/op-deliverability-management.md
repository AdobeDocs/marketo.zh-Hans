---
description: 操作可投放性管理 — Marketo文档 — 产品文档
title: 操作可投放性管理
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 6b54fe2830200c6673559a257065248390c6d212
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 4%

---

# 操作可投放性管理 {#op-deliverability-management}

这是一个利用Marketo Engage默认程序进行可投放性管理最佳实践工作流的示例，该工作流用于审查您当前的电子邮件可投放性状态并管理长期退回和未响应者。

>[!NOTE]
>
>需要自定义字符串字段“营销暂停原因”才能导入。 [了解详情](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

如需进一步的战略帮助或自定义计划，请联系Adobe客户团队或访问 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} 页面。

## 渠道摘要 {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>渠道</th> 
   <th>成员资格状态</th>
   <th>Analytics行为</th>
   <th>项目类型</th>
  </tr> 
  <tr> 
   <td>可操作</td> 
   <td>01个成员</td>
   <td>可操作</td>
   <td>默认</td>
  </tr>
 </tbody> 
</table>

## 先决条件字段 {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>类型</th> 
   <th>友好名称</th>
   <th>API名称</th>
  </tr>
  <tr> 
   <td>字符串</td> 
   <td>营销暂停原因</td>
   <td>MarketingSuspendedReason</td>
  </tr>
 </tbody> 
</table>

## 程序包含以下资产 {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>类型</th> 
   <th>模板名称</th>
   <th>资源名称</th>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>营销暂停长期无响应者</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>营销暂停将长期退回电子邮件</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>更新电子邮件后重置“电子邮件无效”</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>电子邮件更新后重置“营销已暂停”</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>管理</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>审查</td>
  </tr>
 </tbody> 
</table>

![](assets/op-deliverability-management-1.png)

## 冲突规则 {#conflict-rules}

* **项目标记**
   * 在此订阅中创建标记 —  _推荐_
   * 忽略

* **同名登陆页面模板**
   * 复制原始模板 —  _推荐_
   * 使用目标模板

* **具有相同名称的图像**
   * 保留两个文件 —  _推荐_
   * 替换此订阅中的项目

* **同名电子邮件模板**
   * 保留两个模板 —  _推荐_
   * 替换现有模板

## 最佳实践 {#best-practices}

* 构建的每个营销活动都是以最佳实践构建为例，而不是特定于您的用例。 请记住更新智能营销活动以解决您的特定棘手问题和数据挑战。

* 请考虑更新此程序示例的命名约定，以符合您的命名约定。
