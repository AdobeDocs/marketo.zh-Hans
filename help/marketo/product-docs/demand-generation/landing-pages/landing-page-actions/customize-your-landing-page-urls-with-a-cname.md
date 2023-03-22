---
unique-page-id: 2359746
description: 使用CNAME自定义登陆页面URL - Marketo文档 — 产品文档
title: 使用CNAME自定义登陆页面URL
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '237'
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

## 查找您的Munchkin ID {#find-your-munchkin-id}

1. 转到 **管理员** 的上界。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 单击 **我的帐户**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**需要管理员权限**

1. 向下滚动到“支持信息”，并复制您的Munchkin ID。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## 向IT发送请求 {#send-request-to-it}

请您的IT员工设置以下CNAME:(替换 [CNAME] 和 [蒙奇金ID] （使用上一步中的文本）

[CNAME].YourCompany.com > [蒙奇金ID].mktoweb.com

## 完成CNAME设置 {#complete-cname-setup}

1. IT部门创建CNAME后，转到 **管理员** 的上界。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 单击 **登陆页面**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在 **设置** ，单击 **编辑**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在 **登陆页面的域名**，输入 **回退页面**，输入 **主页** 单击 **保存**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>如果您的Marketo登陆页面不可用，您的后备页面将是页面潜在客户，他们将被重定向到。

干得好！ 登陆页面现在使用您的公司域进行标记。
