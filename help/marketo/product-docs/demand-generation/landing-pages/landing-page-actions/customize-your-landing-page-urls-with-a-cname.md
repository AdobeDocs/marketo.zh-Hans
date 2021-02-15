---
unique-page-id: 2359746
description: 使用CNAME - Marketo Docs — 产品文档自定义您的登陆页URL
title: 使用CNAME自定义登陆页URL
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# 使用CNAME {#customize-your-landing-page-urls-with-a-cname}自定义登陆页URL

即使Marketo托管您的登陆页,URL也可以完全自定义。 没有CNAME时的外观：

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

它应该看起来：

`https://go.YourCompany.com/UnsubscribePage.html`

## 选择CNAME {#choose-a-cname}

为您的登陆页选择URL开头的词。 只是一个词，应该相对短。 示例：

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

一个词（加上YourCompany.com）称为CNAME。 你以后需要这个，记下来。

## 查找帐户字符串{#find-your-account-string}

1. 转至&#x200B;**Admin**&#x200B;区域，然后单击&#x200B;**登陆页**。

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**需要管理权限**

1. 在&#x200B;**登录** **页面**&#x200B;选项卡下，从&#x200B;**设置**&#x200B;部分复制&#x200B;**帐户** **字符串**。

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. 您以后还需要，请记下来。

## 向IT {#send-request-to-it}发送请求

要求您的IT员工设置以下CNAME:（将单词[CNAME]和[ACCOUNT STRING]替换为上一步中的文本。）

[CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## 完成CNAME设置{#complete-cname-setup}

1. IT部门创建CNAME后，请转至&#x200B;**Admin**&#x200B;并单击&#x200B;**登陆页**。

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. 在&#x200B;**设置**&#x200B;部分下，单击&#x200B;**编辑**。

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. 在&#x200B;**登陆页**&#x200B;的域名中输入您的CNAME，输入&#x200B;**回退页**，输入您的&#x200B;**主页**&#x200B;并单击&#x200B;**保存**。

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>您的回退页面将是页面潜在客户在您的Marketo登陆页不可用时将被重定向到的页面。

干得好！ 您的登陆页现在使用您的公司域进行品牌化。
