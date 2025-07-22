---
description: 默认动态字段映射 — Marketo文档 — 产品文档
title: 默认动态字段映射
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---

# 默认动态字段映射 {#default-dynamics-field-mapping}

当您最初将Marketo Engage帐户与Microsoft同步时，Marketo会自动在内置的Dynamics和Marketo字段之间建立这些关联。  Marketo还将同步您的Leads、Accounts、Opportunities和Contacts上的自定义字段。

## 潜在客户字段 {#lead-fields}

<table>
  <colgroup>
    <col>
    <col>
    <col>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo字段</th>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>[!UICONTROL Created On]</td>
      <td>创建</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL First Name]</td>
      <td>名字</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL Middle Name]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last]</td>
      <td>[!UICONTROL Last Name]</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>电子邮件地址1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Job Title]</td>
      <td>[!UICONTROL Job title]</td>
      <td>工作标题</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobile Phone]</td>
      <td>手机</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fax]</td>
      <td>[!UICONTROL Fax]</td>
      <td>传真</td>
    </tr>
    <tr>
      <td>[!UICONTROL Address]</td>
      <td>[!UICONTROL Street 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL City]</td>
      <td>[!UICONTROL City]</td>
      <td>地址1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL State]</td>
      <td>[!UICONTROL State/Province]</td>
      <td>address1_stateorprovidle</td>
    </tr>
    <tr>
      <td>[!UICONTROL Country]</td>
      <td>[!UICONTROL Country/Region]</td>
      <td>地址1_国家/地区</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postal Code]</td>
      <td>[!UICONTROL Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Source]</td>
      <td>[!UICONTROL Lead Source]</td>
      <td>leadsourcecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>状态代码</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>描述</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do Not Call]</td>
      <td>[!UICONTROL Do Not Allow Phone Calls]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Unsubscribed]</td>
      <td>[!UICONTROL Do not bulk email]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Rating]</td>
      <td>[!UICONTROL Rating]</td>
      <td>leadqualitycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 2]</td>
      <td>[!UICONTROL Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 3]</td>
      <td>[!UICONTROL Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Email]</td>
      <td>[!UICONTROL Do Not Allow Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Do Not Allow Faxes]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Send Marketing Material]</td>
      <td>[!UICONTROL Marketing Material]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Home Phone]</td>
      <td>电话2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Preferred Method Of Contact]</td>
      <td>[!UICONTROL Preferred Method of Contact]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Topic]</td>
      <td>[!UICONTROL Topic]</td>
      <td>主题</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Company Name]</td>
      <td>companyname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Score]</td>
      <td>[!UICONTROL Relative Score]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Priority]</td>
      <td>[!UICONTROL Priority]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgency]</td>
      <td>mkt_urgency</td>
    </tr>
    <tr>
      <td>[!UICONTROL Subject]</td>
      <td>[!UICONTROL Topic]</td>
      <td>主题</td>
    </tr>
    <tr>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>收入</td>
    </tr>
  </tbody>
</table>

以下Lead字段已同步以供内部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>创建</td>
    </tr>
  </tbody>
</table>

## 联系人字段 {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo字段</th>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>[!UICONTROL Created On]</td>
      <td>创建</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL First Name]</td>
      <td>名字</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL Middle Name]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last]</td>
      <td>[!UICONTROL Last Name]</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>电子邮件地址1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Job Title]</td>
      <td>[!UICONTROL Job Title]</td>
      <td>工作标题</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobile Phone]</td>
      <td>手机</td>
    </tr>
    <tr>
      <td>[!UICONTROL Address]</td>
      <td>[!UICONTROL Address 1: Street 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL City]</td>
      <td>[!UICONTROL Address 1: City]</td>
      <td>地址1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL State]</td>
      <td>[!UICONTROL Address 1: State/Province]</td>
      <td>address1_stateorprovidle</td>
    </tr>
    <tr>
      <td>[!UICONTROL Country]</td>
      <td>[!UICONTROL Address 1: Country/Region]</td>
      <td>地址1_国家/地区</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postal Code]</td>
      <td>[!UICONTROL Address 1: Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>状态代码</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do Not Call]</td>
      <td>[!UICONTROL Do Not Allow Phone Calls]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Unsubscribed]</td>
      <td>[!UICONTROL Do not bulk email]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 2]</td>
      <td>[!UICONTROL Address 1: Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 3]</td>
      <td>[!UICONTROL Address 1: Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Email]</td>
      <td>[!UICONTROL Do Not Allow Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Home Phone]</td>
      <td>电话2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Preferred Method Of Contact]</td>
      <td>[!UICONTROL Preferred Method Of Contact]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Send Marketing Material]</td>
      <td>[!UICONTROL Marketing Material]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Priority]</td>
      <td>[!UICONTROL Priority]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgency]</td>
      <td>mkt_urgency</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Score]</td>
      <td>[!UICONTROL Relative Score]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>描述 </td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Score]</td>
      <td>[!UICONTROL Lead Score]</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>描述 </td>
    </tr>
  </tbody>
