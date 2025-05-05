---
unique-page-id: 4719093
description: Web区段 — Marketo文档 — 产品文档
title: Web区段
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '2051'
ht-degree: 0%

---

# Web区段 {#web-segments}

## 查看区段 {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

区段选项卡会显示您根据各种属性设置的所有自定义区段。  **区段是符合“设置区段”页面中定义的指定条件的访客集合。**&#x200B;区段可以是来自特定行业、位置或基于访客现场活动的访客。

在Web Personalization中，访客可以匹配多个区段。 例如，如果有针对美国访客的区段和针对金融公司的区段，则来自美国银行的Web访客将匹配&#x200B;**美国访客的区段和针对金融公司的区段**。

**图形：**&#x200B;区段页面根据区段的访客数（y轴）和区段名称（x轴）显示选定区段的条形图。

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">名称</th> 
   <th colspan="1" rowspan="1">描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>名称</strong></td> 
   <td colspan="1" rowspan="1">区段的标题</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>匹配</strong></p></td> 
   <td colspan="1" rowspan="1">符合区段的自定义已定义标准的访客数</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>设置营销活动</strong></td> 
   <td colspan="1" rowspan="1">允许您设置与所选搜索词关联的Campaign CTA</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>访客</strong></td> 
   <td colspan="1">与所选搜索词关联的访客表预览</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>点击流</strong></td> 
   <td colspan="1" rowspan="1">显示一个表，其中包含访客在网站上的活动和URL路径以及他们访问每个页面的时间 </td> 
  </tr> 
 </tbody> 
</table>

