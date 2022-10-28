---
description: 实践发行说明 — Marketo文档 — 产品文档
title: 实践发行说明
hide: true
hidefromtoc: true
source-git-commit: f57bb27c1b33e1c47c69f68c3719a35ee3f2d82e
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 2%

---

# 发行说明：2022年10月 {#release-notes-oct-22}

在下面，您将找到’22年10月版中包含的所有功能。 查看您的Adobe Marketo Engage版本以了解功能的可用性。

>[!AVAILABILITY]
>
>由星(![星星](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

将在 **2022年10月14日**，并在随后的几周内分阶段推出其余功能（除非另有指定）。 发行功能和确切日期可能会发生更改。

## 跨渠道编排 {#cross-channel-orchestration}

_**动态聊天**_

* **为动态聊天自动排列对话框流**:通过按“自动排列”按钮，将画布上的所有内容整理为简洁且易于阅读的格式，从而改善您拥挤的对话框画布。

* **支持动态聊天的其他数据类型**:三种新的Marketo Engage类型（布尔、整数、浮点）允许您在动态聊天中利用更多现有的数据字段，进行诸如基于分数进行定位或询问访客是/否问题之类的操作。

* **用于动态聊天的会议链接**:在发送给访客的每个日历邀请中自动包含Google和Outlook的“团队”或“会面”链接的选项。

* **用于动态聊天的计划会议通知**:销售代表会收到有关计划会议的自动电子邮件通知以及有关访客聊天机器人交互的任何相关信息。

* **动态聊天的角色和权限**:管理员可以使用粒度权限控制应用程序的可见性和使用情况，并创建自定义用户角色。

   * 完全访问 — 用户可以充分利用该功能（例如，发布对话框、更改颜色方案等）
   * 只读访问权限 — 用户可以查看信息但无法更改（例如，查看受众标准或流设计器，但不能更改）
   * 访问受限 — 用户无法查看或访问配置或集成部分

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发运</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

## 新一代体验 {#next-generation-experience}

* **更新了下一代体验中的屏幕**:我们将在下一代体验中提供额外的刷新屏幕，这些屏幕提供了可通过切换开关访问的更新设计和可用性增强功能：

   * 登陆页面模板详细信息
   * 电子邮件模板列表

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发运</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md">切换开关</a></td>
  </tr>
  </tbody>
</table>

* **增强了“电子邮件模板详细信息”中的“使用者”选项卡**:在新体验中，您将看到与使用电子邮件模板的资产相关的其他信息，包括资产状态、上次修改时间和上次修改时间。 您还可以搜索、排序和过滤资产使用的列表。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发运</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

* **报表资产过滤器模型**:报表配置模型的新设计，在配置菜单中显示新的资产树，并为创建和修改日期设置筛选器。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发运</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

## 营销数据环境 {#marketing-data-environment}

* **AdobePrivacy Service集成**:与Privacy Service协调，以自动跨Experience Cloud产品遵守数据隐私法规。 目前，此服务仅适用于已载入AdobeIdentity Management系统的Marketo Engage客户。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发运</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">AdobeIdentity Management</a></td>
  </tr>
  </tbody>
</table>

## API增强功能 {#api-enhancements}

* **批量潜在客户导入：销售人员关联**:与潜在客户REST API对等，以便能够在批量潜在客户导入过程中将潜在客户与销售人员关联，从而降低复杂性和所需API调用数。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发运</td>
   <td><a href="https://developers.marketo.com/rest-api/bulk-import/bulk-lead-import/">批量导入潜在客户</a></td>
  </tr>
  </tbody>
</table>

## 销售分析 {#sales-insight}

![（星号）](assets/yellow-star.png)

* **Sales Insight与动态聊天的集成**:分析功能板现在包括智能网格中的动态聊天活动，以及每周摘要和详细信息卡片。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发运</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">动态聊天集成</a></td>
  </tr>
  </tbody>
</table>

## 公告 {#announcements}

* **Forms 1.0**:Forms 1.0的弃用将在10月版中完成。 Forms 1.0资产将无法再向Marketo Engage提交数据，如果尝试，则将返回错误。

* **无脚本Forms**:在浏览器中禁用Javascript后，Forms将无法再正常运行。 表单提交将要求启用Javascript。