</table>

以下Contact字段已同步以供内部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>创建</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company Name]</td>
      <td>parentcustomerid</td>
    </tr>
  </tbody>
</table>

## 帐户字段 {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo字段</th>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Account (a)]</td>
      <td>[!UICONTROL Account]</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Address]</td>
      <td>[!UICONTROL Address 1: Street 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing City]</td>
      <td>[!UICONTROL Address 1: City]</td>
      <td>地址1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Country]</td>
      <td>[!UICONTROL Address 1: Country/Region]</td>
      <td>地址1_国家/地区</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Postal Code]</td>
      <td>[!UICONTROL Address 1: Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Billing Address 2]</td>
      <td>[!UICONTROL Address 1: Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Billing Address 3]</td>
      <td>[!UICONTROL Address 1: Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Main Phone]</td>
      <td>[!UICONTROL Main Phone]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Business Type]</td>
      <td>[!UICONTROL Business Type]</td>
      <td>businesstypecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Account Number]</td>
      <td>[!UICONTROL Account Number]</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Company Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>收入</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>描述</td>
    </tr>
    <tr>
      <td>[!UICONTROL Industry]</td>
      <td>[!UICONTROL Industry]</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC Code]</td>
      <td>[!UICONTROL SIC Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Website]</td>
      <td>[!UICONTROL Website]</td>
      <td>网站</td>
    </tr>
    <tr>
      <td>[!UICONTROL Num Employees]</td>
      <td>[!UICONTROL Number of Employees]</td>
      <td>女性人数</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC Code]</td>
      <td>[!UICONTROL SIC Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Account Name]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Num Employees]</td>
      <td>[!UICONTROL Number of Employees]</td>
      <td>女性人数</td>
    </tr>
  </tbody>
</table>

以下“帐户”字段已同步以供内部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>创建</td>
    </tr>
  </tbody>
</table>

## 机会字段 {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo字段</th>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Close Probability]</td>
      <td>[!UICONTROL Probabliity]</td>
      <td>关闭概率</td>
    </tr>
    <tr>
      <td>[!UICONTROL Stage]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Actual Close Date]</td>
      <td>[!UICONTROL Actual Close Date]</td>
      <td>actualclosedate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Name]</td>
      <td>[!UICONTROL Topic]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estimated Value]</td>
      <td>[!UICONTROL Est. Revenue]</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL Description]</td>
      <td>[!UICONTROL Description]</td>
      <td>描述</td>
    </tr>
  </tbody>
</table>

以下“帐户”字段已同步以供内部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics字段</th>
      <th>MS Dynamics API名称</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Opportunity]</td>
      <td>opportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL Potential Customer]</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Marketo中与Microsoft相关的系统字段（只读） {#microsoft-related-system-fields}

以下字段是在Marketo中创建的，但用户无法对其进行调整。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo字段</th>
      <th>描述</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Type]</td>
      <td>潜在客户或联系人。 如果为空，则商机在Marketo中仅作为人员存在</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>日期创建于[!DNL MS Dynamics] (可能不同于在Marketo中创建)</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft is Deleted]</td>
      <td>此人以前在Microsoft中，但现在已被删除，仅居住在Marketo中</td>
    </tr>
  </tbody>
</table>
