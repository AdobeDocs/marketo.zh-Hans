---
unique-page-id: 2359798
description: 添加其他登陆页面CNAME - Marketo文档 — 产品文档
title: 添加其他登陆页面CNAME
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
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

## 查找帐户字符串 {#find-your-account-string}

1. 转到 **管理员** 单击 **登陆页面**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. 复制 **帐户字符串** 从 **设置** 中。

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. 记下它以用于下一步。

## 向IT发送请求 {#send-request-to-it}

1. 请求您的IT部门设置以下CNAME:(替换 [CNAME] 的CNAME和 [帐户字符串] （与上一步骤中的文本）。

   [CNAME].YourCompany.com > [帐户字符串].mktoweb.com

## 添加新CNAME {#add-a-new-cname}

1. IT部门创建CNAME后，请转到 **管理员** 然后单击 **登陆页面**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. 单击 **新建** 然后选择 **新域别名**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. 输入 **域别名。** 的 **默认页面** 如果访客未放入URL，则会显示。 输入在这种情况下他们应该去的地方。

   >[!NOTE]
   >
   >对于默认页面，您可以选择登陆页面或外部URL，如您的公共网站。

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. 输入 **默认页面** 单击 **创建**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

不错！ 现在，您知道如果您想添加CNAME，该怎么做。
