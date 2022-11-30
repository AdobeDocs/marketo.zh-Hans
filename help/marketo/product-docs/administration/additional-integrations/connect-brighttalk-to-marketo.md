---
unique-page-id: 15695874
description: 将BrightTALK连接到Marketo - Marketo文档 — 产品文档
title: 将BrightTALK连接到Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# 将BrightTALK连接到Marketo {#connect-brighttalk-to-marketo}

了解如何将BrightTALK渠道连接到Marketo实例。 为此，您必须同时是这两者的管理员。

>[!NOTE]
>
>**需要管理员权限**

## BrightTALK中的步骤 {#steps-in-brighttalk}

1. 登录到 [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;}，单击 **立即连接**.
1. 在“Advanced Marketo Connector（高级连接器）”下，单击 **连接**.
1. 您将转到凭据屏幕，要求您：客户端ID、客户端密钥、身份服务URL和Rest服务URL。 要获取此信息，请登录Marketo。

## Marketo步骤 {#steps-in-marketo}

>[!NOTE]
>
>此时，您将需要设置仅限API用户角色和API用户，以限制BrightTALK在您的Marketo实例中将具有的权限。 由于我们已经有这些步骤的文章，因此我们会将您链接到这些步骤。

1. 创建 [仅API用户角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}。

1. [创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;}，使用您在步骤4中创建的BrightTALK API角色。

1. 返回到“管理员”区域。

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. 在集成下，单击 **LaunchPoint**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. 单击 **新建** 下拉框并选择 **新服务**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. 输入您选择的显示名称。 单击服务下拉列表，然后选择 **自定义** (do _not_ 选择BrightTALK)。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >请记住，不要在下拉菜单中选择BrightTALK。 我们正在删除该字段，选择该字段可能会对您的Marketo/BrightTALK集成造成重大问题。

1. 输入您选择的描述。 单击“仅API用户”下拉列表，然后选择在步骤5中创建的BrightTALK API用户。 单击 **创建**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 单击 **查看详细信息** 对于您刚刚创建的自定义服务。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. 复制（并保存） **客户端ID** 和 **客户端密钥**. 单击 **关闭**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. 在集成下，选择 **Web服务**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. 在Rest API下，复制（并保存） **端点** 和 **身份**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## BrightTALK中的其他步骤 {#additional-steps-in-brighttalk}

1. 从步骤3返回到BrightTALK连接器设置屏幕，然后输入您从步骤12和14保存的凭据。

   凭据验证后，您已正式将BrightTALK连接到Marketo。 下一步是确定 [要同步哪些数据字段](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}。
