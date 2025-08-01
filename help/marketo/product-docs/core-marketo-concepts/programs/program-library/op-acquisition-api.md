---
description: OP-Acquisition-API - Marketo文档 — 产品文档
title: OP-Acquisition-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 4%

---

# OP-Acquisition-API {#op-acquisition-api}

此示例程序适用于利用Marketo Engage默认程序跟踪从API源获取记录的操作流程。

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

## 程序包含以下Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>类型</th>
   <th>模板名称</th>
   <th>资源名称</th>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>设置客户获取 — 批次</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>设置客户获取 — 触发器</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>营销活动（包含所有智能营销活动）</td>
  </tr>
 </tbody>
</table>

![](assets/op-acquisition-api-1.png)

## 冲突规则 {#conflict-rules}

* **项目标记**
   * 在此订阅中创建标记 — _推荐_
   * 忽略

* **同名登陆页面模板**
   * 复制原始模板 — _推荐_
   * 使用目标模板

* **具有相同名称的图像**
   * 保留两个文件 — _推荐_
   * 替换此订阅中的项目

* **同名电子邮件模板**
   * 保留两个模板 — _推荐_
   * 替换现有模板

## 最佳实践 {#best-practices}

* 如果您需要在数据管理中赶上，请首先运行批处理营销活动。

* 考虑使用类似的程序，以确保与所有输入源的最佳实践保持一致，以包括您的CRM或数据集成。

* 在特定于渠道的营销计划中，请务必根据需要捕获客户获取。
