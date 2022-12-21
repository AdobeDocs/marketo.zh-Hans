---
unique-page-id: 2359746
description: 使用CNAME自定义登陆页面URL - Marketo文档 — 产品文档
title: 使用CNAME自定义登陆页面URL
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# 使用CNAME自定义登陆页面URL {#customize-your-landing-page-urls-with-a-cname}

即使Marketo托管您的登陆页面，也可以完全自定义URL。 没有CNAME时的样子：

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

它的外观：

`https://go.YourCompany.com/UnsubscribePage.html`

## 选择CNAME {#choose-a-cname}

选择要在登陆页面URL开头显示的词语。 只是一个词，应该相对较短。 示例:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

一个词（加上YourCompany.com）叫做CNAME。 你以后需要这个，记一下。

## 查找帐户字符串 {#find-your-account-string}

1. 转到 **管理员** 单击 **登陆页面**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**需要管理员权限**

1. 在 **登陆** **页面** 选项卡，复制 **帐户** **字符串** 从 **设置** 中。

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. 您以后还需要，请记下来。

## 向IT发送请求 {#send-request-to-it}

请您的IT员工设置以下CNAME:(替换 [CNAME] 和 [帐户字符串] （使用上一步中的文本）

[CNAME].YourCompany.com > [帐户字符串].mktoweb.com

## 完成CNAME设置 {#complete-cname-setup}

1. IT部门创建CNAME后，转到 **管理员** 单击 **登陆页面**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. 在 **设置** ，单击 **编辑**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. 在 **登陆页面的域名**，输入 **回退页面**，输入 **主页** 单击 **保存**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>如果您的Marketo登陆页面不可用，您的后备页面将是页面潜在客户，他们将被重定向到。

干得好！ 登陆页面现在使用您的公司域进行标记。
