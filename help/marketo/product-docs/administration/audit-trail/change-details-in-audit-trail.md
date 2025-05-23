---
unique-page-id: 11379928
description: 有关更改详细信息，请参阅审核记录 — Marketo文档 — 产品文档
title: 审核记录中的更改详细信息
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
feature: Audit Trail
source-git-commit: 1477b889f74597396b3467371229a511e4390f91
workflow-type: tm+mt
source-wordcount: '1902'
ht-degree: 10%

---

# 审核记录中的更改详细信息 {#change-details-in-audit-trail}

审核记录提供了有关谁在您的Marketo订阅中执行操作的丰富洞察信息。 详情如下。

## 资产审核记录 {#asset-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">资产/类型</th> 
   <th colspan="1">操作</th> 
   <th colspan="1">更改详细信息</th> 
  </tr> 
  <tr> 
   <td rowspan="15"><strong>默认项目群</strong><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>创建</td> 
   <td>渠道类型“渠道类型”<br>或<br>克隆自“项目名称”</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到工作区“工作区名称”<br>位置“Campaign文件夹”或“参与计划”<br>已克隆的计划名称“新名称”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>编辑渠道</td> 
   <td>新频道“新频道名称”旧频道“旧频道名称” </td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>添加令牌“令牌名称”值“令牌值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>编辑令牌“令牌名称”新值“新值”旧值“旧值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>删除令牌“令牌名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>添加分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td><p>编辑分析行为“行为名称”</p><p>旧行为“行为名称”</p></td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>删除分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">添加期间成本值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">编辑期间成本新成本值“#”、新计划月份“yyyy-mm”、旧成本值“#”、旧计划月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">删除期间成本。 值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td>导出</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td rowspan="19"><strong>电子邮件</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>创建</td> 
   <td>使用模板“模板名称”<br>或从“资产名称”克隆的<br>创建</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已将“From Name”更新为“new from name”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已将“From Email”更新为“newemail@name.com”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已将“回复”更新为“newreplytoemail@name.com”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已将“主题”更新为“新主题行”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>添加了分段“segmentation_name”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>删除的分段</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>添加了代码片段“snippet_name”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已删除的代码片段</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>编辑操作中断了来自模板“template_name”的电子邮件（注意：如果您直接编辑代码，将会立即发生这种情况）</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”旧描述“旧描述”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>将模块<code>"&lt;module name&gt;" &lt;attribute&gt;</code>编辑为“value”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>克隆到“Design Studio”到文件夹“foldername”<br>克隆的资产名称“name”<br>或<br>克隆到“营销活动”到程序“程序名称”<br>克隆的资产名称“name”</td> 
  </tr> 
  <tr> 
   <td>移动</td> 
   <td>已移至“Design Studio”文件夹“文件夹名称”<br>或<br>已移至“营销活动”项目“项目名称”</td> 
  </tr> 
  <tr> 
   <td>批准</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>取消批准</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td>起草电子邮件是因为批准了代码片段“代码片段名称”<br>或者<br>起草电子邮件是因为批准了模板“模板名称”</td> 
  </tr> 
   <td rowspan="17">电子邮件程序</td> 
   <td>创建</td> 
   <td>渠道类型“渠道类型”<br>或<br>克隆自“项目名称”</td> 
  </tr> 
  <tr> 
   <td colspan="1">重命名</td> 
   <td colspan="1">新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到工作区“工作区名称”<br>位置“Campaign文件夹或参与计划”<br>已克隆的计划名称“新名称”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>中止</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>编辑渠道</td> 
   <td>新频道“新频道”旧频道“旧频道”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>添加令牌“令牌名称”值“令牌值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>编辑令牌“令牌名称”新值“新值”旧值“旧值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>删除令牌“令牌名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目计划</td> 
   <td>将计划设置为从“开始日期、开始时间”开始，到“结束日期、结束时间”结束</td> 
  </tr> 
  <tr> 
   <td>修改项目计划</td> 
   <td>已将计划更改为“新日期、新时间”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>添加分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>编辑分析行为“行为名称”<br>旧行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>删除分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">添加期间成本值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">编辑期间成本新成本值“#”、新计划月份“yyyy-mm”、旧成本值“#”、旧计划月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">删除期间成本。 值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td rowspan="8">电子邮件模板</td> 
   <td>创建</td> 
   <td>空白或从“模板名称”克隆</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”，上一描述“上一描述”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已编辑HTML</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到“文件夹名称”<br>已克隆资产名称“名称”</td> 
  </tr> 
  <tr> 
   <td>批准</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>取消批准</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td rowspan="23">参与计划</td> 
   <td>创建</td> 
   <td>渠道类型“渠道类型”<br>或<br>从“项目名称”克隆</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到工作区“工作区名称”<br>位置“Campaign文件夹或参与计划”<br>已克隆的计划名称“新名称”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>编辑渠道</td> 
   <td>新频道“新频道”旧频道“旧频道”</td> 
  </tr> 
  <tr> 
   <td>修改程序流</td> 
   <td><p>添加流</p><p>名称“name”投放位置“#”</p></td> 
  </tr> 
  <tr> 
   <td>修改程序流</td> 
   <td><p>编辑流</p><p>新流名称：“新名称”旧流名称：“旧名称”</p><p>新投放位置：“new #”旧投放位置：“old #”</p></td> 
  </tr> 
  <tr> 
   <td>修改程序流</td> 
   <td>删除流名称“name”</td> 
  </tr> 
  <tr> 
   <td>修改程序流</td> 
   <td>添加内容<br>流名称“流名称”<br>键入“电子邮件”或“项目”<br>名称“电子邮件名称”或“项目名称”<br>智能促销活动“智能促销活动名称”</td> 
  </tr> 
  <tr> 
   <td>修改程序流</td> 
   <td>激活内容<br>流名称“流名称”<br>内容名称“电子邮件名称”或“项目名称”</td> 
  </tr> 
  <tr> 
   <td>修改程序流</td> 
   <td>停用内容<br>流名称“流名称”<br>内容名称“电子邮件名称”或“程序名称”</td> 
  </tr> 
  <tr> 
   <td>修改程序流</td> 
   <td>删除内容<br>流名称“流名称”<br>内容名称“电子邮件名称”或“程序名称”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>添加令牌“令牌名称”值“令牌值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>编辑令牌“令牌名称”新值“新值”旧值“旧值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>删除令牌“令牌名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>添加分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>编辑分析行为“行为名称”<br>旧行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>删除分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>更改项目状态。 新值“on/off”旧值“off/on”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">添加期间成本值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">编辑期间成本新成本值“#”、新计划月份“yyyy-mm”、旧成本值“#”、旧计划月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">删除期间成本。 值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td>导出</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td rowspan="18">活动计划</td> 
   <td>创建</td> 
   <td>渠道类型“渠道类型”<br>或<br>克隆自“项目名称”</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到工作区“工作区名称”<br>位置“campaign文件夹”或“参与计划”<br>已克隆计划名称“新名称”</td> 
  </tr> 
  <tr> 
   <td>编辑渠道</td> 
   <td>新频道“新频道”旧频道“旧频道” </td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>添加令牌“令牌名称”值“令牌值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>编辑令牌“令牌名称”新值“新值”旧值“旧值”</td> 
  </tr> 
  <tr> 
   <td>修改程序令牌</td> 
   <td>删除令牌“令牌名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目计划</td> 
   <td>将计划设置为从“开始日期、开始时间”开始，到“结束日期、结束时间”结束</td> 
  </tr> 
  <tr> 
   <td>修改项目计划</td> 
   <td>已将计划更改为“新日期、新时间”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>添加分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>编辑分析行为“行为名称”<br>旧行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td>修改项目设置</td> 
   <td>删除分析行为“行为名称”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">添加期间成本值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">编辑期间成本新成本值“#”、新计划月份“yyyy-mm”、旧成本值“#”、旧计划月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">删除期间成本。 值“#”程序月份“yyyy-mm”</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改项目设置</td> 
   <td colspan="1">已添加活动合作伙伴“partner_name”</td> 
  </tr> 
  <tr> 
   <td>导出</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td rowspan="5">文件夹</td> 
   <td>创建</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>添加了令牌“token_name”、值“value”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>编辑了令牌“token_name”新值“token_value”旧值“old_token_value”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已删除令牌“token_name”</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Forms</td> 
   <td>创建</td> 
   <td>即将推出。 了解更多信息或从“表单名称”克隆</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”旧描述“旧描述”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已编辑表单设置 </td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已编辑字段详细信息</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>克隆到“Design Studio”到文件夹“foldername”<br>克隆的资产名称“name”<br>或<br>克隆到“营销活动”到程序“程序名称”<br>克隆的资产名称“name”</td> 
  </tr> 
  <tr> 
   <td>移动</td> 
   <td>已移至“Design Studio”文件夹“文件夹名称”<br>或<br>已移至“营销活动”项目“项目名称”</td> 
  </tr> 
  <tr> 
   <td>Forms</td> 
   <td>批准</td> 
   <td>由#个资源使用 </td> 
  </tr> 
  <tr> 
   <td rowspan="9">登陆页面</td> 
   <td>创建</td> 
   <td>使用模板“模板名称”<br>或从“资产名称”克隆的<br>创建</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”上一个“描述”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>添加了“图像”，删除了“图像”，编辑了图像组件</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>添加了“富文本”、删除了“富文本”、编辑了富文本组件</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>克隆到“Design Studio”到文件夹“foldername”<br>克隆的资产名称“name”<br>克隆的资产URL“www.url.com”<br>或<br>克隆到“营销活动”到程序“程序名称”<br>克隆的资产名称“name”<br>克隆的资产URL“www.url.com”</td> 
  </tr> 
  <tr> 
   <td>移动</td> 
   <td>已移至“Design Studio”文件夹“文件夹名称”<br>或<br>已移至“营销活动”项目“项目名称”</td> 
  </tr> 
  <tr> 
   <td>批准</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td>由于模板“模板名称”获得批准，已起草登陆页面</td> 
  </tr> 
  <tr> 
   <td>取消批准</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td rowspan="8">登陆页面模板</td> 
   <td>创建</td> 
   <td><p>空白<br>或<br>克隆自“资产名称”</p></td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”前描述“前描述”</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到“文件夹名称”<br>已克隆资产名称“名称”</td> 
  </tr> 
  <tr> 
   <td>导出</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>批准</td> 
   <td>由#个资源使用 </td> 
  </tr> 
  <tr> 
   <td>取消批准</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td rowspan="5">列表（静态）</td> 
   <td>创建</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>导出</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到“人员数据库”并放入文件夹“foldername”<br>已克隆资产名称“name”<br>或<br>已克隆到“营销活动”并放入程序“程序名称”<br>已克隆资产名称“name”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td rowspan="12">Smart Campaign</td> 
   <td>创建</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>激活</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>停用</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>中止</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>移动</td> 
   <td>已移至“程序”到程序“程序名称”<br>或<br>已移至“文件夹”到文件夹“文件夹名称”</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”上一个“描述”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>克隆到“程序”到程序“程序名称”<br>克隆的资产名称“名称”<br>或<br>克隆到“文件夹”到文件夹“文件夹名称”<br>克隆的资产名称“名称”</td> 
  </tr> 
  <tr> 
   <td>修改smartlist设置</td> 
   <td>显示当前状态的快照，包括筛选器和触发器的名称和值</td> 
  </tr> 
  <tr> 
   <td>修改营销活动计划</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>修改流步骤操作</td> 
   <td>显示当前状态的快照，包括每个流程步骤的名称和值</td> 
  </tr> 
  <tr> 
   <td rowspan="7">智能列表</td> 
   <td>创建</td> 
   <td>从“智能列表名称”克隆</td> 
  </tr> 
  <tr> 
   <td>导出</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”上一个“描述”</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到“人员数据库”并放入文件夹“foldername”<br>已克隆资产名称“name”<br>或<br>已克隆到“营销活动”并放入程序“程序名称”<br>已克隆资产名称“name”</td> 
  </tr> 
  <tr> 
   <td>修改smartlist设置</td> 
   <td>显示当前状态的快照，包括筛选器和触发器的名称和值 </td> 
  </tr> 
  <tr> 
   <td rowspan="11">代码片段</td> 
   <td>创建</td> 
   <td><p>从“代码片段名称”克隆的Blank<br>或<br></p></td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>添加了分段“segmentation_name”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>删除的分段</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已编辑</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>重命名</td> 
   <td>新名称“新名称”，以前名称“以前名称”</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>新描述“新描述”上一个“描述”</td> 
  </tr> 
  <tr> 
   <td>克隆</td> 
   <td>已克隆到“文件夹名称”<br>已克隆的代码片段名称“名称”</td> 
  </tr> 
  <tr> 
   <td>批准</td> 
   <td>由#个资源使用</td> 
  </tr> 
  <tr> 
   <td>审批，无草稿</td> 
   <td>不适用</td> 
  </tr> 
  <tr> 
   <td>取消批准</td> 
   <td><p>不适用</p></td> 
  </tr> 
 </tbody> 
