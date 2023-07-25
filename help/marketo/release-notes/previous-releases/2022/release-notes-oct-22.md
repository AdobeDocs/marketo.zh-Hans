---
description: 发行说明 — 2022年10月 — Marketo文档 — 产品文档
title: 发行说明 — 2022年10月
exl-id: 1494b8b9-049c-4969-ab95-a4be41d886b0
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 2%

---

# 发行说明：2022年10月 {#release-notes-oct-22}

在下方，您会找到2022年10月版本中包含的所有功能。 查看Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![星形](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，并将于以下日期开始发行 **2022年10月14日**，在接下来的几周内分阶段推出剩余的功能。 发行功能和日期可能会有变动。 请检查每个功能下方的状态。

### 营销数据环境 {#marketing-data-environment}

</br>

* **项目群成员自定义字段同步**：能够双向同步为项目群成员捕获的可扩展字段（例如，在活动注册期间的与会者偏好，如食物、会话、曲目等） 使用Salesforce中的Campaign成员字段。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">项目群成员自定义字段同步</a></td>
  </tr>
  </tbody>
</table>

* **AdobePrivacy Service集成**：与Privacy Service协调以跨Experience Cloud产品自动遵守数据隐私法规。 目前，此服务仅适用于已载入AdobeIdentity Management System的Marketo Engage客户。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">AdobeIdentity Management</a></td>
  </tr>
  </tbody>
</table>

### 新一代体验 {#modern-ux}

</br>

* **更新了下一代体验中的屏幕**：我们将在下一代体验中提供更多、刷新的屏幕，这些屏幕提供更新的设计和可用性增强功能，可通过切换开关访问：

   * 登陆页面模板详细信息
   * 电子邮件模板列表

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">切换开关</a></td>
  </tr>
  </tbody>
</table>

* **电子邮件模板详细信息中的“增强的使用者”选项卡**：在新Experience中，您将看到与使用电子邮件模板的资产相关的其他信息，包括资产状态、上次修改时间和上次修改者。 您还可以搜索、排序和筛选资源使用的列表。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

* **报表资源筛选模式**：新的报表配置模式设计，在配置菜单中显示了新的资源树，并筛选了创建和修改日期。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

### API增强功能 {#api-enhancements}

</br>

* **批量销售线索导入：销售人员关联**：与Lead REST API实现对等性，以便在批量商机导入过程中将商机与销售人员关联，从而减少所需的API调用的复杂性和次数。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td><a href="https://developers.marketo.com/rest-api/bulk-import/bulk-lead-import/">批量商机导入</a></td>
  </tr>
  </tbody>
</table>

### 销售分析 {#sales-insight}

</br>

![(star)](assets/yellow-star.png)

* **Sales Insight与Dynamic Chat集成**：分析功能板现在包括智能网格中的Dynamic Chat活动，以及每周摘要和详细信息卡。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Dynamic Chat集成</a></td>
  </tr>
  </tbody>
</table>

## Agile版本功能

以下功能遵循Agile格式，并在标准发布日期之前或之后的各种日期发布。 请检查每个功能下方的状态。

* **自动排列用于Dynamic Chat的对话框流**：通过按按钮通过“自动排列”，将画布上的所有内容整理为干净且易于阅读的格式，从而改进拥挤的对话框画布。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md#stream-designer-icons">流设计器图标</a></td>
  </tr>
  </tbody>
</table>

* **Dynamic Chat的会议链接**：用于在发送给访客的每个日历邀请中自动包含Google和Outlook的“团队”或“会议”链接的选项。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md">日程表</a></td>
  </tr>
  </tbody>
</table>

* **支持Dynamic Chat的其他数据类型**：三种新数据类型（布尔值、整数、浮点数）允许您利用Dynamic Chat中更多的现有Marketo Engage字段来解答诸如根据得分定位或询问访客是/否问题。

<table> 
  <tr> 
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr> 
   <td>已发货</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

## 公告 {#announcements}

* **Forms 1.0**：Forms 1.0的弃用操作将在10月版本中完成。 Forms 1.0资源将不再能够向Marketo Engage提交数据，如果尝试，则将返回错误。

* **无脚本Forms**：在浏览器中禁用Javascript后，Forms将无法再正常运行。 提交表单需要启用Javascript。
