---
description: 继承文档1 - Marketo文档 — 产品文档
title: 继承文档1
hide: true
hidefromtoc: true
source-git-commit: b6628cee17799801815f5b84c424399538eaf5ee
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 7%

---

# 继承文档1 {#inherit-doc-1}

对继承的实例进行审计可能看起来像是

您是否从其他管理员继承了现有Marketo Engage实例？ 如果是这样的话，这篇文章是为您准备的。

>[!TIP]
>
>如果您是新Marketo Engage用户并且不熟悉许多术语，请查看 [Marketo术语表](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## 用户和角色 {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>用户</td> 
   <td><li>有多少用户？</li>
<li>是否有任何应过期的用户？</li>
<li>贵公司是否有删除用户的相关政策？</li> 
<li>有多少用户具有管理员权限？</li>
<li>这些用户中的任何一个是否应更改为其他角色？</li> 
<li>此实例中的API用户是谁？</li></td>
   <td>3.1</td>
  </tr>
  <tr> 
   <td>角色</td> 
   <td><li>有多少角色？</li>  
<li>每个角色具有哪些权限/访问权限？ 是否应对任何内容进行调整？</li>
<li>每个角色有多少用户？</li>
<li>用户登录的频率如何？</li>
<li>每个API用户是否都有自己的用户角色？ 如果不能，请考虑实施此操作以更轻松地排除故障。</li> 
<li>您的用户角色和权限是否与公司数据隐私政策一致？</li></td>
   <td>3.2</td>
  </tr>
  <tr> 
   <td>内部文档</td> 
   <td><li>您的组织中是否明确定义了用户和角色？</li>
<li>您添加新用户/管理员的流程是什么？</li></td>
   <td>3.3</td>
  </tr>
  <tr> 
   <td>沙盒（如果适用）</td> 
   <td><li>您是否有沙盒实例？ 如果是这样的话，请查看上面针对沙盒的类别。</li>
<li>项目导入是否与您的沙盒关联？</li></td>
   <td>3.4</td>
  </tr>
 </tbody> 
</table>

## 审核记录 {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>审核记录</td> 
   <td><li>谁在实例中工作？</li></td>
   <td>3.1</td>
  </tr>
 </tbody> 
</table>

## 工作区和分区 {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>工作区和分区</td> 
   <td><li>您有多少工作区和/或分区？</li>
<li>每个工作区和分区的主要用途是什么？</li>
<li>它们是否需要审核或更改？</li>
<li>工作区和分区之间的关系是什么？</li>
<li>每个工作区有多少用户具有访问权限？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>内部文档</td> 
   <td><li>如何定义工作区和分区？</li>
<li>向实例添加工作区或向工作区添加用户的流程是什么？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 智能营销活动 {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>Smart Campaign设置</td> 
   <td><li>您是否对Smart Campaign的大小有限制？</li>
<li>如果不能，请考虑添加一个。 我们建议将智能营销活动限制为数据库的25%，以避免在工作流程中过度通信或处理整个数据库，这不仅会保护您的品牌，还有助于保护实例的性能。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 通信限制 {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>通信限制</td> 
   <td><li>是否存在限制？ 贵企业是否有可能需要通信限制的政策？</li>
<li>Adobe建议将通信限制为每天1次，每7天3次，并阻止非操作电子邮件。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 标记 {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>标记</td> 
   <td><li>有多少个标记？ 正在使用多少个标记？ 是否需要添加任何内容？</li>
<li>您的项目中是否需要标记？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>渠道</td> 
   <td><li>有多少个渠道？ 有多少项正在使用？</li>
<li>是否所有渠道计划状态都合适？ 它们是否在计划中显示进度？</li>
<li>您的渠道是否与特定项目类型相关？</li>
<li>哪些状态被视为每个渠道的成功？ 这些是否符合您的营销目标？</li>
<li>是否正确使用了操作渠道？</li>
<li>对于高级Report Builder(Revenue Cycle Explorer\RCE)，您的渠道分析行为是否设置为与纳入期间成本的计划实践保持一致？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>营销日历（如果适用）</td> 
   <td><li>有多少种日历条目类型？ 它们仍然相关吗？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 数据库管理 {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>字段管理</td> 
   <td><li>有多少田？ 单击“导出字段名称”可查看您的字段、自定义字段及其API名称的列表。</li>
<li>有多少自定义字段？</li>
<li>使用了多少字段？ 在字段操作下拉列表中选择“导出使用者”，以查看字段的相关资源。</li>
<li>Marketo Engage与您的CRM之间同步了多少次？</li>
<li>CRM字段是否已同步到相应的对象？</li>
<li>是否为人员详细信息设置了自定义视图？ 应该有吗？</li>
<li>您的字段是否具有基于源的命名约定？ 如果不能，请考虑实施此操作。</li>
<li>是否存在阻止的字段？ 一定要明白为什么会这样。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>自定义活动</td> 
   <td><li>是否有任何自定义活动？</li>
<li>如果是这样的话，请单击它们以了解哪些活动与Marketo表单、电子邮件或登陆页面无关。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>自定义对象</td> 
   <td><li>有多少自定义对象？ 它们如何同步到您的CRM？</li>
<li>您的程序和列表查询如何使用这些自定义对象？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 集成 {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight （如果适用）</td> 
   <td><li>是否已安装MSI软件包？</li>
<li>您是否已升级到最新版本的Sales Insight？</li>
<li>您是否已完成Sales Insight配置？</li>
<li>您是否根据已购买的名额授予了用户访问权限？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 宝箱 {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 其他 {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>区域</th> 
   <th>审核焦点</th>
   <th>列3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
