---
unique-page-id: 2359798
description: 添加其他登陆页面CNAME - Marketo文档 — 产品文档
title: 添加其他登陆页面CNAME
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 添加其他登陆页面CNAME {#add-additional-landing-page-cnames}

您可能想要添加登陆页面CNAME，以允许不同的URL指向您的Marketo登陆页面。 执行以下步骤将帮助您管理多个域。

>[!CAUTION]
>
>Cookie无法跨域共享。

>[!TIP]
>
>**相同的顶级域 — 好！ Cookie已共享**.<br/> **go**.mycompany.com > **信息**.mycompany.com
>
>**不同的顶级域 — 错误！ Cookie是 _not_ 共享**.<br/> 走。**mycompany**.com >转。**mynewcompany**.com

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **管理员** 的上界。

   ![](assets/add-additional-landing-page-cnames-1.png)

1. 单击 **我的帐户**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. 向下滚动到“支持信息”，并复制您的Munchkin ID。

   ![](assets/add-additional-landing-page-cnames-3.png)

## 向IT发送请求 {#send-request-to-it}

1. 请求您的IT部门设置以下CNAME:(替换 [CNAME] 的CNAME和 [蒙奇金ID] （与上一步骤中的文本）。

   [CNAME].YourCompany.com > [蒙奇金ID].mktoweb.com

## 添加新CNAME {#add-a-new-cname}

1. IT部门创建CNAME后，转到 **管理员** 的上界。

   ![](assets/add-additional-landing-page-cnames-4.png)

1. 单击 **登陆页面**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. 单击 **新建** 然后选择 **新域别名**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. 输入 **域别名。** 的 **默认页面** 如果访客未放入URL，则会显示。 输入在这种情况下他们应该去的地方。

   >[!NOTE]
   >
   >对于默认页面，您可以选择登陆页面或外部URL，如您的公共网站。

   ![](assets/add-additional-landing-page-cnames-7.png)

1. 输入 **默认页面** 单击 **创建**.

   ![](assets/add-additional-landing-page-cnames-8.png)

不错！ 现在，您知道如果您想添加CNAME，该怎么做。