</table>

## 管理员审核记录 {#admin-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>管理区域</th> 
   <th>操作</th> 
   <th>更改详细信息</th> 
  </tr> 
  <tr> 
   <td>IP限制</td> 
   <td>Edit</td> 
   <td>编辑了以下内容的IP限制：允许/阻止的“阻止”、IP地址“#”、禁用的IP限制“”</td> 
  </tr> 
  <tr> 
   <td rowspan="2">分区</td> 
   <td>创建</td> 
   <td>已创建名为“分区名称”的分区</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>已删除“分区名称”分区</td> 
  </tr> 
  <tr> 
   <td>密码强度</td> 
   <td>Edit</td> 
   <td>密码安全性已更改为模板：标准安全性，最小长度： #，上小写： #，数字： #，大小写混合： #，到期： #，会话超时： #</td> 
  </tr> 
  <tr> 
   <td rowspan="3">角色<br><br></td> 
   <td>创建</td> 
   <td>使用“角色名称”创建的角色（注意：如果您需要有关所添加权限的详细信息，请联系支持人员） — <br>显示分配给角色的权限快照</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>已删除“角色名称”角色</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>角色已从“先前名称”编辑为“新名称”（注意：如果您需要有关已编辑权限的详细信息，请联系支持人员） — <br>显示分配给角色的权限快照<br></td> 
  </tr> 
  <tr> 
   <td>智能列表报告</td> 
   <td>Edit</td> 
   <td>编辑登录以下载的SmarList：“true或false”</td> 
  </tr> 
  <tr> 
   <td rowspan="7">用户<br><br><br><br></td> 
   <td>创建（邀请）</td> 
   <td>邀请的用户：电子邮件“电子邮件地址”，姓名“名字和姓氏”，访问过期时间“空白或带日期”，API用户“true或false” — <br>显示分配给用户的角色和工作区的快照</td> 
  </tr> 
  <tr> 
   <td colspan="1">Delete</td> 
   <td colspan="1">已删除“用户名”用户</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>用户已使用“email”（电子邮件）从“old name”（旧名称）重命名为“new name”（新名称），apiUser：“true or false”（真或假）访问过期：“blank”或“with a date”（带日期）</td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>已编辑用户的电子邮件：“电子邮件”，apiUser：“true或false”，访问过期：“空白或使用日期”</td> 
  </tr> 
  <tr> 
   <td colspan="1">Edit</td> 
   <td colspan="1">显示当前状态的快照，包括分配给用户的角色和工作区</td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>颁发给电子邮件的日历许可证：“用户的电子邮件”名称：“用户名”</td> 
  </tr> 
  <tr> 
   <td>重置</td> 
   <td>名称“name”和电子邮件“email”的密码重置</td> 
  </tr> 
  <tr> 
   <td rowspan="2">工作区</td> 
   <td>创建</td> 
   <td>已使用名称“工作区名称”创建Workspace</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>已删除“工作区名称”工作区</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[在审核记录中筛选](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
