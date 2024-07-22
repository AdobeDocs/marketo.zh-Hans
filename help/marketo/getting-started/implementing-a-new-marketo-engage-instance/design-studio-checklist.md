---
description: 为新Marketo Engage实例设置Design Studio部分。
title: 新实例最佳实践 — 设计工作室核对清单
feature: Getting Started
exl-id: 070ee235-dad0-4627-bac0-14bf0174bb03
source-git-commit: 7805983cdaff0b99a38aefc2c2467b53f3386da3
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 2%

---

# 新实例最佳实践：设计工作室核对清单 {#new-instance-best-practices-design-studio-checklist}

Design Studio部分是可重复使用的“全局资产”应驻留的位置。 创建您的组织计划在程序中使用的全局资产，使用一致的命名约定，并将它们组织在子文件夹中以便轻松搜索。

请记住[下载核对清单](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)并跟踪您的进度。

## 登陆页面 {#landing-pages}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>全局登陆页面</td>
    <td><li>创建<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages#product-docs" target="_blank">全局登陆页面（自由格式/引导式）</a>。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups" target="_blank">创建测试页面</a>以测试入选的登陆页面模板（如果适用）。</li></td>
  </tr>
  <tr>
    <td>模板</td>
    <td><li>为全局登陆页面创建设计。</li></td>
  </tr>
  <tr>
    <td>隐私和合规性</td>
    <td><li>在登陆页面中使用<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page" target="_blank">代码片段</a>或<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-text-and-tokens-to-a-landing-page#add-a-token-to-your-landing-page" target="_blank">令牌</a>创建页脚，以符合隐私要求。</li></td>
  </tr>
</tbody>
</table>

## Forms {#forms}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>全局Forms</td>
    <td><li>设置<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/forms/creating-a-form/create-a-form#product-docs" target="_blank">全局表单</a>以用于订阅首选项、封闭内容下载、演示请求、网络研讨会注册等用例。</li></td>
  </tr>
  <tr>
    <td>隐私和合规性</td>
    <td><li>使您的表单符合<a href="https://business.adobe.com/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">通用数据保护条例(GDPR)</a>。</li></td>
  </tr>
  <tr>
    <td>数据标准化</td>
    <td><li>请考虑将选择列表应用于<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/forms/creating-a-form/add-a-field-to-a-form#product-docs" target="_blank">表单字段</a>，而不是应用于打开的文本字段以防止数据混乱。</li></td>
  </tr>
</tbody>
</table>

## 电子邮件 {#emails}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>全局电子邮件</td>
    <td><li>创建全局电子邮件。</li></td>
  </tr>
  <tr>
    <td>模板</td>
    <td><li>使用设计人员/开发人员设计基于模块的<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/general/email-editor-2/create-an-email-template" target="_blank">电子邮件模板</a>，或使用您自己的HTML。</li>
    <li>创建经过测试的电子邮件模板以A/B测试入选模板（如果适用）。</li></td>
  </tr>
  <tr>
    <td>隐私和合规性</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email" target="_blank">向电子邮件模板中添加代码片段</a>以控制可重复使用的块，如版权年份、全球位置和特定于合规性的语言。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email" target="_blank">添加令牌</a>以根据目标受众对内容进行个性化。</li></td>
  </tr>
</tbody>
</table>

## 代码片段 {#snippets}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>代码片段</td>
    <td><li>创建<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet#product-docs" target="_blank">代码片段</a>，使其具有可重复使用的内容块，这些内容块可用于多个用例，例如电子邮件和登陆页中的联系信息、社交媒体链接、品牌信息以及隐私和合规性说明。</li></td>
  </tr>
</tbody>
</table>

## 图像和文件 {#images-and-files}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>命名约定</td>
    <td><li>对图像和文件使用一致的命名约定。</li>  
    <br>示例：  
    <br><ul><li>文件命名约定：资产类型 — 资产名称（例如：White-Paper-Evaluating-Cloud-Computing-Get-Your-Board-on-Board）</li>
    <p><li>图像命名约定：图像类型 — 资产类型 — 资产名称（例如：Thumbnail-White-Paper-Evaluating-Cloud-Computing-Get-Your-Board-on-Board）</li></td>
  </tr>
</tbody>
</table>

## 组织 {#organization}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>文件夹结构 </td>
    <td><li>为每种类型的资产创建子文件夹，并<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders" target="_blank">组织全局资产</a>（例如，对话流、电子邮件模板、电子邮件、表单、图像和文件、登陆页面、登陆页面模板、代码片段等） 适当地。</li></td>
  </tr>
</tbody>
</table>
