---
unique-page-id: 11385579
description: 创建内容模式 — Marketo文档 — 产品文档
title: 创建内容模式
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 创建内容模式 {#create-content-patterns}

在设置内容模式时，当Web访客单击与内容模式相关的HTML网页时，会自动发现内容。 它用于将HTML页面（博客帖子、新闻稿、新闻文章）作为内容片段添加到所有内容页面。 当自动发现基于内容模式时，它会在Web访客查看或单击指向该页面的链接时，发现和跟踪与定义的URL模式相关的HTML页面。 此内容片段(URL、页面名称和元数据（包括图像URL和描述）将添加到“所有内容”页面，以准备预测内容。 要自动发现其他内容(如PDF和嵌入式视频)，您需要 [启用内容发现](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. 转到 **内容设置**.

   ![](assets/settings-dropdown-hand-2.png)

1. 单击 **URL模式**.

   ![](assets/click-url-patterns-hand.png)

1. 单击 **+** 打开一行，您可以在其中输入信息。

   ![](assets/content-settings-create-patterns-hand.png)

1. 添加存在网页的域的URL扩展名。 选择类别（例如，“博客”、“文章”、“数据表”、“新闻发布”）。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右侧下拉列表中的项目反映了您在 [创建类别](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. 单击 **+** 添加其他路径。

   ![](assets/url-patterns-add2.png)

1. 添加其他路径的扩展和目录，然后单击 **保存**.

   ![](assets/url-patterns-save.png)

## 内容模式规则 {#content-pattern-rules}

* 您可以在表达式中的任意位置使用通配符(示例： _domain.com/&#42;_, _domain.com/&#42;博客&#42;_)

* 我们建议使用/&#42; 在表达式的末尾继续模式发现(示例： _domain.com/blog/&#42;_ 发现Blog文件夹中的所有帖子)
* 内容模式不区分大小写(示例： _domain.com/Blog/&#42;_ 在 _domain.com/Blog_ 和 _domain.com/blog_)

* 未发现URL参数（这样可避免发现具有相同内容URL但参数不同的多个项目）

## 示例 {#examples}

对于 _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>URL模式</th> 
   <th>结果</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>发现所有与模式匹配的内容domain.com/blog/ :</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>2017年/*</td> 
   <td><p>发现所有与模式匹配的内容domain.com/article/2017/ :</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>发现包含“数据表：”字样的任何URL</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>新闻稿</td> 
   <td><p>只发现一个完全匹配的HTML页面：</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>如果URL表达式为空，则URL模式仅会发现主页：</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
