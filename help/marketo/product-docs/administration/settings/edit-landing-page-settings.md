---
unique-page-id: 2359918
description: 编辑登陆页设置 — Marketo Docs — 产品文档
title: 编辑登陆页设置
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# 编辑登陆页设置{#edit-landing-page-settings}

您可以编辑您的域名和回退页面、启用或禁用表单预填、防止滥用您的登陆页等。 下面介绍如何操作。

>[!NOTE]
>
>**需要管理权限**

1. 在&#x200B;**Admin**&#x200B;下，单击&#x200B;**登陆页**。

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. 在&#x200B;**登陆页**&#x200B;部分，单击&#x200B;**编辑**。

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. 输入您的域和页面信息。

   | 期限 | 定义 |
   |---|---|
   | 登陆页的域名 | 这是您的CNAME。 CNAME是您为登陆页人提供的URL的第一部分。 例如，在`https://go.yourCompany.com`中，单词“go”是CNAME。 你可以有多个，但大多数人只是使用它。 |
   | 回退页 | 如果登陆页不存在或关闭，则此位置即可到达。 了解有关[回退页面](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md)的更多信息。 |
   | 主页 | 输入您的公司网站URL。 |

   ![](assets/three.png)

1. 选中&#x200B;**表单预填**&#x200B;复选框，允许表单预填已知(cookie)人员的信息。 取消选中以阻止。

   ![](assets/four.png)

1. 如果要阻止恶意站点似乎托管您的内容，请选中&#x200B;**不允许将Marketo页面嵌入外部网页**&#x200B;复选框。

   ![](assets/five.png)

   >[!NOTE]
   >
   >如果希望预填充`<script>`标记显示在代码中`<head>`标记的末尾，请选中&#x200B;**在头末插入预填充脚本**&#x200B;框。 如果希望它显示在开头，请保持未选中状态。
   >
   >选中&#x200B;**删除默认的favicon链接**&#x200B;可阻止Marketo将任何favicon链接插入代码。

1. 进行选择后，单击&#x200B;**保存。**

   ![](assets/six.png)

   干得好！ 您的登陆页现在拥有正确的信息，应立即开始工作。
