---
description: CT-YYYY-MM-Content，位于Marketo登录页面 — Marketo文档 — 产品文档
title: Marketo登录页面上的CT-YYYY-MM-Content
feature: Programs
exl-id: 638c4d6a-a8c7-4f03-9dae-07fecfb1302b
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 3%

---

# Marketo登录页面上的CT-YYYY-MM-Content {#ct-yyyy-mm-content-on-marketo-landing-page}

此示例设计为一个内容程序，该程序利用Marketo Engage登录页面和使用Marketo Engage默认程序的Marketo Engage表单。 表单用于访问内容/选件。 选件的链接可显示在感谢页面上、以感谢电子邮件发送或同时显示两者。

有关进一步的策略帮助或自定义计划的帮助，请联系Adobe客户团队或访问[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}页面。

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
   <td>Web内容</td> 
   <td>01个成员 
<br/>02 — 参与成功</td>
   <td>包含</td>
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
   <td>电子邮件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入门电子邮件模板</a></td>
   <td>01-Email — 谢谢</td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入门LP模板</a></td>
   <td>01 - LP — 注册</td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入门LP模板</a></td>
   <td>02 - LP — 谢谢</td>
  </tr>
  <tr> 
   <td>表单</td> 
   <td> </td>
   <td>FM — 内容注册表</td>
  </tr>
  <tr> 
   <td>本地报告</td> 
   <td> </td>
   <td>电子邮件性能</td>
  </tr>
  <tr> 
   <td>本地报告</td> 
   <td> </td>
   <td>登陆页面性能</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>00 — 捕获客户获取计划</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 — 填写表单</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 — 参与（计划成功）</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>Assets — 包含所有创意资产 
<br/>(电子邮件、登陆页面和Forms的子文件夹)  </td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>营销活动 — 包含所有智能营销活动</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>报告</td>
  </tr>
 </tbody> 
</table>

![](assets/ct-yyyy-mm-content-on-marketo-landing-page-1.png)

## 我的令牌已包含 {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>令牌类型</th> 
   <th>令牌名称</th>
   <th>值</th>
  </tr> 
  <tr> 
   <td>富文本</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>双击可查看详细信息  
<br/><code><--My Content Description Here--></code> 
<br/>在“我的令牌”选项卡下的程序级别编辑此内容描述。 
<br/>您将了解： 
<li>项目符号1</li>
<li>项目符号2</li>
<li>项目符号3</li></td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL？不带http://</td>
  </tr>
 </tbody> 
</table>

## 冲突规则 {#conflict-rules}

* **项目标记**
   * 在此订阅中创建标记 — _推荐_
   * 忽略

* **同名登陆页面模板**
   * 复制原始模板
   * 使用目标模板 — _推荐_

* **具有相同名称的图像**
   * 保留两个文件
   * 替换此订阅中的项目 — _推荐_

* **同名电子邮件模板**
   * 保留两个模板
   * 替换现有模板 — _推荐_

## 最佳实践 {#best-practices}

* 导入内容程序后，将表单从本地资产移动到位于Design Studio中的全局资产。
   * 减少表单数量并利用Design Studio中的更多全局资产，可在程序设计和管理中实现更大的可扩展性。 它还提供了灵活性，可以定期更新字段、选择加入语言等的合规性。

* 请考虑更新导入项目中的模板以使用当前品牌模板，或者通过添加代码片段或适当的徽标/页脚信息来更新新导入的模板以反映您的品牌。

* 请考虑更新此程序示例的命名约定，以符合您的命名约定。

>[!NOTE]
>
>切记在程序模板上更新我的令牌值，每次您根据需要使用程序时都要更新。

>[!TIP]
>
>不要忘记激活“02参与”营销活动以跟踪成功！ _before_&#x200B;执行此操作您的表单已上线且已发送电子邮件。

>[!IMPORTANT]
>
>引用URL的“我的令牌”不能包含http://或https:// ，否则该链接无法在资产中正常工作。
