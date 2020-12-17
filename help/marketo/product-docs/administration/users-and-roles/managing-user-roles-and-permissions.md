---
unique-page-id: 2359909
description: 管理用户角色和权限- Marketo Docs —— 产品文档
title: 管理用户角色和权限
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---


# 管理用户角色和权限{#managing-user-roles-and-permissions}

设置、创建和编辑用户角色，并将其分配给用户。 这允许您控制每个Marketo用户有权访问的区域和功能。

例如，营销用户通常需要跨应用程序广泛访问，以创建、修改和部署电子邮件、登陆页和项目。 另一方面，Web设计人员几乎将所有时间都花在Design Studio中，创建用于电子邮件和登陆页的资源。 虽然公司领导者在Analytics领域广泛利用Marketo的报告，但他们可能无需自己创建或驱动资产或项目。

>[!NOTE]
>
>**需要管理员权限**

Marketo提供多个内置角色，具有不同级别的访问权限：

* **管理员**-应用程序的所有部分，包括“管理员”部分
* **标准用户**-应用程序的所有部分，“管理员”部分除外
* **营销用户** -应用程序的所有部分，“管理员”部分除外
* **Web设计人员**-仅限Design Studio
* **Analytics用户**-仅限Analytics部分

您无法编辑“管理员”和“标准用户”角色，但可以编辑其他角色。 您还可以创建新的自定义角色，以匹配公司中的特定组织结构。

## 为用户{#assign-roles-to-a-user}分配角色

在您首次[创建用户时或通过[编辑现有用户](managing-marketo-users.md)为用户分配角色。](http://docs.marketo.com/display/DOCS/Create%2C+Delete%2C+Edit+and+Change+a+User+Role)

1. 要编辑现有用户，请转到&#x200B;**Admin**&#x200B;并单击&#x200B;**用户和角色**。

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. 在列表中，选择要编辑的用户，然后单击&#x200B;**编辑用户**。

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. 在&#x200B;**角色**&#x200B;下，根据用户需要的权限选择要分配给用户的角色，然后单击&#x200B;**保存**。

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >要了解每个角色，请参阅[角色权限描述](managing-user-roles-and-permissions/descriptions-of-role-permissions.md)。

## 创建新角色{#create-a-new-role}

有时，您的组织的员工具有非常特定的角色，需要自定义权限组合。

1. 要创建新的用户角色，请转到“管理员”，然后单击“用户和角色”。

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. 单击“角色”选项卡。

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. 单击“新建角色”。

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. 输入角色名称、描述（可选），然后选择此角色中的用户需要的权限。

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## 编辑角色{#edit-a-role}

如果需要更改与现有角色关联的权限，则可以编辑该角色。

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**用户和角色**。

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. 单击**角色**选项卡。

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. 在列表中，选择要修改的角色，然后单击&#x200B;**编辑角色**。

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. 如有必要，请更改&#x200B;**角色名称**&#x200B;和**说明**，然后更改相关&#x200B;**权限**&#x200B;的选择。

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >具有您所编辑角色的用户将在注销后再次登录后收到修改后的权限。

## 删除角色{#delete-a-role}

如果角色变得不必要，您可以删除它。

1. 转到“管理员”并单击“用户和角色”。

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. 单击“角色”选项卡。

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. 在列表中，选择要删除的角色，然后单击删除角色。

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. 单击删除以确认。

   ![](assets/image2014-9-9-18-3a10-3a50.png)

>[!MORELIKETHIS]
>
>在[Marketo入门](../../../getting-started.md)中了解有关创建其他用户并为其分配角色的更多信息。

>[!NOTE]
>
>**深潜**
>
>了解[管理员](http://docs.marketo.com/display/docs/administration)深入篇中的其他管理任务。
