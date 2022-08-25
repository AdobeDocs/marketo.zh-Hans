---
description: 聊天机器人行为 — Marketo文档 — 产品文档
title: 聊天机器人行为
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: 1803d6355747f4b6300509a3d361bf235dd56f44
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# 聊天机器人行为 {#chatbot-behavior}

下面是访客在每个聊天机器人预期行为之外的不同可能情景。

<table>
  <tbody>
    <tr>
      <th>缩写</th>
      <th>详细信息</th>
    </tr>
    <tr>
      <td>D1、D2、D3等</td>
      <td>表示多个对话框，其中D1为对话框1</td>
    </tr>
    <tr>
      <td>P1、P2、P3等</td>
      <td>表示P1为最高优先级的对话优先级</td>
    </tr>
    <tr>
      <td>WP1、WP2、WP3等</td>
      <td>表示多个网页，其中WP1是第一个网页</td>
    </tr>
    <tr>
      <td>V1、V2、V3等</td>
      <td>表示多个网页访客，其中V1为访客1</td>
    </tr>
   </tbody>
</table>

## 方案 {#scenarios}

<table>
  <tr>
      <th>方案</th>
      <th>预期的聊天机器人行为</th>
      <th>后端操作</th>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1访问WP1</p>
      </td>
      <td>
        <p>D1将解析为V1 </p>
      </td>
      <td>D1的触发器计数将增加1</td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1访问WP1</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将解析为V1</p>
        <p>刷新后，D1将再次得到解析</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>刷新后，对D1触发器或参与计数没有任何更改</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，但未响应</p>
      </td>
      <td>D1将解析为V1</td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>D1参与计数没有变化</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击并提供第一个响应</p>
      </td>
      <td>D1将解析为V1</td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>D1的参与次数将增加1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击并提供第一个响应</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将解析为V1</p>
        <p>刷新后，D1将继续</p>
      </td>
      <td>
        <p>D1的触发器计数和参与计数将增加1</p>
        <p>刷新后，对任何计数均无更改</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，与聊天机器人互动，并完成D1</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将解析为V1</p>
        <p>刷新后，将不会为V1解析任何对话框或下一个对话框</p>
      </td>
      <td>
        <p>D1的触发器计数、参与计数和已完成计数将增加1</p>
        <p>刷新后，不会解析任何对话框或下一个对话框</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1,WP2</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，但未响应 </p>
        <p>V1访问WP2</p>
      </td>
      <td>
        <p>页面访问WP1、D1将解析为V1</p>
        <p>页面访问WP2、D1将解析为V2</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>在WP2中，对D1触发器计数没有更改</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1,WP2</p>
        <p>V1首次访问WP1</p>
        <p>V1点击D1并参与</p>
        <p>V1访问WP2</p>
      </td>
      <td>
        <p>页面访问WP1、D1将解析为V1</p>
        <p>页面访问WP2、D1将解析为V1</p>
      </td>
      <td>
        <p>D1的触发器计数和参与计数将增加1</p>
        <p>在WP2中，对任何计数均不进行更改</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>D2仅针对WP2</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击并提供第一个响应</p>
        <p>V1访问WP2</p>
      </td>
      <td>
        <p>D1将在WP1上解析</p>
        <p>D1在WP2上将继续为V1</p>
      </td>
      <td>
        <p>D1的触发器计数和参与计数将增加1</p>
        <p>对D2触发器或参与计数没有更改</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>D2仅针对WP2</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，但未响应 </p>
        <p>V1访问WP2</p>
      </td>
      <td>D1将在WP1上解析<br/>
      D2将在WP2上解析</td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>D2的触发器计数将增加1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>D2仅针对WP2</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击并完成D1</p>
        <p>V1访问WP2</p>
      </td>
      <td>D1将在WP1和完成后得到解决<br/>D2将在WP2上解析</td>
      <td>
        <p>D1的触发器计数、参与计数和已完成计数将增加1</p>
        <p>D2的触发器计数将增加1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>D2仅针对WP2</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击并完成D1</p>
        <p>V1访问WP2</p>
        <p>D2上的V1点击提供第一个响应 </p>
      </td>
      <td>D1将在WP1和完成后得到解决<br/>D2将在WP2上解析</td>
      <td>
        <p>D1的触发器计数、参与计数和已完成计数将增加1</p>
        <p>D2的触发器和参与计数将增加1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，但未响应</p>
        <p>D1已取消发布</p>
      </td>
      <td>D1将解析为V1</td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>D1参与计数没有变化</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，但未响应</p>
        <p>D1已取消发布</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将首次解析为V1</p>
        <p>刷新后，不会解析任何对话框</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>D1参与计数没有变化</p>
        <p>刷新后，D1触发器或参与计数没有变化</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1与D1交互 </p>
        <p>D1已取消发布</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将解析为V1</p>
        <p>刷新后，D1将继续</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>D1参与计数将增加1</p>
        <p>刷新后，由于D1将继续不会进一步更改触发器或参与计数</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，但未响应</p>
        <p>D1已发布，但有新更改</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将首次解析为V1</p>
        <p>刷新后，包含新更改的对话框将被解析</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>刷新后，作为D1，显示了新更改，但没有进一步更改以触发计数</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1仅针对WP1</p>
        <p>V1首次访问WP1</p>
        <p>D1的V1点击提供第一个响应</p>
        <p>D1已发布，但有新更改</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将首次解析为V1</p>
        <p>刷新后，具有旧更改的对话框将继续</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>D1的参与次数将增加1 </p>
        <p>刷新后，将显示旧的D1，因此不会更改触发计数</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1针对具有1个优先级的WP1</p>
        <p>D2针对WP1，具有2个优先级</p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击，但未响应</p>
        <p>D1已取消发布</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将首次解析为V1</p>
        <p>刷新后，D2将解析为V1</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>刷新后，D2的触发器计数将增加1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1针对具有1个优先级的WP1</p>
        <p>D2针对WP1，具有2个优先级 </p>
        <p>V1首次访问WP1</p>
        <p>V1在D1上单击并完成D1</p>
        <p>V1刷新WP1并查看D2<br/>V1在D2上单击并完成D2</p>
        <p>营销人员对D1进行了更改并重新发布</p>
        <p>V1刷新WP1</p>
      </td>
      <td>
        <p>D1将首次解析为V1</p>
        <p>刷新后，D2将解析为V1</p>
        <p>完成D1和D2后，无论发生什么更改或重新发布D1,D2都不会再显示给V1</p>
      </td>
      <td>
        <p>D1的触发器计数、参与计数和已完成计数将增加1</p>
        <p>D2完成后刷新，不执行任何操作</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1针对WP1的“网站逗留时间”触发器为30秒</p>
        <p>V1访问WP1</p>
      </td>
      <td>
        <p>D1将被解析，但不会触发到V1</p>
        <p>30秒后，D1将显示/触发到V1</p>
      </td>
      <td>D1的触发器计数仅在网页花费了30秒以上后，才会增加1秒</td>
    </tr>
    <tr>
      <td>
        <p>D1针对WP1和WP2，触发“页面逗留时间”的触发器为30秒</p>
        <p>V1访问WP1、WP2</p>
      </td>
      <td>
        <p>D1将被解析，但不会触发到V1</p>
        <p>30秒后，D1将显示/触发到V1</p>
      </td>
      <td>D1的触发器计数仅在网页花费了30秒以上后，才会增加1秒</td>
    </tr>
    <tr>
      <td>
        <p>针对WP1的D1触发器为“滚动百分比”为50</p>
        <p>V1访问WP1</p>
      </td>
      <td>
        <p>D1将被解析，但不会触发到V1</p>
        <p>滚动50%后，D1将显示/触发到V1</p>
      </td>
      <td>D1的触发器计数仅在滚动50%后增加1</td>
    </tr>
    <tr>
      <td>
        <p>D1针对具有1个优先级的WP1，事件“页面逗留时间”触发器为30秒</p>
        <p>D2针对WP1，具有2个优先级，事件“页面滚动百分比”为50</p>
        <p>V1访问WP1,10秒后V1访问WP2,V1访问WP1</p>
      </td>
      <td>
        <p>在WP1上，D1将被解析，但不会触发到V1</p>
        <p>在WP2上，D2将被解析，但不会触发到V1</p>
        <p>在WP1上，D1将被解析，20秒后，D1将触发到V1</p>
      </td>
      <td>D1的触发器计数仅在30秒后增加1</td>
    </tr>
    <tr>
      <td>
        <p>D1针对WP1，触发“网站逗留时间”为1分钟</p>
        <p>V1访问WP1 1分钟，显示为D1，但不参与</p>
        <p>V1关闭WP1,2天后返回WP1</p>
      </td>
      <td>
        <p>D1将自动显示给V1，因为它们在上一会话中已满足触发器条件</p>
        <p>同一逻辑将应用于“页面逗留时间”和“页面滚动百分比”</p>
      </td>
      <td>
        <p>D1的触发器计数将增加1</p>
        <p>返回后，不执行任何操作</p>
      </td>
    </tr>
  </tbody>
</table>