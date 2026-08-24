---
description: AWS迁移 — Marketo Engage文档 — 产品文档
title: AWS迁移
feature: Getting Started
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 034bb35c7f1d46fb001c5380947f563d130b5ab9
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 5%

---

# AWS迁移 {#aws-migration}

在接下来的几个月中，所有Marketo Engage订阅都将从专用数据中心迁移到AWS公共云，以提高可靠性、可扩展性和速度。

您将在迁移前约30天收到电子邮件以及应用程序内通知。 使用本指南进行准备。

## 建议的操作 {#actions}

在迁移期间，所有Marketo Engage服务将不可用。 我们建议您采取以下步骤来减轻对您的业务产生的任何影响。

* **避免创建或更新潜在客户/人员**，或避免运行修改人员记录的进程。

* **不触发后续流程**，因为计划的营销活动将暂停。

* **暂时禁用向Marketo Engage发送数据或从中接收数据的任何集成**。

* **避免运行**&#x200B;数据导入或导出或任何主要的潜在客户/人员生成营销活动。

* **审核并更新IP**&#x200B;登录、API访问、电子邮件发送、Web跟踪和集成。

* **添加新IP地址**&#x200B;并保留您当前的IP不变。 通过下面[&#128279;](#ip-addresses)的表查看要添加的IP地址。

## 预期的服务影响 {#impacts}

您无需对以下影响执行任何操作。

* **CRM集成和LaunchPoint服务**&#x200B;将被禁用，但以后应自动恢复。
* **登陆页面、表单和数据收集**&#x200B;将不可用，并且将改为显示维护消息。

