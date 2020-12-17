---
unique-page-id: 2360189
description: 使用CNAME（管理）- Marketo Docs —— 产品文档自定义登陆页URL
title: 使用CNAME自定义登陆页URL（管理）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# 使用CNAME（管理）{#customize-your-landing-page-urls-with-a-cname-administration}自定义登陆页URL

即使Marketo托管您的登陆页，也应为您的公司自定义URL。

>[!NOTE]
>
>无CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>品牌名称：
>
>https://go。**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**需要管理员权限**

让我们帮你设置！

1. 选择CNAME。

   它是URL的前部。 示例：

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **页面**.YourCompany.com/NameOfPage.html

   单个词（加上YourCompany.com）称为CNAME。 你以后需要这个，记下来。

1. 查找帐户字符串。

1. 转到&#x200B;**Admin**&#x200B;区域并单击&#x200B;**登陆页**。

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. 在&#x200B;**登陆页**&#x200B;选项卡下，从“设置”部分复制“帐户字符串”。

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. 稍后您还需要这个，请记下它。

1. 向IT部门发送请求。

1. 请您的IT员工设置以下CNAME（将单词[CNAME]和[ACCOUNT STRING]替换为上一步中的文本）:

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

1. 完成CNAME设置。

1. IT人员创建CNAME后，请转至&#x200B;**Admin**&#x200B;并单击&#x200B;**登陆页**。

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. 在&#x200B;**设置**&#x200B;部分下，单击&#x200B;**编辑**。

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. 在&#x200B;**登陆页的域名**&#x200B;中输入您的CNAME，输入您的&#x200B;**备用页**，输入您的&#x200B;**主页**，然后单击&#x200B;**保存**。

   ![](assets/image2014-9-16-13-3a10-3a45.png)

如果您的Marketo登陆页不可用，将在您的备用页面重定向人员。

干得好！ 您的登陆页现在与您的公司域一起添加品牌。