请参阅[如何创建和查看区段标签](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**区段 — 右侧面板**

![](assets/image2014-11-12-10-3a46-3a32.png)

在表中选择区段会在右侧面板中显示有关该区段的更多详细信息。

这些详细信息包括：

* 区段名称
* 区段的创建日期
* 显示与该区段一起运行的营销活动的关联营销活动。 单击反应数将会转到营销活动页面，其中显示该区段的营销活动CTA（行动号召）
* 区段的匹配次数（符合区段标准的访客数）以及与区段匹配的独特（独特）访客数。 单击独特访客链接会转到显示区段结果的访客页面
* 区段的所有者/用户创建者
* 与区段关联的域站点
* 区段选定标准的简短摘要

## 启用或禁用区段 {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

要启用或禁用区段，请选中表中该区段的复选框，然后在表底部的“选择操作”下拉框中，选择操作“启用”或“禁用”。 禁用区段后，“状态”列下将显示“禁用”一词。

## 创建区段 {#create-segments}

您创建的区段符合您在&#x200B;**设置区段**&#x200B;页面中定义的任何特定条件。 您也可以根据条件的组合自定义区段，以定位营销活动中的特定受众。

创建新区段

从&#x200B;**区段**&#x200B;页面，单击图形下的&#x200B;**新建**。 出现以下屏幕。

![](assets/four.png)

定义区段的常规参数：

* **名称：**&#x200B;命名您的区段。
* **描述：**&#x200B;提供区段条件的更详细说明。
* **域：**&#x200B;选择要包含在区段中的域。
* **区段规则逻辑：**&#x200B;选择AND / OR逻辑以生成每个区段属性
* **计时：**&#x200B;定义您希望在营销活动中的访客参与度级别

   * **登入点**：来自访问网站的访客的参与
   * **第1次至第9次点击后**：与访客进行特定次数的网站点击

>[!TIP]
>
>**区段规则逻辑**
>
>有三个过滤器选项：
>
>1. 使用所有筛选器（1和2及3...）
>1. 使用任意过滤器（1或2或3...）
>1. 高级过滤器（使用和/或表达式）
>
>    高级过滤器允许您控制区段条件。 输入以“and”和“or”分隔的过滤器编号。
>
>    * 1和2及3
>    * 1或2或3
>
>    将“and”和“or”混合在一起需要用括号来阐明逻辑意图。 例如，“1或2和3”必须编写为以下内容之一：
>
>    * 1和（2或3）
>    * （1和2）或3
>
>    对于更复杂的逻辑，可以接受嵌套括号，例如
>
>    * （1和2）或（3和4）
>    * 1和(2或（3和4）)
>
>    在插入、删除或重新排序任何内容后，检查您的逻辑。

将区段属性从右侧列拖放到左侧的区段编辑器中：

![](assets/five.png)

### Firmographics {#firmographics}

**位置**

将&#x200B;**位置**&#x200B;拖放到区段编辑器中。

* 从以下参数中选择：

   * **包含** — 选择您希望营销活动包含还是排除位置。
   * **选择要添加的国家/地区** — 从下拉框中，选择要包含在区段中的国家/地区。 国家/地区名称显示在右侧。 您可以选择多个国家/地区。

添加国家/地区后，您还可以指定区段的州/省、城市和邮政编码。

* **选择要添加的州或省** — 从下拉框中，选择要包括的美国州或加拿大省。 您可以进行多个选择。
* **邮政编码** — 输入要包含在区段中的邮政编码。
* **城市** — 输入您要包含的一个或多个城市。 在城市之间使用分号。

>[!TIP]
>
>**我应选择哪些区段条件？ “AND”或“OR”？** OR作为每个字段中的附加选项。 潜在客户只需满足在每个字段内选择的多个标准中的一个标准，即可获得该区段的资格。 （例如，潜在客户可能来自美国&#x200B;*或来自国防工业*）。 AND函数作为此区段必须满足的附加必需参数。 （例如，潜在客户必须既来自美国，也来自国防工业）。 在每个分段用户档案中，每个单独的字段都可用作两个字段，即“AND”或“OR”，具体取决于所选的区段条件。

**行业**&#x200B;在&#x200B;**个人资料分段**&#x200B;部分下，选中&#x200B;**行业**&#x200B;旁边的框。

* 从以下参数中选择：

   * **包括** — 选择您希望该区段包括还是排除某个行业。
   * **选择要添加的行业** — 选择要包含在区段中的行业。 行业出现在下拉框的下方。 您可以选择多个行业。

**组织组**

在&#x200B;**配置文件分段**&#x200B;部分下，选中&#x200B;**组织组**&#x200B;旁边的复选框。

* 从下拉框中，从以下选项中选择：

   * 财富500强 — 仅包括此部分中的财富500强公司
   * Fortune 1000 — 仅包括Fortune 1000在此分类中的公司
   * 全球2000强 — 将全球2000强公司包括在此部分
   * 企业 — 包括员工超过1,000人且收入超过2.5亿美元的组织
   * SMB — 仅包括此部门中的中小型企业

**个命名帐户 —**

**组织**

* **来自这些公司（特定名称）**

   * 从“选择要添加的公司”下拉列表中选择要定位的公司。
   * 您可以键入要定位的确切组织名称。 *建议&#x200B;_始终_&#x200B;使用指定帐户列表，而不是手动键入名称以获得更好的匹配（请参阅下文）。

**命名帐户列表**

从[命名帐户列表](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)中选择分段键目标帐户。

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>命名帐户列表名称旁边方括号中的数字被用作Web Personalization [读取API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/javascriptapi/web-personalization)列表的索引引用。

**排除ISP**

该区段不包括Internet服务提供商(ISP)。

### 已知人员 {#known-people}

**数据库**

Web Personalization与您的Marketo数据库集成，允许您按已知人员属性和数据来细分和个性化营销活动。

选择数据库，然后从下拉列表中选择人员数据字段。 从下拉列表中选择&#x200B;**+**&#x200B;以添加字段。

![](assets/seven.png)

您可以在“帐户设置”>“数据库”中添加或删除人员数据字段

>[!TIP]
>
>根据Marketo人员的所有人员数据字段（如职务、分数、角色等）创建区段标准。
>
>例如 “职位等于CMO”和“得分小于或等于50”

**Marketo电子邮件促销活动**&#x200B;通过访客点击Marketo电子邮件并到达网站时的电子邮件反向链接，对促销活动进行细分和个性化。 按Marketo项目名称或营销活动名称进行分段，并继续通过电子邮件到Web的对话。 选择+以从下拉列表中添加字段。

![](assets/image2015-5-27-17-3a20-3a34.png)

**状态**

根据潜在客户的状态定义您的区段：已知或匿名。

* 已知 — 从已知访客的下拉框中选择此选项。 当访客在您的网站上提交表单并出现在Web Personalization的“人员”页面中时，即为已知访客。
* 匿名 — 从匿名访客的下拉框中选择此选项。

![](assets/image2015-5-27-17-3a23-3a2.png)

### 行为 {#behavioral}

**访问 —**&#x200B;根据访客行为或身份定义区段。

* 访问次数 — 从下拉框中选择此选项，以指定潜在客户在网站上的访问次数。

   * 从下拉框中选择等于、等于或大于，或者等于或小于。

* 特定访问次数 — 从下拉列表中选择此选项，以指定特定访客。

   * 在右侧的文本框中，输入要跟踪的访客编号。 单击访客（在访客页面中）以及右侧面板上的Set Campaign时，可以找到唯一的Web Personalization访客标识号。 访客ID位于高级设置部分。 访客ID也可以在URL中找到（例如VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS）。

**搜索词** — 根据潜在客户的搜索词定义区段。

* 搜索的访客 — 从下拉列表中，从访客搜索中选择要跟踪的搜索词，或添加您自己的搜索词。 （搜索词上不需要使用&#42;通配符，因为它设置为默认包含包含搜索词的短语）。

**反向链接** — 添加访客被引用的URL。

* 选择要添加的反向链接 — 从下拉列表中，选择要跟踪的反向链接网站或添加您自己的反向链接。 选中后，反向链接将显示在下面的框中。 （允许使用&#42;作为通配符）

**包含页面** — 跟踪潜在客户访问您网站的特定页面。

* URL匹配 — 添加要跟踪的特定网页的URL。 您可以通过用分号分隔多个URL来添加它们。 （允许使用&#42;作为通配符）。

**排除页面** — 排除您不希望在此区段中匹配的特定页面。 （允许使用&#42;作为通配符）。

* URL不匹配 — 添加要从跟踪中排除的特定网页的URL。 您可以通过用分号分隔多个URL来添加它们

![](assets/segment-extra.png)

### 设备/浏览器 {#device-browser}

**移动操作系统**

将移动设备操作系统拖放到区段编辑器中

![](assets/image2015-5-27-17-3a45-3a3.png)

* **访客类型**<br />
  **移动操作系统** — 从下拉框中选择列出的一个或多个移动操作系统。 选定的移动设备操作系统显示在下方。

   * 访客正在使用任何移动设备
   * 访客正在使用此特定设备/操作系统
   * 访客未使用任何移动设备

* **设备** — 从下拉列表中选择一个或多个设备(Apple、Samsung、LG、HTC、Nexus、Blackberry等……)。 选定的设备显示在下方。

**浏览器**

使用特定浏览器类型和/或版本的Target访客。

* 浏览器类型 — 从下拉框中，选择一个或多个Internet浏览器。 选定的浏览器显示如下。
* 浏览器版本 — 输入要添加到区段的浏览器版本。 您可以通过用逗号分隔多个版本来选择多个版本。 （允许使用&#42;作为通配符）。

### API {#api}

**数据事件** — 触发特定自定义数据事件的区段访客

添加要定位的事件值。 例如，来自第三方数据源。

**用户上下文API**

Web Personalization API调用[在此处阅读更多相关信息。](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/javascriptapi/web-personalization)

>[!TIP]
>
>**使用通配符 —**&#x200B;当您想要包含任何搜索词或URL且其中包含“[google.com](https://google.com)”或“搜索词产品”时，我们将其称为通配符，并且应在每端输入一个星号 — 此小家伙&#42;。 因此，来自[google.com](https://google.com)的任何内容都应作为&#42; [google.com](https://google.com)&#42;输入

## 编辑区段 {#edit-segments}

您可以编辑已创建的区段。

1. 要编辑区段，请转到&#x200B;**区段**。

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. 在&#x200B;**区段**&#x200B;表中，单击要编辑的区段的编辑图标(![](assets/segment-edit.png))。 将打开&#x200B;**设置区段**&#x200B;页面，其中包含选定的区段。
1. 应用您想要对区段所做的任何编辑或更改。
1. 单击&#x200B;**保存**。

## 删除区段 {#delete-segments}

您可以删除已创建的区段。

1. 从上面的&#x200B;**区段**&#x200B;页面中，选择一个区段。
1. 单击要删除的区段的删除图标( ![](assets/segment-delete.png))。
1. 出现确认消息，确认您即将删除&#x200B;**区段**。

>[!NOTE]
>
>您无法删除与营销活动关联的区段。 首先，您需要删除营销活动，然后删除区段。

太棒了！ 现在，您已了解区段部分，接下来让我们了解促销活动。

>[!MORELIKETHIS]
>
>* [创建基本Web区段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
>* [新建Dialog Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [在区域中创建新的Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [创建新的构件Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
