---
unique-page-id: 2360189
description: 使用CNAME（管理）自定义登陆页面URL - Marketo文档 — 产品文档
title: 使用CNAME（管理）自定义登陆页面URL
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 使用CNAME自定义登陆页面URL  {#customize-your-landing-page-urls-with-a-cname}

即使Marketo托管您的登陆页面，也应该为您的公司自定义URL。

>[!NOTE]
>
>无CNAME：
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>品牌CNAME：
>
>https://go.**您的公司**.com/UnsuscribePage.html

>[!NOTE]
>
>**需要管理员权限**

让我们为您做好准备！

1. 选择一个CNAME。

   它是URL的前面。 示例:

   * **转到**.YourCompany.com/NameOfPage.html
   * **信息**.YourCompany.com/NameOfPage.html
   * **页面**.YourCompany.com/NameOfPage.html

   一个字(加上YourCompany.com)称为CNAME。 您稍后将需要此项，因此请记下它。

1. 查找您的帐户字符串。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 单击 **[!UICONTROL 登陆页面]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. 在 **[!UICONTROL 登陆页面]** 选项卡，从设置部分中复制帐户字符串。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. 您稍后也将需要它，因此请记下它。

1. 向IT发送请求。

1. 要求您的IT员工设置以下CNAME(将 [CNAME] 和 [帐户字符串] （其中包含上一步中的文本）：

   [CNAME].YourCompany.com > [帐户字符串].mktoweb.com

1. 完成CNAME设置。

1. 在IT部门创建CNAME后，返回至 **[!UICONTROL 管理员]** 区域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 单击 **[!UICONTROL 登陆页面]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在 **[!UICONTROL 设置]** 部分，单击 **[!UICONTROL 编辑]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在中输入您的CNAME **[!UICONTROL 登陆页面的域名]**，输入您的 **[!UICONTROL 回退页]**，输入您的 **[!UICONTROL 主页]**，然后单击 **[!UICONTROL 保存]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

如果您的Marketo登陆页面不可用，则您的回退页是将用户重定向到的页面。

做得好！ 您的登陆页面现在使用您的公司域进行标记。
