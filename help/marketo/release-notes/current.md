---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 94c6a8dd94bce1d4e938f62365e8fc2c3c391814
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 2%

---

# 发行说明： 2023年7月 {#release-notes-july-23}

在下面，您会找到2023年7月版本中包含的所有功能。 查看Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![星形](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，并将于以下日期开始发行 **2023年7月21日**，在接下来的几周内分阶段推出剩余的功能。 发行功能和日期可能会有变动。 请检查每个功能下方的状态。

</br>

* **参与画布**：参与画布是一种可视化工具，允许您构建和组织可重复使用的营销活动。 它完全向后兼容，因此通过单击按钮，即可在此新结构中查看所有现有营销策划。 画布可以下载和共享。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

## Agile版本功能

以下功能遵循Agile格式，并在标准发布日期之前或之后的各种日期发布。 请检查每个功能下方的状态。

### Dynamic Chat {#dynamic-chat}

</br>

* **Dynamic Chat聊天源**：“聊天”现在作为新人员记录和活动的源提供。 此源可用于帮助用户筛选智能列表/营销活动中的活动。 还可以阻止源更新字段。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

* **增强的Dynamic Chat活动**：Dynamic Chat活动、筛选器和触发器已通过其他属性和标准命名约定得到增强。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

### Marketo Sales Insight {#marketo-sales-insight}

</br>

* **取消订阅附加设置**：现在，通过新的配置选项取消订阅附加，您可以更好地控制取消订阅消息。 新功能使管理员能够控制取消订阅消息在销售电子邮件中的显示时间、位置和内容。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

* **动态字段提示**：您现在可以提示销售团队进一步个性化电子邮件中的特定部分，在Sales Insight Actions中为电子邮件模板添加新的字段提示。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

* **默认动态字段**：默认动态字段允许您配置一个回退值，如果没有可填充的值，动态字段可以解析该回退值。 这有助于确保在填写所有个性化设置后发送电子邮件。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

* **对Sales Insight的Dynamic Chat支持**：已进行更新，以支持所有Dynamic Chat用户在此版本中引入的新Dynamic Chat属性。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

* **对Sales Insight Actions的Dynamic Chat支持**：我们现在支持潜在客户信息源中的Dynamic Chat活动，以及在将Live Chat路由到代理时的通知。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

* **Dynamic Chat触发令牌**：引入了用于有趣时刻的Dynamic Chat活动的新触发器令牌。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>

## 公告 {#announcements}

Marketo Engage实时个性化即将提供两项增强功能。

* **升级到jQuery 3.7**：为了提高安全性和稳定性，Marketo正在升级到jQuery 3.7.0。未加载其自身jQuery的RTP用户不会受到负面影响，因为Marketo将更改从rtp.js加载的默认版本。 但是，如果您的RTP用户使用的jQuery版本低于3.0.0，请与 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} ，以获得实施符合您需求的自定义版本rtp.js的帮助。

>[!NOTE]
>
>请与您的Web开发团队合作，以确定您的网站是加载您自己的JQuery库，还是使用从Web个性化RTP JavaScript标记加载的默认版本。

* **升级到Google Analytics4**：Marketo以前支持Universal Analytics，后者将在2023年7月1日之前停止记录数据。 RTP用户将需要遵循其Google Analytics功能板中的迁移过程，以完全支持RTP中的Google Analytics4集成。 今后，用户将拥有一个独特的字母数字标记(位于 `<head>` 部分)，允许Marketo向Google Analytics发送数据。
