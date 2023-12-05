---
description: 文档 — Marketo文档 — 产品文档
title: 文档
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '836'
ht-degree: 0%

---

# 文档 {#doc}

文本

## Vibes SMS术语表 {#vibes-sms-glossary}

<table>
<thead>
  <tr>
    <th>术语</th>
    <th>定义</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>客户获取促销活动</td>
    <td>为获取订阅列表的新订阅者而开展的营销活动。 可通过Marketo Web窗体或发送关键词短信将订阅者添加到客户获取促销活动。</td>
  </tr>
  <tr>
    <td>营销活动管理器</td>
    <td>在Vibes平台中，您可以通过Campaign Manager设置订阅列表和客户获取促销活动。 具有完整Vibes平台许可证的用户有权访问其他营销活动类型。</td>
  </tr>
  <tr>
    <td>公司密钥</td>
    <td>company_key是您的平台帐户的唯一字母数字标识符。 如果在Vibes平台中有多个公司帐户（如子帐户），则可能会有多个company_keys。 每个Marketo Engage实例只能映射到一个Vibes company_key。</td>
  </tr>
  <tr>
    <td>CTA（行动号召）</td>
    <td>用于获取定期文本消息程序或订阅列表中的订阅者的数字或物理标牌或口头脚本。 可以置于在线、社交媒体、电子邮件、印刷品等中。</td>
  </tr>
  <tr>
    <td>自定义短域</td>
    <td>如果您使用的是Vibes链接缩短程序，则默认情况下，缩短的URL将显示在Vibes短URL： https://vbs.cm/xxxxxx下。 自定义短域是您的品牌特有的域。 <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">了解有关自定义短域的更多信息</a>.<p>
    这仅适用于从Vibes平台发送的消息，特别是客户获取促销活动消息和短代码默认消息。<p>
    推荐使用Marketo URL缩短器，以便在Marketo程序中包含点击数据。</td>
  </tr>
  <tr>
    <td>默认消息</td>
    <td>短代码的强制性消息，用于回复HELP、STOP和无法识别的消息请求。</td>
  </tr>
  <tr>
    <td>断开连接</td>
    <td>断开连接是一种由于手机号码从运营商网络中删除而导致的选择退出的形式。 断开连接的原因包括：帐户已完全关闭、预付帐户资金不足或出于其他未知原因从运营商网络中删除了号码。 断开连接且未移植到其他移动运营商的移动号码将从Vibes平台中的所有订阅列表中取消订阅。</td>
  </tr>
  <tr>
    <td>双重选择加入</td>
    <td>一种客户获取方法，要求潜在订阅者确认其同意通过响应命令（如“Y”或邮政编码）添加到订阅列表。 使用双重选择加入提示可以帮助您遵守州和联邦的短信准则。</td>
  </tr>
  <tr>
    <td>活动</td>
    <td>事件是可以提交到Vibes平台并用于触发API触发的操作（包括消息发送）的已定义发生次数。 每个事件都包含特定于事件的数据，包括一个event_type ，用于确定它对应于哪个API触发的消息营销活动。 事件API可以通过Marketo Engage中的Webhook触发。 通过我们的 <a href="https://developer-platform.vibes.com/reference/event-api">事件API参考</a>.</td>
  </tr>
  <tr>
    <td>关键词</td>
    <td>消费者发送到短代码的短单词或字母数字字符串，用于启动移动体验。</td>
  </tr>
  <tr>
    <td>长代码(10DLC)</td>
    <td>用于在品牌和消费者之间发送双向消息的发件人ID。 美国长码为10位数。</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>手机电话号码或人员的电话号码。 MDN和手机号码不是Marketo中的唯一标识符。</td>
  </tr>
  <tr>
    <td>移动数据库</td>
    <td>移动数据库是Vibes存储订阅者数据的数据库。 每个订阅者都有一个唯一的“人员记录”，其中填充了手机号码和任何关联的自定义字段。</td>
  </tr>
  <tr>
    <td>参与者</td>
    <td>与您的移动程序进行一个或多个移动交互（如发送短信）但尚未订阅订阅列表的人员。</td>
  </tr>
  <tr>
    <td>人员记录</td>
    <td>人员记录是特定手机号码的数据集合。 还为每个人员记录分配了一个唯一的person_key用于标识。 Marketo ID使用external_person_id字段链接到Vibes。 在中了解有关人员记录的更多信息 <a href="https://developer-platform.vibes.com/reference/person-api">Vibes人员API文档</a>.</td>
  </tr>
  <tr>
    <td>短代码</td>
    <td>用于在品牌和消费者之间发送双向消息的发件人ID。 美国的短码是5到6个数字。 加拿大短代码是4-6个数字。 Marketo LaunchPoint与Vibes的集成支持每个实例使用一个短代码。</td>
  </tr>
  <tr>
    <td>短信</td>
    <td>短信服务。 此消息仅包含文本。</td>
  </tr>
  <tr>
    <td>订阅列表</td>
    <td>同意接收来自您程序的定期消息的手机号码（及其对应的人员记录）列表。</td>
  </tr>
  <tr>
    <td>订阅者</td>
    <td>订阅订阅列表的手机号码。</td>
  </tr>
  <tr>
    <td>Vibes Platform</td>
    <td>您登录以管理营销活动的网站。 转到 <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> 访问Vibes平台。</td>
  </tr>
</tbody>
</table>

## 短信报告 {#sms-reporting}

文本

单击短信消息本地资产>查看功能板；消息级别的报表

屏幕快照

短信进度 — 显示发送的总数和投放的总数。 金额位于右侧，如果将鼠标悬停在栏上，则会显示百分比。

屏幕快照

“摘要”图表将以百分比形式显示计算出的跳出率。 将鼠标悬停在存档栏上，以查看按金额和百分比列出的投放率。 将鼠标悬停在栏的橙色跳出率部分上，可查看软跳出率和硬跳出率金额和百分比。

屏幕快照

使用“一段时间内的活动”图表可选择发送的总数或投放的总数。 从日期范围选择器中选择适当的范围。

屏幕快照
