---
unique-page-id: 2359918
description: 编辑登陆页设置- Marketo Docs —— 产品文档
title: 编辑登陆页设置
translation-type: tm+mt
source-git-commit: 95ca406109e04f56c9846f83cb2c4202bf606518
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# 编辑登陆页设置 {#edit-landing-page-settings}

您可以编辑您的域名和备用页面、启用或禁用表单预填、防止滥用登陆页等。 这是方法。

>[!NOTE]
>
>**需要管理员权限**

1. 在“管 **理员**”下，单击 **登陆页**。

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. 在登陆页 **部分** ，单击编 **辑**。

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. 输入您的域和页面信息。

   | 期限 | 定义 |
   |---|---|
   | 登陆页的域名 | 这是您的CNAME。 CNAME是您为登陆页提供的URL的第一部分。 例如，在 `http://go.yourCompany.com`中，单词“go”是CNAME。 你可以有多个，但大多数人只是用这个。 |
   | 回退页 | 如果登陆页不存在或关闭，则此处为该位置。 了解有关备用页 [面的更多信息](set-a-fallback-page.md)。 |
   | 主页 | 输入您的公司网站URL。 |

   ![](assets/three.png)

1. 选中“表 **单预填** ”复选框，允许表单预填已知(Cookied)人员的信息。 取消选中以阻止。

   ![](assets/four.png)

1. 如果要防止恶意站点看似托管您的内容，请选中“ **不允许将Marketo页面嵌入到外部网页中** ”复选框。

   ![](assets/five.png)

   >[!NOTE]
   >
   >如果希望预填充标 `<script>` 签显示在代码中标 `<head>` 签的末尾，请选中“在头 **部结尾插入预填充脚本** ”框。 如果希望它显示在开头，请不选中。
   >
   >选中 **删除默认的收藏夹链接** ，以阻止Marketo将任何收藏夹链接插入到代码中。

1. 进行选择后，单击“保 **存”。**

   ![](assets/six.png)

   干得好！ 您的登陆页现在拥有正确的信息，应立即开始开始工作。

