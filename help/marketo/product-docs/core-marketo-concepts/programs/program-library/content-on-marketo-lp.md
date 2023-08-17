---
description: Marketo LP上的内容 — Marketo文档 — 产品文档
title: Marketo LP上的内容
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 2%

---

# Marketo LP上的内容 {#content-on-marketo-lp}

项目名称：Marketo LP上的CT-YYYY-MM-Content

此示例参考旨在成为一个内容程序，它利用Marketo登陆页面和Marketo表单，来利用Marketo默认程序。 表单用于访问内容/选件。 选件的链接可显示在感谢页面上、以感谢电子邮件发送或同时显示两者。 如需进一步的战略帮助或自定义计划，请联系Adobe客户团队或访问 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) 页面。

**渠道摘要**

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
<br/>02参与成功</td>
   <td>包含</td>
   <td>默认</td>
  </tr>
 </tbody> 
</table>

**程序包含以下资源：**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>类型</th> 
   <th>模板名称</th>
   <th>资源名称</th>
  </tr> 
  <tr> 
   <td>电子邮件</td> 
   <td>快速入门电子邮件模板</td>
   <td>01-Email — 谢谢</td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td>快速入门LP模板</td>
   <td>01 - LP — 注册</td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td>快速入门LP模板</td>
   <td>02 - LP — 谢谢</td>
  </tr>
  <tr> 
   <td>表单</td> 
   <td> </td>
   <td>内容注册表</td>
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
   <td>01填写表单</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02参与（计划成功）</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>资产 — 容纳所有创意资产 
<br/>（电子邮件和登陆页面的子文件夹）  </td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>营销活动 — 包含所有智能营销活动</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>报表</td>
  </tr>
 </tbody> 
</table>

屏幕快照 — 项目图片

**我的令牌包括：**

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
<br/>在“我的令牌”选项卡下的项目级别编辑此内容描述。 
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
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文本</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL？不带http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>有关默认冲突规则，请参阅程序导入说明。

**建议的导入默认冲突规则：**

* 项目标记
   * 在此订阅中创建标记（默认） — 推荐
   * 忽略

* 同名登陆页面模板
   * 复制原始模板（默认）
   * 使用目标模板 — 推荐

* 具有相同名称的图像
   * 保留两个文件（默认）
   * 替换此订阅中的项目 — 推荐

* 同名电子邮件模板
   * 保留两个模板（默认）
   * 替换现有模板 — 推荐

SCREENSHOT — 默认冲突规则图片

**推荐的最佳实践：**

* Marketo咨询最佳实践建议在导入内容项目后，将表单从本地资源移至Marketo Engage设计工作室中的全局资源。
   * 减少表单数量并利用Design Studio中的更多全局资产，可在程序设计和管理中实现更大的可扩展性。 它还提供了灵活性，可以定期更新字段、选择加入语言等的合规性。

* 请考虑更新导入项目中的模板，以便使用当前品牌模板，或者通过添加代码片段或适当的徽标和页脚信息来更新新导入的模板以反映您的品牌。

* 如果需要，可以考虑更新此项目模板的命名约定，使其与您的命名约定保持一致。

* 不要忘记根据需要更新程序模板上的我的令牌值，每次您使用程序时都要更新。

* 如需进一步的战略帮助或自定义计划，请联系您的Adobe客户团队或访问 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) 页面。

>[!TIP]
>
>不要忘记激活“02参与”营销活动以跟踪成功！ 请在您的表单上线并发送电子邮件之前执行此操作。

>[!NOTE]
>
>引用URL的“我的令牌”不能包含http://或https:// ，否则该链接无法在资产中正常工作。
