---
unique-page-id: 2359798
description: 添加其他登陆页面CNAME - Marketo文档 — 产品文档
title: 添加其他登陆页面CNAME
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 添加其他登陆页面CNAME {#add-additional-landing-page-cnames}

您可能需要添加登陆页面CNAME，以允许其他URL指向您的Marketo登陆页面。 执行以下步骤将帮助您管理多个域。

>[!CAUTION]
>
>Cookie无法跨域共享。

>[!TIP]
>
>**相同顶级域 — 好！ Cookie已共享**.<br/> **转到**.mycompany.com > **信息**.mycompany.com
>
>**其他顶级域 — 错误！ Cookie是&#x200B;_非_共享**。<br/>开始。**mycompany**.com >开始。**mynewcompany**.com

>[!NOTE]
>
>**需要管理员权限**

1. 转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/add-additional-landing-page-cnames-1.png)

1. 单击&#x200B;**我的帐户**。

   ![](assets/add-additional-landing-page-cnames-2.png)

1. 向下滚动至“支持信息”并复制您的Munchkin ID。

   ![](assets/add-additional-landing-page-cnames-3.png)

## 向IT发送请求 {#send-request-to-it}

1. 要求您的IT部门设置以下CNAME： （将单词[CNAME]替换为您选择的CNAME，将[Munchkin ID]替换为您上一步中的文本）。

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## 添加新CNAME {#add-a-new-cname}

1. IT部门创建CNAME后，转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/add-additional-landing-page-cnames-4.png)

1. 单击&#x200B;**登陆页面**。

   ![](assets/add-additional-landing-page-cnames-5.png)

1. 单击&#x200B;**新建**，然后选择&#x200B;**新建域别名**。

   ![](assets/add-additional-landing-page-cnames-6.png)

1. 输入您的&#x200B;**域别名。**&#x200B;如果访客未置入URL，则显示&#x200B;**默认页面**。 输入在这种情况下，他们应该前往的位置。

   >[!NOTE]
   >
   >对于默认页面，您可以选择登陆页面或外部URL，例如您的公共网站。

   ![](assets/add-additional-landing-page-cnames-7.png)

1. 输入您的&#x200B;**默认页面**&#x200B;并单击&#x200B;**创建**。

   ![](assets/add-additional-landing-page-cnames-8.png)

太好了！ 如果您希望添加CNAME，现在知道该怎么做。
