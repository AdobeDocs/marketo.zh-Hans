---
title: 连接Experience Manager文档
description: 了解如何将Adobe Experience ManagerCloud Service连接到Adobe Marketo Engage，以便您能够利用AEM资源。
hide: true
hidefromtoc: true
source-git-commit: 3a3c3dae689760b720c4823bc1d11bf39da998fe
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 连接Adobe Experience ManagerCloud Service {#connect-adobe-experience-manager-cloud-services}

了解如何将您的AEM AssetsCloud Service帐户连接到Adobe Marketo Engage实例，以便您可以在Marketo Engage电子邮件Designer中利用AEM资源存储库。

>[!NOTE]
>
>**需要管理员权限**

1. 在Marketo Engage中，转到&#x200B;**管理员**&#x200B;区域并在左侧导航树中选择&#x200B;**Adobe Experience Manager**。

屏幕快照

1. 单击&#x200B;_Adobe Experience ManagerCloud Service_&#x200B;旁边的&#x200B;**编辑**。

屏幕快照

1. 选择一个或多个存储库。

屏幕快照

>[!NOTE]
>
>仅列出与您的Marketo Engage订阅在同一IMS组织中关联的存储库。

1. 必须添加[服务凭据证书](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)才能配置存储库。 单击&#x200B;**+添加证书**&#x200B;按钮。

屏幕快照

1. 拖放您的证书（仅限JSON文件），或从您的计算机中选择它。 完成后单击&#x200B;**添加**。

屏幕快照

1. 配置的存储库以及状态和到期如下所示。 单击省略号按钮(**...**)以查看证书。 否则，你就完蛋了。

屏幕快照

现在，可从Marketo EngageEmail Designer访问该存储库中数字资产管理库的所有图像。

>[!MORELIKETHIS]
>
>[使用Experience Manager资源](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
