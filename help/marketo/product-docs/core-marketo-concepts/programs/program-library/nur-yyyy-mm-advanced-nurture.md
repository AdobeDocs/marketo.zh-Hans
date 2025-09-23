---
description: NUR-YYYY-MM-Advanced Nurture - Marketo文档 — 产品文档
title: NUR-YYYY-MM-高级培养
feature: Programs
exl-id: bd9c6605-a13f-4c73-aaa8-eca43cfcc950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 10%

---

# NUR-YYYY-MM-高级培养 {#nur-yyyy-mm-advanced-nurture}

这是利用Marketo Engage参与计划的高级培养计划示例。 嵌套电子邮件程序阻止用户接收他们已使用的内容，或控制他们应在每个流中使用的内容类型。 可以为每个嵌套电子邮件程序运行归因报表。 渠道：“Nurture”以及嵌套电子邮件程序的专用“Nurture电子邮件”渠道使用Marketo Engage电子邮件程序发送一封新闻稿电子邮件。 电子邮件可以包含或不包含A/B测试。

要获得进一步的战略帮助或自定义计划，请联系Adobe客户团队或访问[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}页面。

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
<br/>02 — 已参与 — 成功</td>
   <td>包含</td>
   <td>参与度</td>
  </tr>
  <tr>
   <td>培养电子邮件</td>
   <td>01 — 跳过
<br/>02 — 已发送
<br/>03 — 已参与 — 成功</td>
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
   <td>嵌套程序</td>
   <td> </td>
   <td>01 — 主题X</td>
  </tr>
  <tr>
   <td>嵌套程序</td>
   <td> </td>
   <td>02 — 主题Y</td>
  </tr>
  <tr>
   <td>嵌套程序</td>
   <td> </td>
   <td>03 — 主题Z</td>
  </tr>
  <tr>
   <td>电子邮件</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速启动电子邮件模板</a></td>
   <td>01 — 电子邮件（位于嵌套程序中）</td>
  </tr>
   <tr>
   <td>电子邮件</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速启动电子邮件模板</a></td>
   <td>02 — 电子邮件（位于嵌套程序中）</td>
  </tr>
   <tr>
   <td>电子邮件</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速启动电子邮件模板</a></td>
   <td>03 — 电子邮件（位于嵌套程序中）</td>
  </tr>
  <tr>
   <td>本地报告</td>
   <td> </td>
   <td>电子邮件性能</td>
  </tr>
  <tr>
   <td>本地报告</td>
   <td> </td>
   <td>电子邮件链接性能</td>
  </tr>
  <tr>
  <tr>
   <td>智能活动</td>
   <td> </td>
   <td>01 — 添加到培养</td>
  </tr>
  <tr>
   <td>智能活动</td>
   <td> </td>
   <td>02 — 暂停培养</td>
  </tr>
  <tr>
   <td>智能活动</td>
   <td> </td>
   <td>03 — 继续培养</td>
  </tr>
  <tr>
   <td>智能活动</td>
   <td> </td>
   <td>04 — 参与（计划成功）</td>
  </tr>
  <tr>
   <td>智能活动</td>
   <td> </td>
   <td>00 — 跳过电子邮件（位于每个嵌套程序中）</td>
  </tr>
  <tr>
   <td>智能活动</td>
   <td> </td>
   <td>01 — 发送电子邮件（位于每个嵌套程序中）</td>
  </tr>
  <tr>
   <td>智能活动</td>
   <td> </td>
   <td>02 — 参与成功（位于每个嵌套程序中）</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>Assets（包含嵌套程序和Asset文件夹也位于嵌套程序中以包含电子邮件）</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>嵌套程序(位于Assets文件夹下)</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>营销活动 — 将所有“智能营销活动”置于父培养项目中，营销活动文件夹也位于每个嵌套项目中</td>
  </tr>
  <tr>
   <td>文件夹</td>
   <td> </td>
   <td>报告</td>
  </tr>
 </tbody>
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

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

* 请考虑更新导入项目中的模板以使用当前品牌模板，或者通过添加代码片段或适当的徽标/页脚信息来更新新导入的模板以反映您的品牌。

* 请考虑更新此程序示例的命名约定，以符合您的命名约定。

* 确保您有暂停和恢复培养节奏的规则。 应在激活参与计划之前激活或计划这些智能营销活动。

>[!NOTE]
>
>切记在程序模板上更新我的令牌值，每次您根据需要使用程序时都要更新。

>[!TIP]
>
>不要忘记激活“04 — 参与（项目成功）”营销活动以跟踪成功！ 请在发送电子邮件前&#x200B;_执行_&#x200B;操作。
