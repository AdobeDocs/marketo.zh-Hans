---
description: 操作数据管理 — Marketo文档 — 产品文档
title: 操作数据管理
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 14%

---

# 操作数据管理 {#op-data-management}

这是一个使用默认程序的简单操作数据管理最佳实践工作流的示例，可帮助您管理Marketo Engage数据库中记录的数据一致性。

要获得进一步的战略帮助或自定义计划，请联系Adobe客户团队或访问[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}页面。

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
   <td>标准化国家/地区 — 美国</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>标准化国家/地区 — 英国</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>列入阻止列表将设置为True</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>将Is Partner设置为True</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>列表导入</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>现场活动</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>在线Advertising</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>贸易展</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>Web内容</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>Web请求</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>网络研讨会</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>从列表导入新人员</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>实时活动的新人员</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>在线Advertising的新用户</td>
  </tr>
  <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>贸易展的新人员</td>
  </tr>
   <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>从Web内容新建人员</td>
  </tr>
   <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>来自Web请求的新人员</td>
  </tr>
   <tr>
   <td>智能营销活动</td>
   <td> </td>
   <td>网络研讨会的新用户</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>人员Source夜间批处理（适用于高流量实例）</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>Source触发的人员（适用于低流量实例）</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>捕获人员Source</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>标准化</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>记录管理</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>阻止列表</td>
  </tr>
 </tbody>
</table>

![](assets/op-data-management-1.png)

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

* 构建的每个营销活动都是以最佳实践构建为例，而不是特定于您的用例。 请记住更新智能营销活动以解决您的特定棘手问题和数据挑战。

* 请考虑更新此程序示例的命名约定，以符合您的命名约定。
