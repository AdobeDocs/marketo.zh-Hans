---
unique-page-id: 10617187
description: 了解隐私设置 — Marketo文档 — 产品文档
title: 了解隐私设置
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 1%

---

# 了解隐私设置 {#understanding-privacy-settings}

## 概述 {#overview}

Marketo为营销人员提供获取Web访客同意进行跟踪的方法。 有两种方式选择退出，或者您可以选择由匿名处理的IP跟踪。

* Web访客在其浏览器中选择不跟踪(DNT)功能（营销人员执行Web访客的“不跟踪”请求）
* Web访客使用营销人员在网站上提供的选择退出Cookie

或者，营销人员可以跟踪用户，但使用匿名化的IP。

这些方法可能会影响Marketo在特定区域中的价值和功能。 但是，如果营销人员&#x200B;_未_&#x200B;更改Marketo配置中的任何内容，则Marketo功能将保持不变。

## “不跟踪”的浏览器设置 {#browser-settings-for-do-not-track}

Web访客可以通过选择“不跟踪”(DNT)来设置浏览器，以防止任何网站进行跟踪。 这样可防止跟踪此特定浏览器和设备。 有关完整的详细信息，请参阅浏览器的隐私设置。

在[!DNL Munchkin]中，营销人员可以[决定是支持还是忽略浏览器的DNT设置](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md)。

在Web Personalization中，营销人员可以决定是[支持还是忽略浏览器的DNT设置](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md)。

## 从特定网站选择退出 {#opt-out-from-a-specific-website}

您还可以允许网站访客从您的网站选择退出网站跟踪，无论是否配置了&#x200B;**浏览器不跟踪**&#x200B;设置。 这允许网站访客直接从您的网站指定其跟踪偏好设置。

为此，必须在启用[!DNL Munchkin]跟踪的网页上向选择退出链接添加参数。 这可以是任何网页，但网页链接必须包含以下参数：

？marketo_opt_out=true

以下是带有选择退出链接的网页示例，以及在单击链接后的登陆页面。 您的会有所不同。

以下网页包含选择退出链接中带有“？marketo_opt_out=true”参数的按钮。

![](assets/understanding-privacy-settings-1.png)

您可以创建登陆页面，并将其发布为单击包含“？marketo_opt_out=true”参数的链接时的跟进页面。

![](assets/understanding-privacy-settings-2.png)

单击该链接时，Marketo会向访客的浏览器添加一个名为&#x200B;**mkto_opt_out**&#x200B;的Cookie，以禁用对使用上述参数单击该链接的网站访客的[!DNL Munchkin]跟踪。

要验证是否可以植入Cookie，请确认您是Cookie潜在客户，然后单击链接。 然后，检查浏览器Cookie以验证是否已添加&#x200B;**mkto_opt_out** Cookie。

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>这当前仅适用于[!DNL Munchkin]版本152及更高版本。

## Opt In {#opt-in}

营销人员可以通过在电子邮件、表单、登陆页面和其他方法中使用Marketo的功能，让用户选择加入。

## 使用匿名化IP进行跟踪 {#tracking-using-an-anonymized-ip}

营销人员可以通过使用匿名处理的IP地址跟踪用户来维护隐私。 为此，请将此代码添加到嵌入到网站中的RTP或[!DNL Munchkin] Javascript中。

* 对于[!DNL Munchkin]，只需将{&quot;anonymizeIP&quot;，true}添加到init函数中。

  >[!NOTE]
  >
  >使用此参数需要启用[!DNL Munchkin] V2。 要为您的订阅启用此功能，请联系[Marketo支持](https://nation.marketo.com/community/support_solutions)。

* 对于Web Personalization (RTP)，请将其添加到Javascript：

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
