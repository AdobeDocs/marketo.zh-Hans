---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: 'https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 29aa413a7346a79906f4021dedc79e8e48170c69
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 15%
---
# 发行说明：2026年10月 {#release-notes-oct-26}

在下方，您会找到2026年10月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年10月23日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。 请查看每个功能旁边的状态。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>规划营销活动技能</strong>：适用于Marketo Engage的CX Enterprise Coworker现在可以将营销活动简报转换为完整的Marketo Engage项目设置文档。 该文档包括文件夹结构、智能营销活动、电子邮件配置、令牌和QA核对清单。 这有助于团队更快地启动营销活动，并标准化项目设置。 技能可通过Markdown进行配置。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>可调用代理</strong>：创建作为智能营销活动中的流程步骤运行的AI代理，并根据您以纯语言编写的说明对潜在客户记录执行操作。 例如，代理可以标准化潜在客户的数据或标记可能的机器人，然后将结果写回潜在客户上的字段。 这可以在无需自定义代码的情况下将基于判断的销售线索处理纳入营销活动。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>克隆到此程序/文件夹</strong>：现在，跨Marketo Engage的克隆操作始终提供“此文件夹”或“此程序”选项作为选择克隆资源的目标时的首选选项。 选择此选项可将资源克隆到当前资源的父程序或文件夹。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <tr>
   <td><strong>有关CRM同步的即时警报</strong>：启用或禁用环境的本机CRM同步现在会向订阅CRM通知渠道的用户触发通知。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **弃用从Web获取图像**：为了符合现代安全和隐私最佳实践，从10月版本起，[从Web获取图像](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"}功能将被弃用。

* **自定义活动属性的API名称限制**：通过API或UI创建的自定义活动属性的API名称现在只能包含字母数字字符和下划线，并且必须以字母数字字符开头。

* **Get Lead Activities和Get Lead Changes的静态列表大小限制**：从2026年9月30日起，如果目标列表包含10,000个或更多潜在客户，对包含`listId`参数的Get Lead Activities或Get Lead Changes端点的调用开始失败，并显示1003错误代码（指示目标静态列表包含太多记录）。 请参阅[迁移指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}以获取更多信息。
