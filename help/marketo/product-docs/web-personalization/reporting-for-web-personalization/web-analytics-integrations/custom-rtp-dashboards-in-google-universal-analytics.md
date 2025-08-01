---
unique-page-id: 7504238
description: Google Universal Analytics中的自定义RTP功能板 — Marketo文档 — 产品文档
title: Google Universal Analytics中的自定义RTP功能板
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Google Universal Analytics中的自定义RTP功能板 {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[将RTP与Google Universal Analytics集成](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

本文说明如何在Google Universal Analytics (GUA)中设置RTP功能板。 从RTP发送到GUA的数据可以设置为两个单独的自定义仪表板，称为：

* RTP B2B
* RTP参与

## 设置自定义仪表板 {#setting-up-a-custom-dashboard}

1. 登录到Google Analytics。 单击顶部菜单中的&#x200B;**[!UICONTROL Reporting]**。 单击&#x200B;**[!UICONTROL Dashboards]**&#x200B;和&#x200B;**[!UICONTROL New Dashboard]**。

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. 选择&#x200B;**空白画布**，添加&#x200B;**仪表板名称**，然后单击&#x200B;**[!UICONTROL Create Dashboard]**。

1. 单击&#x200B;**[!UICONTROL Add Widget]**&#x200B;以创建新构件。

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B仪表板 {#rtp-b-b-dashboard}

此仪表板允许用户从B2B角度分析其网站性能。

它按行业、收入、规模、基于帐户的列表和目标区段提供访问来源和现场行为等信息。

仪表板由3列组成

* 流量源
* 区段
* 第一层向下扩展

1. 创建一个名为&#x200B;**RTP B2B仪表板**&#x200B;的新仪表板，并定义以下小组件：

![](assets/image2015-3-22-16-3a50-3a3.png)

<table>
 <thead>
  <tr>
   <th>
    <div>
      列1 — 流量源
    </div></th>
   <th>
    <div> <strong>列2 — 分段</strong>
    </div></th>
   <th>
    <div> <strong>列3 — 第一层向下钻取</strong>
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>
    <ul>
     <li>名称：按区段和渠道显示的会话</li>
     <li>构件类型：<span class="uicontrol">栏</span><br></li>
     <li><span class="uicontrol">创建一个显示</span>：<span class="uicontrol">会话</span>的条形图</li>
     <li><span class="uicontrol">按</span>分组： <span class="uicontrol">事件标签</span></li>
     <li><span class="uicontrol">透视依据</span>：<span class="uicontrol">默认渠道分组</span></li>
     <li>筛选器：<br><span class="uicontrol">仅显示</span> | <span class="uicontrol">事件类别</span> （<span class="uicontrol">包含</span>） RTP区段</li>
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名称：RTP分段用户的数量</li>
     <li>类型： <span class="uicontrol">2.1指标</span></li>
     <li><span class="uicontrol">显示以下量度</span>： <span class="uicontrol">用户</span><br></li>
     <li>筛选器：<br><span class="uicontrol">仅显示</span> | <span class="uicontrol">事件类别</span> （包含）RTP段</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名称：按行业划分的会话</li>
     <li>类型： <span class="uicontrol">饼图</span><br></li>
     <li><span class="uicontrol">创建一个饼图，其中显示</span>： <span class="uicontrol">会话</span></li>
     <li><span class="uicontrol">按</span>分组：<span class="uicontrol">RTP-Industry</span></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <th>
    <ul>
     <li><strong>名称：按行业和渠道划分的会话</strong></li>
     <li><strong>构件类型：<span class="uicontrol">栏</span></strong></li>
     <li><strong><span class="uicontrol">创建一个显示</span>：<span class="uicontrol">会话</span>的条形图</strong></li>
     <li><strong><span class="uicontrol">分组依据</span>： <span class="uicontrol">RTP-Industry</span></strong></li>
     <li><strong><span class="uicontrol">透视依据</span>：<span class="uicontrol">默认渠道分组</span></strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li>
    </ul></th>
   <th>
    <ul>
     <li><strong>名称：按国家/地区分段会话</strong></li>
     <li><strong>类型： <span class="uicontrol">Geomap</span></strong></li>
     <li><strong><span class="uicontrol">绘制所选量度</span>： <span class="uicontrol">国家/地区</span> | <span class="uicontrol">个会话</span></strong></li>
     <li><strong><span class="uicontrol">选择区域</span>：<span class="uicontrol">世界</span></strong></li>
     <li><strong>筛选器：<span class="uicontrol">仅显示</span> | <span class="uicontrol">事件类别</span> （包含）RTP段</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th>
    <ul>
     <li><strong>名称：按RTP类别显示的会话</strong></li>
     <li><strong>类型： <span class="uicontrol">饼图</span></strong></li>
     <li><strong><span class="uicontrol">创建一个饼图，其中显示</span>： <span class="uicontrol">会话</span></strong></li>
     <li><strong><span class="uicontrol">按</span>分组： <span class="uicontrol">RTP类别</span></strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
  </tr>
  <tr>
   <th> </th>
   <th>
    <ul>
     <li>名称：热门目标区段</li>
     <li>类型： <span class="uicontrol">栏</span></li>
     <li><span class="uicontrol">创建一个显示</span>： <span class="uicontrol">用户</span>的条形图</li>
     <li><span class="uicontrol">按</span>分组： <span class="uicontrol">事件操作</span></li>
     <li>筛选器：<span class="uicontrol">仅显示</span> | <span class="uicontrol">事件类别</span> （包含）RTP段</li>
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th>
    <ul>
     <li>名称：按RTP组排列的会话</li>
     <li>类型：条形图<br></li>
     <li>创建条形图，其中显示：会话</li>
     <li>分组依据： RTP-Group</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
  </tr>
  <tr>
   <th> </th>
   <th>
    <ul>
     <li>名称：按热门区段划分的会话和目标</li>
     <li>类型：表<br></li>
     <li>显示以下列：<br>事件标签 | 会话 | 目标转化率</li>
     <li>筛选器：<br>仅显示 | 事件类别（包含）RTP区段</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th> </th>
  </tr>
 </tbody>
</table>

## RTP参与仪表板 {#rtp-engagement-dashboard}

利用此仪表板，用户可分析其RTP促销活动绩效和推荐引擎参与情况。 它提供了平均值的比较。 会话持续时间和每个会话页数介于：

* 未参与
* 参与次数（个性化营销活动的展示次数和点击次数）
* 推荐引擎和主要推荐内容的点击量

创建一个名为&#x200B;**RTP参与仪表板**&#x200B;的新仪表板，并定义以下小组件：

![](assets/image2015-3-22-17-3a7-3a19.png)

<table>
 <thead>
  <tr>
   <th>
    <div> <strong>列1促销活动曝光度</strong>
    </div></th>
   <th>
    <div> <strong>列2促销活动点进</strong>
    </div></th>
   <th>
    <div> <strong>列3推荐引擎</strong>
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>
    <ul>
     <li>名称：<strong>CTA参与总数</strong></li>
     <li>类型： <strong>2.1指标</strong></li>
     <li>显示以下量度：<strong>总事件</strong></li>
     <li>筛选器：<br><strong>[仅显示]事件类别（包含）： RTP-Campaigns</strong><br><strong>[仅显示]事件操作（完全匹配）： Impression</strong>[不显示]事件标签（包含）： #</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名称： <strong>CTA总数（点进）</strong></li>
     <li>类型： <strong>2.1指标</strong></li>
     <li>显示以下量度：<strong>总事件</strong></li>
     <li>筛选器：<br><strong>[仅显示]事件类别（包含）： RTP-Campaigns</strong><br><strong>[仅显示]事件操作（完全匹配）：点击次数</strong><strong>[不显示]事件标签（包含）： #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名称： <strong>CRE — 总点击次数</strong></li>
     <li>类型： <strong><span class="uicontrol">2.1指标</span></strong><br></li>
     <li><span class="uicontrol">显示以下量度</span>： <strong><span class="uicontrol">页面查看次数</span></strong></li>
     <li>筛选器： <strong>[<span class="uicontrol">仅显示</span>] <span class="uicontrol">页面</span> （<span class="uicontrol">包含</span>）： rcmd</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <td colspan="1">
    <ul>
     <li>名称： <strong>平均 会话持续时间（参与度）</strong></li>
     <li>类型： <strong>2.1指标</strong></li>
     <li>显示以下量度： <strong>平均 会话持续时间</strong></li>
     <li>筛选器：<br><strong>[仅显示]事件类别（完全匹配）： RTP-Campaigns</strong><br><strong>[仅显示]事件操作（完全匹配）： impression</strong><strong>[不显示]事件标签（包含）： #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td colspan="1">
    <ul>
     <li>名称： <strong>平均 会话持续时间（点进）</strong></li>
     <li>类型： <strong>2.1指标</strong></li>
     <li>显示以下量度： <strong>平均 会话持续时间</strong></li>
     <li>筛选器：<br><strong>[仅显示]事件类别（完全匹配）： RTP-Campaigns</strong><br><strong>[仅显示]事件操作（完全匹配）：点击次数</strong><strong>[不显示]事件标签（包含）： #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td colspan="1">
    <ul>
     <li>名称： <strong>CRE — 最推荐的内容</strong></li>
     <li>类型： <strong><span class="uicontrol">表</span></strong><br></li>
     <li><span class="uicontrol">显示以下列</span>： <br><strong><span class="uicontrol">页面标题</span> | <span class="uicontrol">页面查看次数</span></strong><br></li>
     <li>筛选器：<br>筛选器： <strong>[<span class="uicontrol">仅显示</span>] <span class="uicontrol">页面</span> （<span class="uicontrol">包含</span>）： rcmd</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <td>
    <ul>
     <li>名称： <strong>页面/会话（参与度）</strong></li>
     <li>类型： <strong><span class="uicontrol">2.1指标</span> </strong></li>
     <li><span class="uicontrol">显示以下量度</span>：<strong><span class="uicontrol">页/会话</span></strong></li>
     <li>筛选器：<br><strong>[<span class="uicontrol">仅显示</span>] <span class="uicontrol">事件类别</span> （<span class="uicontrol">完全匹配</span>）： RTP促销活动</strong></li>
     <li><strong>[<span class="uicontrol">只显示</span>] <span class="uicontrol">事件操作</span> （<span class="uicontrol">完全匹配</span>）： impression</strong></li>
     <li><strong>[<span class="uicontrol">不显示</span>] <span class="uicontrol">事件标签</span> （<span class="uicontrol">包含</span>）： #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名称： <strong>页面/会话（点进）</strong></li>
     <li>类型： <strong>2.1指标</strong></li>
     <li>显示以下量度：<strong>页面/会话</strong></li>
     <li>筛选器：<br><strong>[仅显示]事件类别（完全匹配）： RTP — 促销活动</strong></li>
     <li><strong>[仅显示]事件操作（完全匹配）：点击次数</strong></li>
     <li><strong>[不显示]事件标签（包含）： #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td> </td>
  </tr>
  <tr>
   <td>
    <ul>
     <li>名称：<strong>CTA展示次数</strong></li>
     <li>类型： <strong><span class="uicontrol">表</span></strong></li>
     <li><span class="uicontrol">显示以下列</span>： <strong><span class="uicontrol">事件标签</span> | <span class="uicontrol">事件总数</span> | <span class="uicontrol">用户</span></strong></li>
     <li>筛选器：<br><strong>[<span class="uicontrol">仅显示</span>] <span class="uicontrol">事件类别</span> （<span class="uicontrol">完全匹配</span>）： RTP — 营销活动</strong><br><strong>[<span class="uicontrol">仅显示</span>] <span class="uicontrol">事件操作</span> （<span class="uicontrol">完全匹配</span>）：展示</strong><strong>[<span class="uicontrol">不显示</span>] <span class="uicontrol">事件标签</span> （<span class="uicontrol">包含</span>）： #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>名称：<strong>CTA点进</strong></li>
     <li>类型： <strong><span class="uicontrol">表</span></strong></li>
     <li><span class="uicontrol">显示以下列</span>： <strong><span class="uicontrol">事件标签</span> | <span class="uicontrol">事件总数</span> | <span class="uicontrol">用户</span></strong></li>
     <li>筛选器：<br><strong>[<span class="uicontrol">仅显示</span>] <span class="uicontrol">事件类别</span> （<span class="uicontrol">完全匹配</span>）： RTP营销活动</strong><br><strong>[<span class="uicontrol">仅显示</span>] <span class="uicontrol">事件操作</span> （<span class="uicontrol">完全匹配</span>）：点击次数</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td> </td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[将RTP与Google Universal Analytics集成](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>Google Universal Analytics中的[自定义RTP报告](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
