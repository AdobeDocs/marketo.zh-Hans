---
description: 电子邮件验证 — Marketo文档 — 产品文档
title: 电子邮件验证
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: f60c40441be4bcfcc277b620f6d4e19b2047caef
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# 电子邮件验证 {#email-verification}

Adobe Marketo Engage订阅要求所有非API用户(包括Marketo Engage管理员)验证其电子邮件地址。 未分配管理员角色的单点登录(SSO)用户在启用电子邮件验证功能后将自动验证其电子邮件。

**用户邀请**

当管理员邀请用户时，该用户在单击“邀请”链接后会自动进行验证。 未分配管理员角色的SSO用户将自动进行验证。

**更改电子邮件地址**

当用户的电子邮件地址发生更改时，该地址会变为未验证。 系统会向他们发送电子邮件，以便他们重新验证。 用户可以通过单击 **重新发送验证**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

**用户和角色**

在管理员>用户和角色中，电子邮件状态列显示每个用户的验证状态。

![](assets/email-verification-3.png)

要向未验证的用户重新发送验证电子邮件，只需选择其记录并单击 **验证电子邮件** 按钮。
