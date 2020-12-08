---
unique-page-id: 15695874
description: Connect BrightTALK to Marketo - Marketo Docs —— 产品文档
title: 将BrightTALK连接到Marketo
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# 将BrightTALK连接到Marketo {#connect-brighttalk-to-marketo}

了解如何将BrightTALK渠道与Marketo实例连接。 为此，您必须同时是两者的管理员。

>[!NOTE]
>
>**需要管理员权限**

## BrightTALK中的步骤 {#steps-in-brighttalk}

1. 登录到business.brighttalk.com/demandcentral, [然后](http://business.brighttalk.com/demandcentral/login) 单击“ **立即连接”**。
1. 在“Advanced Marketo Connector（高级营销工具连接器）”下，单 **击“Connect**（连接）”。
1. 您将进入凭据屏幕，询问：客户端ID、客户端机密、标识服务URL和休息服务URL。 要获取此信息，请登录Marketo。

## 营销中的步骤 {#steps-in-marketo}

>[!NOTE]
>
>此时，您将需要设置“仅API用户角色”和“API用户”，以限制BrightTALK在您的Marketo实例中将具有的权限。 因为我们已经有这些步骤的文章，我们会将您链接到这些步骤。

1. 创建仅 [限API的用户角色](http://docs.marketo.com/x/iwMk)。
1. [使用您在步骤](http://docs.marketo.com/x/jwMk)4中创建的BrightTALK API角色创建API用户。
1. 返回“管理员”区域。

   ![](assets/one.png)

1. 在“集成”下，单 **击LaunchPoint**。

   ![](assets/two.png)

1. 单击“ **新建** ”下拉框，然后选 **择“新建服务**”。

   ![](assets/three.png)

1. 输入您选择的显示名称。 单击“服务”下拉框并选 **择“自定** ”( **不选** 择BrightTALK)。

   ![](assets/four.png)

   >[!CAUTION]
   >
   >切记不要在下拉框中选择BrightTALK。 我们正在删除这一领域，选择它可能会在您的Marketo/BrightTALK集成中造成严重问题。

1. 输入您选择的描述。 单击“仅API用户”下拉框，选择您在步骤5中创建的BrightTALK API用户。 单击 **创建**。

   ![](assets/five.png)

1. 单击 **视图** “详细信息”，查看您刚刚创建的自定义服务。

   ![](assets/six.png)

1. 复制（并保存）客 **户端ID** 和客 **户端机密**。 单击 **关闭**。

   ![](assets/eight-1.png)

1. 在“集成”下，选 **择“Web服务**”。

   ![](assets/nine-1.png)

1. 在Rest API下，复制（并保存）终 **点** 和 **标识**。

   ![](assets/ten.png)

## BrightTALK中的步骤 {#steps-in-brighttalk-1}

1. 从步骤3返回至BrightTALK连接器设置屏幕，并输入您从步骤12和14保存的凭据。

   验证凭据后，您已正式将BrightTALK连接到Marketo。 下一步是确 [定要同步的数据字段](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync)。

