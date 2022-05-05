---
description: 正在同步调用和调用关键消息 — Marketo文档 — 产品文档
title: 正在同步呼叫和呼叫密钥消息
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# 正在同步呼叫和呼叫密钥消息 {#syncing-call-and-call-key-messages}

默认情况下，Veeva CRM中的调用和调用关键消息对象会同步到Marketo Engage。 Marketo会根据呼叫日期同步最长6个月的数据。

>[!NOTE]
>
>Marketo将保留自呼叫日期起最长六个月的呼叫数据。

**哪些触发器/过滤器与调用和调用密钥消息相关？**

触发器：

* 已添加到调用
* 从调用中删除
* 已添加到调用密钥消息
* 从调用密钥消息中删除
* 更新的调用
* 更新了呼叫密钥消息

过滤器：

* 具有调用
* 有呼叫密钥消息

调用和调用密钥消息的以下字段会同步，并可用作约束和触发器。

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        对象
      </th>
      <th>
        字段标签
      </th>
      <th>
        描述
      </th>
      <th>
        字段名称
      </th>
      <th>
        数据类型
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>调用</td>
      <td>会计</td>
      <td>与调用关联的帐户的查找。</td>
      <td>Account_vod__c</td>
      <td>查找（帐户）</td>
    </tr>
    <tr>
      <td>调用</td>
      <td>调用类型</td>
      <td>根据呼叫类型和内容进行系统维护的呼叫类型。 此字段用于报告。 有效值为：仅详细信息、带示例的详细信息、组详细信息、带示例的组详细信息、仅示例。 不应更改这些值，但可能会更改这些选取列表的转换。 与会者的呼叫类型与标题呼叫相同。 对于有3名专业人员的组呼叫，所有4条记录的呼叫类型都为“组详细信息”</td>
      <td>Call_Type_vod__c</td>
      <td>挑库</td>
    </tr>
    <tr>
     <td>调用</td>
      <td>联系人</td>
      <td>查找与呼叫关联的联系人（如果有）。</td>
      <td>Contact_vod__c</td>
      <td>查找（联系人）</td>
    </tr>
    <tr>
      <td>调用</td>
      <td>日期</td>
      <td>首次保存或提交调用的日期。 如果未提供日期或日期时间字段，则通过触发器将此字段设置为当前日期。</td>
      <td>Call_Date_vod__c</td>
      <td>日期</td>
    </tr>
    <tr>
      <td>调用</td>
      <td>详细产品</td>
      <td>用于显示调用详细产品列表的帮助程序字段。 产品名称应使用双空格分隔，并按从左到右的优先级顺序排列。 此字段不控制处理，包含此字段可使相关列表和报表更加用户友好。</td>
      <td>Detailed_Products_vod__c</td>
      <td>文本区域(255)</td>
    </tr>
    <tr>
      <td>调用</td>
      <td>父调用吗？</td>
      <td>公式字段来确定“呼叫”记录是“父呼叫”还是“与会者呼叫”记录。 1表示该记录为父调用。 0表示它是“与会者呼叫”。</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>公式（数字）</td>
    </tr>
    <tr>
      <td>调用</td>
      <td>状态</td>
      <td>呼叫的状态 — 已计划、已保存或已提交。 使用翻译工作台更改显示值。 呼叫时触发器会查看此字段，以查看呼叫是否已锁定（已提交）。 按“保存”或“提交”按钮时，将为用户设置此值。</td>
      <td>Status_vod__c</td>
      <td>挑库</td>
    </tr>
    <tr>
      <td>调用</td>
      <td>记录类型</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>记录类型</td>
    </tr>
    <tr>
      <td>调用密钥消息</td>
      <td>调用</td>
      <td>调用的查找。 每个键消息都与一个调用关联。</td>
      <td>Call2_vod__c</td>
      <td>主控详细信息（调用）</td>
    </tr>
    <tr>
      <td>调用密钥消息</td>
      <td>类别</td>
      <td>记录消息的消息类别。 主要用于报表。</td>
      <td>Category_vod__c</td>
      <td>挑库</td>
    </tr>
    <tr>
      <td>调用密钥消息</td>
      <td>CLM演示文稿名称</td>
      <td>加盖CLM的演示名称</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>调用密钥消息</td>
      <td>关键消息名称</td>
      <td>带盖章的密钥消息名称</td>
      <td>Key_Message_Name_vod__c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>调用密钥消息</td>
      <td>产品名称</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>公式（文本）</td>
    </tr>
    <tr>
      <td>调用密钥消息</td>
      <td>反应</a>
      </td>
      <td>对消息的反应选择表。 编辑选取列表以更改反应值。</td>
      <td>Reaction_vod__c</td>
      <td>挑库</td>
    </tr>
  </tbody>
</table>
