---
unique-page-id: 2359746
description: 使用CNAME自定义登陆页面URL - Marketo文档 — 产品文档
title: 使用CNAME自定义登陆页面URL
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 使用CNAME自定义登陆页面URL {#customize-your-landing-page-urls-with-a-cname}

即使Marketo托管您的登陆页面，也可以完全自定义URL。 没有CNAME时的外观：

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

它应呈现的外观：

`https://go.YourCompany.com/UnsubscribePage.html`

## 选择一个CNAME {#choose-a-cname}

为您的登陆页面选择位于URL开头的单词。 它只是一个词，应该相对较短。 示例:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

一个单词(加上YourCompany.com)称为CNAME。 稍后您需要此项，请记下它。

## 查找您的Munchkin ID {#find-your-munchkin-id}

1. 转到 **管理员** 区域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 单击 **我的帐户**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**需要管理员权限**

1. 向下滚动至“支持信息”并复制您的Munchkin ID。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## 向IT部门发送请求 {#send-request-to-it}

要求您的IT员工设置以下CNAME： (将 [CNAME] 和 [Munchkin ID] 使用上一步中的文本。)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## 完成CNAME设置 {#complete-cname-setup}

1. IT部门创建CNAME后，转到 **管理员** 区域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 单击 **登陆页面**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在 **设置** 部分，单击 **编辑**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在中输入您的CNAME **登陆页面的域名**，输入您的 **回退页**，输入您的 **主页** 并单击 **保存**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>如果您的Marketo登录页面不可用，您的后备页面将成为潜在客户将重定向到的页面。

做得好！ 您的登陆页面现在使用您的公司域进行标记。
