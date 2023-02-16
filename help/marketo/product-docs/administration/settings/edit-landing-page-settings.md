---
unique-page-id: 2359918
description: 编辑登陆页面设置 — Marketo文档 — 产品文档
title: 编辑登陆页面设置
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 编辑登陆页面设置 {#edit-landing-page-settings}

您可以编辑域名和后备页面、启用或禁用表单预填充、防止误用登陆页面等。 这是方法。

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **管理员** 的上界。

   ![](assets/edit-landing-page-settings-1.png)

1. 单击 **登陆页面**.

   ![](assets/edit-landing-page-settings-2.png)

1. 在 **登陆页面** ，单击 **编辑**.

   ![](assets/edit-landing-page-settings-3.png)

1. 输入域和页面信息。

   ![](assets/edit-landing-page-settings-4.png)

   | 术语 | 条件 |
   |---|---|
   | 登陆页面的域名 | 这是您的CNAME。 CNAME是您为登陆页面的人员提供的URL的第一部分。 例如， `https://go.yourCompany.com`，则词“go”表示CNAME。 你可以有多个，但大多数人只使用一个。 |
   | 回退页面 | 如果登陆页面不存在或已关闭，则可前往此处。 详细了解 [回退页面](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | 主页 | 输入公司网站URL。 |

1. 检查 **表单预填充** 复选框，允许表单预填已知(cookie)人员的信息。 取消选中以阻止。

   ![](assets/edit-landing-page-settings-5.png)

1. 如果要阻止恶意网站似乎托管您的内容，请检查 **不允许将Marketo页面嵌入到外部网页中** 复选框。

   ![](assets/edit-landing-page-settings-6.png)

   >[!NOTE]
   >
   >如果您想要预填充 `<script>` 标记显示在 `<head>` 标记，请检查 **在头端插入预填充脚本** 框中。 如果希望在开头显示，请保持未选中状态。
   >
   >检查 **删除默认收藏夹链接** 来阻止Marketo将任何favicon链接插入代码。

1. 进行选择后，单击 **保存。**

   ![](assets/edit-landing-page-settings-7.png)

   干得好！ 您的登陆页面现在具有正确的信息，应该立即开始工作。
