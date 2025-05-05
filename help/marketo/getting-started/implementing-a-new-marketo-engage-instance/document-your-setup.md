---
description: 记录新Marketo Engage实例的设置。
title: 新实例最佳实践 — 记录您的设置
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 1%

---

# 新实例最佳实践：记录您的设置 {#new-instance-best-practices-document-your-setup}

现在您已经了解了为新的Marketo Engage实例设置的关键产品领域，下一步是创建实例配置和技术栈栈的文档。 无论是通过电子表格还是项目管理应用程序创建实例，您的文档都将是跟踪进展和记录详细信息以及保持实例结构化和可持续性的有用资源，可供组织内的未来营销人员使用。

## 数据 {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>列表导入</td>
    <td><li>收集将从其中提取记录的数据源列表，以<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">导入到Marketo Engage</a>。</li>
    <li>如果要从多个数据源导入，请考虑使用主列表或在人员记录上创建<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">自定义字段</a>来表示数据源。</li></td>
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
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>用户</td>
    <td><li>出于安全原因，在您的实例中记录<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">当前用户</a>。 以下详细信息应至少包含在内（通过转至“管理员”&gt;“用户和角色”可全部显示）：</li>
    <ul>
    <li>名称</li>
    <li>电子邮件</li>
    <li>登录</li>
    <li>角色</li>
    <li>访问到期日期</li>
    <li>用户创建日期</li>
    <li>最近登录日期</li></ul>
    <p><img src="assets/note-icon.png" alt="注释图标"> 注意：您还可以展开此项，以包含有关角色/权限的文档。
    <p>
    <li>作为Marketo Engage产品管理员，制定定期审核和更新Marketo Engage用户列表的内部流程。 要更改Adobe Admin Console中的用户列表，请考虑<a href="https://helpx.adobe.com/cn/enterprise/using/users.html" target="_blank">批量操作</a>，例如上传.CSV、使用用户管理REST API等</li></td>
  </tr>
  <tr>
    <td>组织</td>
    <td><li>记录商定的文件夹结构、程序、资产等的标准命名惯例以及做出决策的原因。 <a href="https://experienceleague.adobe.com/zh-hans/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">在此处了解关于最佳实践的更多信息。</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>创建一个更改日志，您可以在其中记录实例中的更改内容以及进行修改的原因。 <a href="https://experienceleague.adobe.com/zh-hans/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">在此处了解关于最佳实践的更多信息。</a></li></td>
  </tr>
  <tr>
    <td>行动手册</td>
    <td><li>为载入实例的内部用户创建用户剧本或管理员剧本。</li></td>
  </tr>
  <tr>
    <td>与内部团队的对话</td>
    <td><li>使内部营销团队的Marketo Engage期望与Marketo Engage的功能保持一致。</li>
    <li>确定在Marketo Engage实例中将成为您利益相关者的团队，并记录他们使用Marketo Engage作为技术来实现的目标。</li></td>
  </tr>
  <tr>
    <td>工作区和分区（如果适用）</td>
    <td><li>记录工作区的定义方式以及它与数据库分区的关系（例如，显示每个人相对于业务部门的全局工作区）。</li>
    <li>将新记录导入相应的分区。</li>
    <li>在CRM中定义将用户放入相应分区的值。</li></td>
  </tr>
</tbody>
</table>
