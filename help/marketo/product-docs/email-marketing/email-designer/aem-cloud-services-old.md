---
title: 连接Experience Manager文档
description: 了解如何将Adobe Experience Manager Cloud Services连接到Adobe Marketo Engage，以便您能够利用AEM资源。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 连接Adobe Experience Manager云服务 {#connect-adobe-experience-manager-cloud-services}

了解如何将您的AEM Assets Cloud Services帐户连接到Adobe Marketo Engage实例，以便您可以在Marketo Engage Email Designer中使用AEM资源存储库。

>[!NOTE]
>
>**需要管理员权限**

1. 在Marketo Engage中，转到&#x200B;**管理员**&#x200B;区域并在左侧导航树中选择&#x200B;**Adobe Experience Manager**。

屏幕快照

1. 单击&#x200B;**Adobe Experience Manager云服务**&#x200B;旁边的&#x200B;_编辑_。

屏幕快照

1. 选择一个或多个存储库。

屏幕快照

>[!NOTE]
>
>仅列出在与Marketo Engage订阅相同的IMS组织中关联的存储库。

1. 必须添加[服务凭据证书](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)才能配置存储库。 单击&#x200B;**+添加证书**&#x200B;按钮。

屏幕快照

1. 拖放您的证书（仅限JSON文件），或从您的计算机中选择它。 完成后单击&#x200B;**添加**。

屏幕快照

1. 配置的存储库以及状态和到期如下所示。 单击省略号按钮(**...**)以查看证书。 否则，你就完蛋了。

屏幕快照

现在，可以从Marketo Engage Email Designer访问该存储库中数字资产管理库的所有图像。

>[!MORELIKETHIS]
>
>[使用Experience Manager资源](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
