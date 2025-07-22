---
unique-page-id: 11385579
description: 创建内容模式 — Marketo文档 — 产品文档
title: 创建内容模式
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 创建内容模式 {#create-content-patterns}

当您设置内容模式时，当Web访客单击与内容模式相关的HTML网页时，将自动发现内容。 它用于将HTML页面（博客文章、新闻稿、新闻文章）作为内容片段添加到所有内容页面。 当自动发现基于内容模式时，它会在Web访客查看或单击指向HTML页面的链接时发现并跟踪与定义的URL模式相关的Web页面。 此内容片段（URL、页面名称和元数据，包括图像URL和描述）将添加到所有内容页面中，以准备预测内容。 要自动发现其他内容（如PDF和嵌入的视频），您需要[启用内容发现](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md)。

1. 转到&#x200B;**[!UICONTROL Content Settings]**。

   ![](assets/settings-dropdown-hand-2.png)

1. 单击 **[!UICONTROL URL Patterns]**。

   ![](assets/click-url-patterns-hand.png)

1. 单击&#x200B;**+**&#x200B;可打开一个您可输入信息的行。

   ![](assets/content-settings-create-patterns-hand.png)

1. 添加网页所在域的URL扩展。 选择类别（例如，[!UICONTROL Blog]、[!UICONTROL Article]、[!UICONTROL Data Sheet]、[!UICONTROL Press Release]）。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右侧下拉列表中的项目反映您[创建类别](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md)时设置的类别。

1. 单击&#x200B;**+**&#x200B;添加其他路径。

   ![](assets/url-patterns-add2.png)

1. 为其他路径添加扩展和类别，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/url-patterns-save.png)

## 内容模式规则 {#content-pattern-rules}

* 您可以在表达式中的任意位置使用通配符（示例： _domain.com/&#42;_、_domain.com/&#42;blog&#42;_）

* 我们建议在表达式末尾使用/&#42;来继续模式发现(示例： _domain.com/blog/&#42;_&#x200B;可发现Blog文件夹中的所有帖子)
* 内容模式不区分大小写(示例： _domain.com/Blog/&#42;_&#x200B;发现&#x200B;_domain.com/Blog_&#x200B;和&#x200B;_domain.com/blog_&#x200B;上的所有html页面)

* 未发现URL参数（这可以避免使用相同的内容URL但不同的参数发现多个项目）

## 示例 {#examples}

对于&#x200B;_domain.com_：

<table> 
 <tbody> 
  <tr> 
   <th>URL模式</th> 
   <th>结果</th> 
  </tr> 
  <tr> 
   <td>博客/*</td> 
   <td><p>发现与模式domain.com/blog/匹配的所有内容：</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>article/2017/*</td> 
   <td><p>发现与模式domain.com/article/2017/匹配的所有内容：</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>发现任何包含“数据表”一词的URL：</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>新闻发布</td> 
   <td><p>仅发现一个完全匹配的HTML页面：</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>如果URL表达式为空，则URL模式仅可发现主页：</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
