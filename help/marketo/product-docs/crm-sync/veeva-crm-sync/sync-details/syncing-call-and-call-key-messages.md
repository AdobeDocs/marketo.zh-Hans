---
description: 同步调用和调用关键消息 — Marketo文档 — 产品文档
title: 同步呼叫与呼叫关键消息
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 6%

---

# 同步呼叫与呼叫关键消息 {#syncing-call-and-call-key-messages}

默认情况下，[!DNL Veeva] CRM中的Call和Call键消息对象同步到Marketo Engage。 Marketo会根据呼叫创建日期同步长达6个月之前的数据。

>[!NOTE]
>
>Marketo会保留呼叫数据，自呼叫之日起最多六个月。

**与呼叫和呼叫关键消息相关的触发器/过滤器是什么？**

触发器：

* 已添加至呼叫
* 从调用中删除
* 已添加到呼叫关键消息
* 从呼叫密钥消息中删除
* 已更新呼叫
* 已更新呼叫密钥消息

过滤器：

* 具有呼叫
* 具有呼叫键消息

已同步调用和调用密钥消息中的以下字段，这些字段可用作约束和触发器。

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
      <td>号召</td>
      <td>会计师</td>
      <td>查找与呼叫关联的帐户。</td>
      <td>Account_vod__c</td>
      <td>查找（帐户）</td>
    </tr>
    <tr>
      <td>号召</td>
      <td>呼叫类型</td>
      <td>系统根据调用的类型和内容维护的调用的类型。 此字段用于报告目的。 有效值为：仅限详细信息、包含示例的详细信息、组详细信息、包含示例的组详细信息、仅限示例的组详细信息。 不应更改这些值，但可以更改这些选取列表的翻译。 与会者的呼叫类型与标头呼叫相同。 对于由3名专业人员组成的组呼叫，所有4条记录的呼叫类型为“组详细信息”</td>
      <td>Call_Type_vod__c</td>
      <td>选取列表</td>
    </tr>
    <tr>
     <td>号召</td>
      <td>联系人</td>
      <td>查找与呼叫关联的联系人（如果有）。</td>
      <td>Contact_vod__c</td>
      <td>查找（联系人）</td>
    </tr>
    <tr>
      <td>号召</td>
      <td>日期</td>
      <td>首次保存或提交呼叫的日期。 如果日期或日期时间字段均未提供，则通过触发器将此字段设置为当前日期。</td>
      <td>Call_Date_vod__c</td>
      <td>日期</td>
    </tr>
    <tr>
      <td>号召</td>
      <td>是家长电话吗？</td>
      <td>用于确定呼叫记录是父呼叫还是与会者呼叫记录的公式字段。 1表示该记录为父呼叫。 0表示这是与会者呼叫。</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>公式（数字）</td>
    </tr>
    <tr>
      <td>号召</td>
      <td>状态</td>
      <td>呼叫的状态 — “已计划”、“已保存”或“已提交”。 使用折算工作台更改显示值。 调用时触发器查看此字段，以查看调用是否已锁定（提交）。 此值在按下“保存”或“提交”按钮时为用户设置。</td>
      <td>Status_vod__c</td>
      <td>选取列表</td>
    </tr>
    <tr>
      <td>号召</td>
      <td>记录类型</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>记录类型</td>
    </tr>
    <tr>
      <td>呼叫关键消息</td>
      <td>号召</td>
      <td>查找呼叫。 每个关键消息都与呼叫相关联。</td>
      <td>Call2_vod__c</td>
      <td>Master-Detail（调用）</td>
    </tr>
    <tr>
      <td>呼叫关键消息</td>
      <td>类别</td>
      <td>记录消息的消息类别。 主要用于报表。</td>
      <td>Category_vod__c</td>
      <td>选取列表</td>
    </tr>
    <tr>
      <td>呼叫关键消息</td>
      <td>CLM演示文稿名称</td>
      <td>带戳的CLM演示文稿名称</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>呼叫关键消息</td>
      <td>关键消息名称</td>
      <td>带戳的密钥消息名称</td>
      <td>Key_Message_Name_vod__c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>呼叫关键消息</td>
      <td>产品名称</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>公式（文本）</td>
    </tr>
    <tr>
      <td>呼叫关键消息</td>
      <td>反应</a>
      </td>
      <td>消息反应的选取列表。 编辑选取列表以更改反应值。</td>
      <td>Reaction_vod__c</td>
      <td>选取列表</td>
    </tr>
  </tbody>
</table>
