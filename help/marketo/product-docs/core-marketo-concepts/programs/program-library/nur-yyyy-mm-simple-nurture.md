---
description: nur-YYYY-MM-Simple Nurture - Marketo文档 — 产品文档
title: NUR-YYYY-MM-Simple Nurture
feature: Programs
exl-id: 3e09ee4f-be65-4f2b-bdf5-ddd98bb49c1c
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 4%

---

# NUR-YYYY-MM-Simple Nurture {#nur-yyyy-mm-simple-nurture}

这是一个简单的Nurture Programs示例，它利用Marketo Engage参与计划，有节奏的内容随时间滴到数据库中，同时利用流根据行为引导记录历程。

如需进一步的战略帮助或自定义计划，请联系Adobe客户团队或访问 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} 页面。

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
   <td>客户培养</td> 
   <td>01 — 成员 
<br/>02 — 参与 — 成功</td>
   <td>包含</td>
   <td>参与</td>
  </tr>
 </tbody> 
</table>

## 程序包含以下资产 {#program-contains-the-following-assets}

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
   <td>01 — 电子邮件</td>
  </tr>
   <tr> 
   <td>电子邮件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入门电子邮件模板</a></td>
   <td>02 — 电子邮件</td>
  </tr>
   <tr> 
   <td>电子邮件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入门电子邮件模板</a></td>
   <td>03 — 电子邮件</td>
  </tr>
  <tr> 
   <td>本地报告</td> 
   <td> </td>
   <td>电子邮件性能</td>
  </tr>
  <tr> 
   <td>本地报告</td> 
   <td> </td>
   <td>参与流效果</td>
  </tr>
  <tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 — 添加到培养</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 — 暂停培养</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>03 — 继续培养</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>04 — 参与（计划成功）</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>资产 — 容纳所有创意资产
   <br/>（电子邮件的子文件夹）</td>
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

![](assets/nur-yyyy-mm-simple-nurture-1.png)

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
 </tbody> 
</table>

## 冲突规则 {#conflict-rules}

* **项目标记**
   * 在此订阅中创建标记 —  _推荐_
   * 忽略

* **同名登陆页面模板**
   * 复制原始模板
   * 使用目标模板 —  _推荐_

* **具有相同名称的图像**
   * 保留两个文件
   * 替换此订阅中的项目 —  _推荐_

* **同名电子邮件模板**
   * 保留两个模板
   * 替换现有模板 —  _推荐_

## 最佳实践 {#best-practices}

* 请考虑更新导入项目中的模板以使用当前品牌模板，或者通过添加代码片段或适当的徽标/页脚信息来更新新导入的模板以反映您的品牌。

* 请考虑更新此程序示例的命名约定，以符合您的命名约定。

* 确保您有暂停和恢复培养节奏的规则。 应在激活参与计划之前激活或计划这些智能营销活动。

>[!NOTE]
>
>切记在程序模板上更新我的令牌值，每次您根据需要使用程序时都要更新。

>[!TIP]
>
>不要忘记激活“04 — 参与（项目成功）”营销活动以跟踪成功！ 执行操作 _早于_ 您的电子邮件已发送。
