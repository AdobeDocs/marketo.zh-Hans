---
description: WR-YYYY-MM-Web请求程序 — Marketo文档 — 产品文档
title: WR-YYYY-MM-Web请求程序
feature: Programs
exl-id: 4acaa2d0-3329-4027-acbd-ae2e0ec6f7c5
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 3%

---

# WR-YYYY-MM-Web请求程序 {#wr-yyyy-mm-web-request-program}

这是一个示例计划，非常适合于使用Marketo Engage默认计划的联系人申请、报价申请、演示申请或试用申请表。 可与Marketo登陆页面一起使用，或作为非Marketo登陆页面上的嵌入式表单。 在提交表单时，会向指定的个人发送警报电子邮件。

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
   <td>Web请求</td> 
   <td>01 — 参与 — 成功</td>
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
   <td>表单</td> 
   <td> </td>
   <td>FM-WebRequestForm</td>
  </tr>
  <tr> 
   <td>电子邮件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入门电子邮件模板</a></td>
   <td>警报 — Web请求</td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入门LP模板</a></td>
   <td>01 - LP — 请求</td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入门LP模板</a></td>
   <td>02 - LP — 谢谢</td>
  </tr>
  <tr> 
   <td>本地报告</td> 
   <td> </td>
   <td>登陆页面性能</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>来自Web请求的新人员</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>网络研讨会的新用户</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>Assets — 容纳所有创意资源 
<br/>（警报和登陆页面的子文件夹）</td>
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

![](assets/wr-yyyy-mm-web-request-program-1.png)

## 我的令牌已包含 {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>令牌类型</th> 
   <th>令牌名称</th>
   <th>值</th>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.Request-Type}}</code></td>
   <td>联系我们</td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.ALERT-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.ALERT-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.ALERT-ReplyToAddress}}</code></td>
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

* 导入网络研讨会程序后，将表单从本地资产移动到位于Design Studio中的全局资产。
   * 减少表单数量并利用Design Studio中的更多全局资产，可在程序设计和管理中实现更大的可扩展性。 它还提供了灵活性，可以定期更新字段、选择加入语言等的合规性。

* 请考虑更新导入项目中的模板以使用当前品牌模板，或者通过添加代码片段或适当的徽标/页脚信息来更新新导入的模板以反映您的品牌。

* 请考虑更新此程序示例的命名规则以符合您的命名规则。

>[!NOTE]
>
>切记在程序模板上更新我的令牌值，每次您根据需要使用程序时都要更新。

>[!IMPORTANT]
>
>引用URL的“我的令牌”不能包含http://或https:// ，否则该链接无法在资产中正常工作。
