---
unique-page-id: 2359918
description: 编辑登陆页面设置 — Marketo文档 — 产品文档
title: 编辑登陆页面设置
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 编辑登陆页面设置 {#edit-landing-page-settings}

您可以编辑域名和备用页面、启用或禁用表单预填充、防止滥用登陆页面等。 下面是具体操作方法。

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/edit-landing-page-settings-1.png)

1. 单击 **[!UICONTROL 登陆页面]**.

   ![](assets/edit-landing-page-settings-2.png)

1. 在 **[!UICONTROL 登陆页面]** 部分，单击 **[!UICONTROL 编辑]**.

   ![](assets/edit-landing-page-settings-3.png)

1. 输入域和页面信息。

   ![](assets/edit-landing-page-settings-4.png)

   | 搜索词 | 条件 |
   |---|---|
   | [!UICONTROL 登陆页面的域名] | 这是您的CNAME。 CNAME是您为登陆页面授予用户的URL的第一部分。 例如，在 `https://go.yourCompany.com`，单词“go”就是CNAME。 您可以有多个，但大多数人只使用一个。 |
   | [!UICONTROL 回退页] | 如果登陆页面不存在或关闭，则前往此位置。 详细了解 [回退页](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL 主页] | 输入您的公司网站URL。 |

1. 查看 **[!UICONTROL 表单预填]** 用于允许表单预填充已知（已编码）人员信息的复选框。 取消选中以阻止。

   ![](assets/edit-landing-page-settings-5.png)

1. 如果要防止恶意网站似乎托管您的内容，请检查 **[!UICONTROL 不允许在外部网页中嵌入Marketo页面]** 复选框。

   ![](assets/edit-landing-page-settings-6.png)

   >[!NOTE]
   >
   >如果您希望预填充 `<script>` 标签末尾的 `<head>` 标记时，请检查 **[!UICONTROL 在头末尾插入预填充脚本]** 盒子。 如果您希望它显示在开头，请将其保留为取消选中状态。
   >
   >Check **[!UICONTROL 删除默认Favicon链接]** 以防止Marketo在代码中插入任何favicon链接。

1. 进行选择后，单击 **[!UICONTROL 保存]**.

   ![](assets/edit-landing-page-settings-7.png)

   做得好！ 您的登陆页面现在包含正确的信息，应该立即开始工作。
