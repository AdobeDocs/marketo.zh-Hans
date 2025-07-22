---
unique-page-id: 2359746
description: 使用CNAME自定义登陆页面URL - Marketo文档 — 产品文档
title: 使用CNAME自定义登陆页面URL
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# 使用CNAME自定义登陆页面URL {#customize-your-landing-page-urls-with-a-cname}

即使Marketo托管您的登陆页面，也可以完全自定义URL。 在没有CNAME时的外观：

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

它应呈现的外观：

`https://go.YourCompany.com/UnsubscribePage.html`

## 选择一个CNAME {#choose-a-cname}

为您的登陆页面选择一个URL开头的单词。 只有一个词，应该相对较短。 示例：

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

一个字(加上YourCompany.com)称为CNAME。 你以后需要这个，所以记下来吧。

## 查找您的Munchkin ID {#find-your-munchkin-id}

1. 转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 单击&#x200B;**我的帐户**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**需要管理员权限**

1. 向下滚动至“支持信息”并复制您的Munchkin ID。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## 向IT发送请求 {#send-request-to-it}

请让您的IT员工设置以下CNAME： (将单词[CNAME]和[Munchkin ID]替换为上一步中的文本。)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## 完成CNAME设置 {#complete-cname-setup}

1. IT部门创建CNAME后，转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 单击&#x200B;**登陆页面**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在&#x200B;**设置**&#x200B;部分下，单击&#x200B;**编辑**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在&#x200B;**[!UICONTROL Domain name for Landing Pages]**&#x200B;中输入您的CNAME，输入您的&#x200B;**[!UICONTROL Fallback page]**，输入您的&#x200B;**[!UICONTROL Homepage]**，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>如果您的Marketo登录页面不可用，您的回退页面将成为潜在客户将被重定向到的页面。

做得好！ 您的登陆页面现在使用您的公司域进行标记。
