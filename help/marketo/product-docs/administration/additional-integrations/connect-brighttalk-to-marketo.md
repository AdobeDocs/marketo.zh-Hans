---
unique-page-id: 15695874
description: Connect BrightTALK到Marketo - Marketo Docs — 产品文档
title: 将BrightTALK连接到Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 将BrightTALK连接到Marketo {#connect-brighttalk-to-marketo}

了解如何将您的BrightTALK渠道连接到您的Marketo实例。 为此，您必须同时为两者的管理员。

>[!NOTE]
>
>**需要管理权限**

## BrightTALK {#steps-in-brighttalk}中的步骤

1. 登录到[business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login)，然后单击&#x200B;**立即连接**。
1. 在“高级Marketo连接器”下，单击&#x200B;**连接**。
1. 您将进入凭据屏幕，询问：客户端ID、客户端机密、标识服务URL和休息服务URL。 要获取此信息，请登录Marketo。

## Marketo中的步骤{#steps-in-marketo}

>[!NOTE]
>
>此时，您将需要设置“仅API用户角色”和“API用户”，以限制BrightTALK在您的Marketo实例中将具有的权限。 因为我们已经有针对这些步骤的文章，我们会将您链接到这些步骤。

1. 创建[仅API用户角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)。
1. [使用您在步骤](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)4中创建的BrightTALK API角色创建API用户。
1. 返回“管理员”区域。

   ![](assets/one.png)

1. 在“集成”下，单击&#x200B;**LaunchPoint**。

   ![](assets/two.png)

1. 单击&#x200B;**新建**&#x200B;下拉框并选择&#x200B;**新建服务**。

   ![](assets/three.png)

1. 输入您选择的显示名称。 单击“服务”下拉框并选择&#x200B;**Custom**(do _not_ select BrightTALK)。

   ![](assets/four.png)

   >[!CAUTION]
   >
   >切记不要在下拉框中选择BrightTALK。 我们正在删除该字段，选择它可能会使您的Marketo/BrightTALK集成出现严重问题。

1. 输入您选择的说明。 单击“仅API用户”下拉框，然后选择您在步骤5中创建的BrightTALK API用户。 单击&#x200B;**创建**。

   ![](assets/five.png)

1. 单击&#x200B;**视图详细信息**&#x200B;以获取您刚刚创建的自定义服务。

   ![](assets/six.png)

1. 复制（并保存）**客户端ID**&#x200B;和&#x200B;**客户端机密**。 单击&#x200B;**关闭**。

   ![](assets/eight-1.png)

1. 在“集成”下，选择&#x200B;**Web服务**。

   ![](assets/nine-1.png)

1. 在Rest API下，复制（并保存）**Endpoint**&#x200B;和&#x200B;**Identity**。

   ![](assets/ten.png)

## BrightTALK {#additional-steps-in-brighttalk}中的其他步骤

1. 从步骤3返回至BrightTALK连接器设置屏幕，并输入您从步骤12和14保存的凭据。

   验证凭据后，您已正式将BrightTALK连接到Marketo。 下一步是确定要同步的[数据字段。](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync)
