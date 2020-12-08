---
unique-page-id: 11385579
description: 创建内容模式- Marketo Docs —— 产品文档
title: 创建内容模式
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---


# 创建内容模式 {#create-content-patterns}

>[!NOTE]
>
>根据购买日期，您的营销订阅可能包括Marketo Predictive Content或Content`<sup>AI</sup>`。 对于使用预测内容的用户，Marketo在2018年4月`<sup>AI</sup>` 30日之前一直支持内容分析功能。 要使这些功能在该日期之后保持不变，请联系您的营销人员客户成功经理以升级到营销人员内容`<sup>AI</sup>`。

设置内容模式时，当Web访客单击与内容模式相关的HTML网页时，内容会被自动发现。 它用于将HTML页面（博客文章、新闻稿、新闻文章）作为内容片段添加到“所有内容”页面。 当自动发现基于内容模式时，它会在Web访客视图或单击指向该页面的链接时，发现并跟踪与定义的URL模式相关的HTML页面。 此内容片段（URL、页面名称和元数据，包括图像URL和说明）将添加到“所有内容”页面以准备预测内容。 要自动发现其他内容（如PDF和嵌入式视频），您需要启 [用内容发现](enable-content-discovery.md)。

1. 转到“ **内容设置**”。

   ![](assets/settings-dropdown-hand-2.png)

1. 单击 **URL模式**。

   ![](assets/click-url-patterns-hand.png)

1. 单击**+ **以打开可在其中输入信息的行。

   ![](assets/content-settings-create-patterns-hand.png)

1. 添加网页所在的域的URL扩展名。 选择类别（例如，博客、文章、数据表、新闻稿）。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右侧下拉列表中的项目反映您在创建类别时设置 [的类别](set-up-categories.md)。

1. 单击**+ **可添加其他路径。

   ![](assets/url-patterns-add2.png)

1. 添加其他路径的扩展名和目录，然后单击“ **保存**”。

   ![](assets/url-patterns-save.png)

## 内容模式规则 {#content-pattern-rules}

* 您可以在表达式的任意位置使用通配符(示例： *domain.com/**, *domain.com/*blog**)

* 我们建议在表达式结束时使用/*继续模式发现(示例： *domain.com/blog/*发* 现Blog文件夹中的所有帖子)
* 内容模式不区分大小写(示例： *domain.com/Blog/** 在domain.com/Blog和domain.com/blog上 *发现* 所 *有html页*)

* 未发现URL参数（这可避免发现具有相同内容URL但参数不同的多个项目）

## 示例 {#examples}

对 *于domain.com*:

<table> 
 <tbody> 
  <tr> 
   <th>URL模式</th> 
   <th>结果</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>发现与模式匹配的所有内容domain.com/blog/:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>article/2017/*</td> 
   <td><p>发现与模式匹配的所有内容domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="--" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>发现包含“数据表：”字样的任何URL</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>新闻稿</td> 
   <td><p>只发现一个完全匹配的HTML页：</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>如果URL表达式为空，则URL模式只会发现主页:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>

