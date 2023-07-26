---
unique-page-id: 7504218
description: Google Universal Analytics中的自定义RTP报表 — Marketo文档 — 产品文档
title: Google Universal Analytics中的自定义RTP报表
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Google Universal Analytics中的自定义RTP报表 {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[将RTP与Google Universal Analytics集成](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

本文介绍了如何为Google Universal Analytics (GUA)设置RTP自定义报表。  从RTP发送到GUA的数据可以设置为两个单独的自定义报告，称为：

* RTP B2B
* RTP参与

## 设置自定义报表 {#setting-up-a-custom-report}

1. 登录到Google Analytics。

1. 单击 **自定义** 在顶部菜单中。

1. 单击 **+新建自定义报表**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## RTP B2B报告 {#rtp-b-b-report}

1. 命名报告 **RTP B2B报告**.

1. 命名第一个选项卡 **行业**.

>[!NOTE]
>
>您会 **复制此选项卡** 并创建其他类似的报表 — 步骤5)

1. 选择 **资源管理器** 报告类型。

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. 在 **量度组** 部分，选择与您的业务相关的量度。

   a.我们建议如下：

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. 复制此选项卡4次并命名它们：

   1. **行业**
   1. **组**
   1. **类别**
   1. **ABM**
   1. **组织**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. 在 **Dimension深入分析** 部分为每个选项卡设置相关维度，如下所示。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      选项卡名称 
    </div></th> 
   <th> 
    <div>
      Dimension深入分析
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>行业</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>类别</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>组织</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. 不要设置任何过滤器，将此报告设置为可用于 **所有网站数据** （如果与特定Analytics帐户相关，则进行更改）。

1. 单击 **保存**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP参与报告 {#rtp-engagement-report}

1. 命名报告 **RTP参与报告**.

1. 将第一个选项卡名称设置为 **所有参与度**.

>[!NOTE]
>
>您将复制此选项卡并创建其他类似选项卡 — 步骤5)

1. 选择 **资源管理器** 报告类型。

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. 在指标组部分，选择与您的业务相关的指标。 以下是建议：

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. 复制此选项卡4次并命名它们：

   1. **所有参与度**
   1. **按行业列出的参与情况**
   1. **按组显示的参与情况**
   1. **按类别显示的参与情况**
   1. **按ABM列出的参与情况**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. 在 **Dimension深入分析** 部分为每个选项卡设置相关维度，如下所示：

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      选项卡名称 
    </div></th> 
   <th> 
    <div>
      Dimension深入分析 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>所有参与度</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>按ABM列出的参与情况</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>按类别显示的参与情况</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>按组显示的参与情况</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>按行业列出的参与情况</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. 设置以下过滤器：

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      字段 
    </div></th> 
   <th> 
    <div>
      匹配类型 
    </div></th> 
   <th> 
    <div>
      值 
    </div></th> 
   <th colspan="1"> 
    <div>
      评论 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>包括</p></td> 
   <td><p>事件类别</p></td> 
   <td>正则表达式</td> 
   <td>RTP-Campaigns|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">将筛选所有与RTP无关的其他自定义事件</td> 
  </tr> 
  <tr> 
   <td>排除</td> 
   <td>事件标签</td> 
   <td>正则表达式</td> 
   <td>#</td> 
   <td colspan="1">允许使用营销活动名称中的#从报表营销活动中进行筛选</td> 
  </tr> 
 </tbody> 
</table>

1. 将此报告设置为可用于 **所有网站数据** （如有必要，请进行更改）。

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. 单击 **保存**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[将RTP与Google Universal Analytics集成](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Google Universal Analytics中的自定义RTP功能板](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
