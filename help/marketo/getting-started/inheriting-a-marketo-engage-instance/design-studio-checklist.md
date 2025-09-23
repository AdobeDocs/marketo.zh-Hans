---
description: 继承实例Design Studio核对清单 — Marketo文档 — 产品文档
title: 继承实例Design Studio核对清单
feature: Getting Started
exl-id: 41e89120-4ac0-4e70-bed0-da4e5c5542ff
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 3%

---

# 继承实例：设计工作室检查表 {#inherited-instance-design-studio-checklist}

结构化模板和创建全局表单、代码片段以及图像和文件将有助于最大限度地减少数据错误并简化程序构建的工作流。 请记住[下载核对清单](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx)并跟踪您的进度。

## 登陆页面 {#landing-pages}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>全局登陆页面</td>
   <td><li>有多少个全局<a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages.md" target="_blank">登陆页面</a>？ 它们是否被程序使用？</li>
   <li>是否已设置<a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-learn.html" target="_blank">订阅中心</a>？
   <br/>     如果不能，请考虑创建一个。</li></td>
  </tr>
  <tr>
   <td>模板</td>
   <td><li>有多少个<a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.md" target="_blank">登陆页面模板</a>？ 它们是否正在被利用？</li></td>
  </tr>
  <tr>
   <td>测试组</td>
   <td><li>有多少个<a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups.md" target="_blank">登陆页面测试组</a>？ 它们仍然相关吗？</li></td>
  </tr>
   <tr>
   <td>隐私和合规性</td>
   <td><li>您的所有登陆页面是否都有相应的页脚？</li></td>
  </tr>
 </tbody>
</table>

## 图像和文件 {#images-and-files}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>命名约定</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md" target="_blank">图像和文件</a>是否具有一致的命名约定？</li></td>
  </tr>
  <tr>
   <td>文件夹结构</td>
   <td><li>图像和文件<a href="/help/marketo/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders.md" target="_blank">是否进行了适当组织</a>且易于搜索？</li></td>
  </tr>
  <tr>
   <td>图像和文件</td>
   <td><li>是否需要更新网页<a href="/help/marketo/product-docs/demand-generation/images-and-files/find-the-url-of-an-uploaded-image-or-file.md" target="_blank">上引用的任何图像或文件</a>？
   <p>示例：硬编码的URL结构<a href="https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632#_Toc54870361" target="_blank">可能需要更新</a>，如<code>http://na-sj01.marketo.com/rs/123-ABC-456/images/puppy.png</code>。
   <p>请与您的Web开发人员合作，确定可能需要进行更新的位置。</li></td>
  </tr>
 </tbody>
</table>

## 表单 {#forms}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>全局Forms</td>
   <td><li>有多少个全局<a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md" target="_blank">表单</a>？</li>
<li>大多数项目使用全球还是本地表单？</li>
<li>所有表单都在为营销和销售收集正确的数据吗？</li>
<li>隐藏值是否得到了适当利用？</li>
<li>是否在非Marketo Engage登陆页面上使用任何Marketo Engage表单？ 它们是如何被引用的？</li>
<p><img src="assets/tip-icon.png" alt="提示图标">提示：更新您使用引入的新嵌入代码嵌入Marketo Engage表单的页面（需要安全的登陆页面）。
<p><a href="/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/design-studio-checklist-2.png" target="_blank"><img src="assets/design-studio-checklist-1.png" alt="代码缩略图"></a>
</td>
  </tr>
  <tr>
   <td>数据标准化</td>
   <td><li>您的<a href="/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md" target="_blank">表单字段</a>主要是选择列表还是打开文本字段？</li>
<p><img src="assets/tip-icon.png" alt="提示图标">提示：如果它们是打开文本字段，请考虑将其切换到选择列表以防止数据混乱。</td>
  </tr>
  <tr>
   <td>隐私和合规性</td>
   <td><li>您的表单策略是否与企业数据隐私和选择加入要求保持一致？
   <br/>     请考虑一下<a href="https://business.adobe.com/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">通用数据保护条例(GDPR)</a>、加拿大的反垃圾邮件法(CASL)、2003年控制非请求性色情制品攻击和营销法案(CAN-SPAM)、加州消费者隐私法案(CCPA)等，以遵守相关法规。</li>
<p><img src="assets/tip-icon.png" alt="提示图标">提示：请记住在这些问题上始终咨询您的法律团队。 在作出任何更改之前，请咨询您的团队了解以前的计划以保持法规遵从性。</td>
  </tr>
 </tbody>
</table>

## 电子邮件 {#emails}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>全局电子邮件</td>
   <td><li>有多少全局<a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md" target="_blank">电子邮件</a>？ 它们是否被程序使用？</li></td>
  </tr>
  <tr>
   <td>模板</td>
   <td><li>有多少个<a href="/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md" target="_blank">电子邮件模板</a>？ 它们是否正在被利用？</li></td>
  </tr>
  <tr>
   <td>电子邮件测试</td>
   <td><li>您如何使用<a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/understanding-email-testing-options.md" target="_blank">电子邮件测试</a>？ 你的方法仍然有效吗？</li></td>
  </tr>
  </tr>
  <tr>
   <td>隐私和合规性</td>
   <td><li>您的所有电子邮件是否都有适当的页脚？ 考虑GDPR、CASL、CAN-SPAM、CCPA等 了解合规影响。</li>
<p><img src="assets/tip-icon.png" alt="提示图标">提示：请记住，请始终就这些合规性问题咨询您的法律团队。 在作出任何更改之前，请咨询您的团队了解以前的计划以保持法规遵从性。</td>
  </tr>
 </tbody>
</table>

## 代码段 {#snippets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>代码段</td>
   <td><li>有多少个<a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md" target="_blank">代码片段</a>？ 它们是否正在被使用？
   <br/>     如果没有，请考虑将它们用于<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md" target="_blank">电子邮件</a>和<a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page.md" target="_blank">登陆页面</a>页脚内容、徽标等。</li></td>
  </tr>
 </tbody>
</table>

## 所有Assets {#all-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>资源状态</td>
   <td><li>有多少资产处于<i>草稿</i>和<i>已批准且草稿</i>状态（例如，<a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md" target="_blank">电子邮件</a>、<a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md#approve-a-landing-page" target="_blank">登陆页面</a>、<a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/approve-a-form.md" target="_blank">表单</a>、<a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/approve-a-snippet.md" target="_blank">代码片段</a>）？
   <br/>     如果有多个文件夹，请考虑删除或批准这些文件夹。</li></td>
  </tr>
  <tr>
   <td>资产共享</td>
   <td><li><a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md#sharing-across-workspaces" target="_blank">在工作区之间共享哪些资源</a>？</li>
   <p><img src="assets/note-icon.png" alt="注释图标"> 注意：了解这一点很重要，因为在一个Workspace中执行的操作可能会导致其他用户在其他Workspace中无法访问资源。</td>
  </tr>
 </tbody>
</table>
