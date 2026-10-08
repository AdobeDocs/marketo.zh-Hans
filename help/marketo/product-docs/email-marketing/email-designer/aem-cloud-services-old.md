---
title: 连接Experience Manager文档
description: 了解如何将AEM云服务连接到Marketo Engage。 在设计器中创作电子邮件时，使用您的AEM资源。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: 'yes'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 8%
---
# 连接Adobe Experience Manager云服务 {#connect-adobe-experience-manager-cloud-services}

了解如何将您的AEM Assets Cloud Services帐户连接到Adobe Marketo Engage实例，以便您可以在Marketo Engage Email Designer中使用AEM资源存储库。

>[!NOTE]
>
>**需要管理员权限**

1. 在Marketo Engage中，转到&#x200B;**管理员**&#x200B;区域并在左侧导航树中选择&#x200B;**Adobe Experience Manager**。

屏幕快照

1. 单击&#x200B;_Adobe Experience Manager云服务_&#x200B;旁边的&#x200B;**编辑**。

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

1. 配置的存储库以及状态和到期如下所示。 单击省略号按钮(**...**) 以查看证书。 否则，您已完成。

屏幕快照

现在，可以从Marketo Engage Email Designer访问该存储库中数字资产管理库的所有图像。

>[!MORELIKETHIS]
>
>[使用Experience Manager资源](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
