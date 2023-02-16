---
unique-page-id: 10617187
description: 了解隐私设置 — Marketo文档 — 产品文档
title: 了解隐私设置
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
source-git-commit: bd6f049d5959356a99314e81bb6cfe517c2efdfa
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# 了解隐私设置 {#understanding-privacy-settings}

## 概述 {#overview}

Marketo为营销人员提供了一种获取Web访客同意跟踪他们的方法。 有两种选择退出的方法，或者您可以选择由匿名IP进行跟踪。

* Web访客在其浏览器中选择“不跟踪”(DNT)功能（并且营销人员会执行Web访客的“不跟踪”请求）
* Web访客使用网站上的营销人员提供的选择退出Cookie

或者，营销人员可以跟踪用户，但使用匿名化IP。

这些方法可能会影响Marketo在特定领域的价值和功能。 但是，如果营销人员 *does&#39;t* 更改Marketo配置中的任何内容时，Marketo功能保持不变。

## 不跟踪的浏览器设置 {#browser-settings-for-do-not-track}

Web访客可以通过选择“不跟踪”(DNT)来设置其浏览器以阻止任何网站进行跟踪。 这会阻止跟踪此特定浏览器和设备。 有关完整的详细信息，请参阅浏览器的隐私设置。

在Munchkin中，营销人员可以 [决定是支持还是忽略浏览器的DNT设置](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

在Web个性化中，营销人员可以决定是否 [支持或忽略浏览器的DNT设置](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## 选择退出特定网站 {#opt-out-from-a-specific-website}

您还可以允许网站访客选择退出网站跟踪，无论是否退出 **浏览器不跟踪** 设置。 这允许网站访客直接从您的网站指定其跟踪首选项。

要实现此目的，您必须在启用了Munchkin跟踪的网页上的选择退出链接中添加一个参数。 这可以是任何网页，但网页链接必须包含以下参数：

?marketo_opt_out=true

以下是单击该链接后具有选择退出链接的网页和的登陆页面示例。 你的会有所不同。

这是一个网页，其中带有一个按钮，在选择退出链接中带有“？marketo_opt_out=true”参数。

![](assets/understanding-privacy-settings-1.png)

当单击具有“？marketo_opt_out=true”参数的链接时，您可以创建并发布登陆页面作为后续页面。

![](assets/understanding-privacy-settings-2.png)

单击链接后，Marketo会添加一个名为 **mkto_opt_out** 到访客的浏览器，该浏览器会为使用上述参数单击链接的网站访客禁用Munchkin跟踪。

要验证是否可以种植Cookie，请确认您是Cookie潜在客户，然后单击链接。 然后，检查您的浏览器Cookie以验证 **mkto_opt_out** cookie。

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>目前，该版本仅适用于Munchkin版本152及更高版本。

## 选择启用 {#opt-in}

营销人员可以通过在电子邮件、表单、登陆页面及其他方法中使用Marketo的功能，使用户能够选择加入。

## 使用匿名化IP进行跟踪 {#tracking-using-an-anonymized-ip}

营销人员可以通过使用匿名化IP地址跟踪用户来保护隐私。 为此，请将此代码添加到嵌入到网站中的RTP或Munchkin Javascript中。

* 对于Munchkin，只需将{&quot;anonyizeIP&quot;,true}添加到init函数中即可。

   >[!NOTE]
   >
   >使用此参数要求启用Munchkin V2。 要启用订阅，请联系 [Marketo支持](https://nation.marketo.com/community/support_solutions).

* 对于Web个性化(RTP)，请将此内容添加到Javascript中：

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
