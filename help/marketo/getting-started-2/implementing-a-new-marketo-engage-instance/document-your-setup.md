---
description: 记录新Marketo Engage实例的设置。
title: 新实例最佳实践 — 记录您的设置
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 47446db902f85e1b4a910d0924efc5beb82bffbe
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# 新实例最佳实践：记录您的设置 {#new-instance-best-practices-document-your-setup}

现在您已经了解了为新的Marketo Engage实例设置的关键产品领域，下一步是创建实例配置和技术栈栈的文档。 无论是通过电子表格还是项目管理应用程序创建实例，您的文档都将是跟踪进展和记录详细信息以及保持实例结构化和可持续性的有用资源，可供组织内的未来营销人员使用。

## 数据 {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>列表导入</td>
    <td><li>收集将从中提取记录的数据源列表 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people" target="_blank">导入到Marketo Engage</a>.</li>
    <li>如果要从多个数据源导入，请考虑使用“主列表”或 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">创建自定义字段</a> 在人员记录上表示数据源。</li></td>
  </tr>
  <tr>
    <td>数据库集成</td>
    <td><li>如果利用Marketo Engage与CRM之间的本机同步，请仔细考虑要在系统之间同步的字段。 并非每个字段都需要同步，因此请对数据流采取战略性措施。</li></td>
  </tr>
</tbody>
</table>

## 文档 {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>用户</td>
    <td><li>记录 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">当前用户</a> 出于安全原因，在您的实例中。 以下详细信息应至少包含在内(转到Adobe Admin Console &gt;用户即可全部看到)：</li>
    <br>名称
    <br>电子邮件
    <br>ID类型
    <br>产品配置文件
    <p>
    <li>作为Marketo Engage产品管理员，制定定期审核和更新Marketo Engage用户列表的内部流程。 要更改Adobe Admin Console中的用户列表，请考虑 <a href="https://helpx.adobe.com/cn/enterprise/using/users.html" target="_blank">上传.csv</a> 批量。</li></td>
  </tr>
  <tr>
    <td>组织</td>
    <td><li>记录商定的文件夹结构、程序、资产等的标准命名惯例以及做出决策的原因。 <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">在此处详细了解最佳实践。</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>创建一个更改日志，您可以在其中记录实例中的更改内容以及进行修改的原因。 <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">在此处详细了解最佳实践。</a></li></td>
  </tr>
  <tr>
    <td>行动手册</td>
    <td><li>为载入实例的内部用户创建用户剧本或管理员剧本。</li></td>
  </tr>
  <tr>
    <td>与内部团队的对话</td>
    <td><li>开始使内部营销团队的Marketo Engage期望与Marketo Engage的功能保持一致。</li>
    <li>确定在Marketo Engage实例中将成为您利益相关者的团队，并记录他们使用Marketo Engage作为技术来实现的目标。</li></td>
  </tr>
</tbody>
</table>