>[!NOTE]
>
>如果您使用[外部表单](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}，并且希望避免丢失在Marketo Engage在迁移期间不可用时收集的表单提交数据，请提前联系[Adobe支持](https://experienceleague.adobe.com/en/support){target="_blank"} **至少两个工作日**，并提供表单ID和您的订阅Munchkin ID。

## 识别您的数据中心/面板 {#identify}

在查看以下表格之前，[了解如何识别](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify)您的订阅所在的数据中心和面板/服务器。

## 计划 {#schedule}

新的日期和数据中心/面板信息会定期添加或更改，因此请监视此计划的更新。

+++7月计划
<table>
 <tbody>
  <tr>
   <th style="width:25%">日期</th>
   <th style="width:25%">数据中心/面板</th>
   <th style="width:25%">时间</th>
   <th style="width:25%">状态</th>
  </tr>
  <tr>
   <td>2026年7月8日</td>
   <td>AB69<br>
   AB64</td>
   <td>下午5点（太平洋夏令时间）<br>
   下午6点（太平洋夏令时间）</td>
   <td>已完成<br>
   已完成</td>
  </tr>
  <tr>
   <td>2026年7月9日</td>
   <td>AB70</td>
   <td>下午5点（太平洋夏令时间）</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月11日</td>
   <td>AB46</td>
   <td>上午10:00（太平洋夏令时间）</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月13日</td>
   <td>NLD101</td>
   <td>上午10:00（太平洋夏令时间）</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月15日</td>
   <td>NLD102<br>
   NLD104</td>
   <td>上午10:00（太平洋夏令时间）<br>
   上午11:00（太平洋夏令时间）</td>
   <td>已完成<br>
   已完成</td>
  </tr>
  <tr>
   <td>2026年7月17日</td>
   <td>NLD103<br>
   NLD105</td>
   <td>上午10:00（太平洋夏令时间）<br>
   上午11:00（太平洋夏令时间）</td>
   <td>已完成<br>
   已完成</td>
  </tr>
  <tr>
   <td>2026年7月21日</td>
   <td>AB54</td>
   <td>下午5点（太平洋夏令时间）</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月23日</td>
   <td>AB48</td>
   <td>下午5点（太平洋夏令时间）</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月31日</td>
   <td>AB43</td>
   <td>下午3点（太平洋夏令时间）</td>
   <td>已完成</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">日期</th>
   <th style="width:25%">数据中心/面板</th>
   <th style="width:25%">时间</th>
   <th style="width:25%">状态</th>
  </tr>
  <tr>
   <td>2026年8月12日</td>
   <td>AB61<br>
   AB17</td>
   <td>下午3点（太平洋夏令时间）<br>
   下午4点（太平洋夏令时间）</td>
   <td>已完成<br>
   已完成</td>
  </tr>
  <tr>
  <td>2026年8月13日</td>
   <td>AB68</td>
   <td>下午4点（太平洋夏令时间）</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年8月20日</td>
   <td>AB42<br>
   <i>AB44</i></td>
   <td>下午5点（太平洋夏令时间）<br>
   下午<i>6点PDT</i></td>
   <td>已完成<br>
   <i>已延迟（日期待定）</i></td>
  </tr>
  <tr>
   <td>2026年8月26日</td>
   <td><i>AB40</i><br>
   AB50</td>
   <td>下午<i>5 PDT</i><br>
   下午6点（太平洋夏令时间）</td>
   <td><i>已延迟（日期待定）</i><br>
   按计划进行</td>
  </tr>
  <tr>
   <td>2026年8月28日</td>
   <td><i>AB53</i><br>
   AB56</td>
   <td><i>下午3点PDT</i><br>
   下午4点（太平洋夏令时间）</td>
   <td><i>已延迟（日期待定）</i><br>
   按计划进行</td>
  </tr>
  <tr>
   <td>2026年9月8日</td>
   <td>AB01<br>
   AB02</td>
   <td>下午5点（太平洋夏令时间）<br>
   下午6点（太平洋夏令时间）</td>
   <td>按计划进行<br>
   按计划</td>
  </tr>
  <tr>
   <td>2026年9月10日</td>
   <td>AB03<br>
   <i>AB04</i></td>
   <td>下午5点（太平洋夏令时间）<br>
   下午<i>6点PDT</i></td>
   <td>按计划进行<br>
   <i>已延迟（日期待定）</i></td>
  </tr>
  <tr>
   <td>2026年9月15日</td>
   <td>AB05<br>
   AB06</td>
   <td>下午5点（太平洋夏令时间）<br>
   下午6点（太平洋夏令时间）</td>
   <td>按计划进行<br>
   按计划</td>
  </tr>
  <tr>
   <td>2026年9月17日</td>
   <td>AB07<br>
   AB08</td>
   <td>下午5点（太平洋夏令时间）<br>
   下午6点（太平洋夏令时间）</td>
   <td>按计划进行<br>
   按计划</td>
  </tr>
  <tr>
   <td>2026年9月22日</td>
   <td>AB09<br>
   AB12</td>
   <td>下午5点（太平洋夏令时间）<br>
   下午6点（太平洋夏令时间）</td>
   <td>按计划进行<br>
   按计划</td>
  </tr>
  <tr>
   <td>2026年9月25日</td>
   <td>AB10<br>
   AB11</td>
   <td>下午4点（太平洋夏令时间）<br>
   下午5点（太平洋夏令时间）</td>
   <td>按计划进行<br>
   按计划</td>
  </tr>
  </body>
</table>

## 要添加的IP地址 {#ip-addresses}

根据您的数据中心，与您的IT部门合作，添加各自的IP地址。

<table>
<tbody>
<tr>
  <th style="width:25%">数据中心</th>
  <th style="width:75%">IP地址</th>
</tr>
<tr>
  <td>AB</td>
  <td>54.160.246.246<br>
  54.237.141.197<br>
  52.20.211.99</td>
</tr>
<tr>
  <td>NLD</td>
  <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
</tr>
</body>
</table>

## 更新和支持 {#support}

有关最新更新，请将此页加入书签。 如果您有任何问题，请通过Admin Console或[Experience League](https://experienceleague.adobe.com/en/support){target="_blank"}中的支持门户联系Adobe支持部门。

## 常见问题解答 {#faq}

**数据存储在何处？**
所有Marketo用户数据都存储在Amazon Web Services (AWS)上。 Marketo已将其基础架构从自有物理数据中心迁移到AWS的企业级云平台。

**个人数据具体存储在哪里？**
个人数据存储在AWS完全托管的关系数据库服务Amazon Aurora中。 Aurora在AWS地区的三个独立可用区中以六种方式复制数据，以保护个人数据免受硬件故障、存储降级和本地化基础架构事件的影响。

**谁拥有存储环境？**
该存储基础架构由Amazon Web Services (AWS)拥有和运营。 Adobe (Marketo)作为AWS的客户运行，采用共同责任模式：AWS负责基础基础架构的安全性和可用性，而Adobe负责其中运行的数据和应用程序的安全性。

**有关生产、备份/灾难恢复位置和存储技术的完整详细信息是什么？**
Marketo使用Amazon Aurora（完全由AWS管理的云原生关系数据库引擎）作为其主要数据库技术。 Aurora将计算和存储分离，以六种方式在生产区域中的三个可用区之间自动复制数据，并且需要四个拷贝的法定数量来确认任何写入操作。

Aurora还实时执行到Amazon S3的连续、自动备份，从而能够在配置的保留时间范围内随时进行时间点恢复(PITR)。

目前，Marketo的Aurora部署在单个AWS区域内运行，无需跨区域复制。 生产数据保留在指定的区域基础架构中，灾难恢复通过Aurora的多可用区存储冗余和连续备份提供，而不是通过地理故障切换到辅助区域。 随着Marketo的AWS基础设施的成熟，可以进一步评估此情况。
