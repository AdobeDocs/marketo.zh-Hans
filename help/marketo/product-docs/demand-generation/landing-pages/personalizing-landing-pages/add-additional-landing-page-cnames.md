---
unique-page-id: 2359798
description: 添加其他登陆页CNAME - Marketo Docs —— 产品文档
title: 添加其他登陆页CNAME
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# 添加其他登陆页CNAME {#add-additional-landing-page-cnames}

您可能希望添加登陆页CNAME以允许不同的URL指向您的营销人员登陆页。 按照以下步骤操作将帮助您管理多个域。

>[!CAUTION]
>
>Cookie不能跨域共享。

>[!TIP]
>
>**相同的顶级域——好！Cookies为shared.go**.mycompany.com > **info**.mycompany.com **不同的顶级域——错误！ Cookie未共享。**
>走。**mycompany**.com >转到。**mynewcompany**.com

>[!NOTE]
>
>**需要管理员权限**

## 查找帐户字符串{#find-your-account-string}

1. 转到&#x200B;**Admin**&#x200B;区域并单击&#x200B;**登陆页**。

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. 从&#x200B;**设置**&#x200B;部分复制&#x200B;**帐户字符串**。

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. 记下来的步骤。

## 向IT {#send-request-to-it}发送请求

1. 请让您的IT部门设置以下CNAME:（将单词[CNAME]替换为您选择的CNAME，将[ACCOUNT STRING]替换为上一步中的文本）。

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## 添加新CNAME {#add-a-new-cname}

1. IT部门创建CNAME后，请转至&#x200B;**Admin**，然后单击&#x200B;**登陆页**。

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. 单击&#x200B;**新建**，然后选择&#x200B;**新建域别名**。

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. 输入&#x200B;**域别名。** 如 **果访客** 未放入URL，则显示默认页面。输入在这种情况下他们应该去的地方。

   >[!NOTE]
   >
   >对于默认页面，您可以选择登陆页或外部URL，如您的公共网站。

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. 输入&#x200B;**默认页面**&#x200B;并单击&#x200B;**创建**。

   ![](assets/image2014-9-16-15-3a20-3a43.png)

不错！ 现在，如果您想添加CNAME，您知道该怎么办。
