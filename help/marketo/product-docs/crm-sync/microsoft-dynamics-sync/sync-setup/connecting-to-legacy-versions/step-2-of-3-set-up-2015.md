---
unique-page-id: 7504739
description: 安装Marketo for Microsoft Dynamics 2015本地步骤2/3 - Marketo文档 — 产品文档
title: 安装Marketo for Microsoft Dynamics 2015本地步骤2（共3步）
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 步骤3之2：设置Marketo for Dynamics（2015内部部署）{#step-of-set-up-for-marketo-on-premises-2015}

出色完成了前面的步骤。 让我们继续讨论这个问题。

>[!PREREQUISITES]
>
>[安装Marketo for Microsoft Dynamics 2015本地步骤1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)

## 分配同步用户角色 {#assign-sync-user-role}

仅将Marketo同步用户角色分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅 [升级Marketo Microsoft Dynamics解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用户的语言设置 [应设置为英语](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 下 **设置**，单击 **安全性**.

   ![](assets/assign1.png)

1. 单击 **用户**.

   ![](assets/assign2.png)

1. 您将在此处看到用户列表。 选择专用的Marketo同步用户或联系您的 [Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理员创建Marketo的专用用户。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击 **管理角色**.

   ![](assets/assign4.png)

1. 选中Marketo同步用户并单击 **确定**.

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >同步用户应具有对Marketo配置的读取权限。

   >[!TIP]
   >
   >如果您看不到角色，请返回 [第1步（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) 并导入解决方案。

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都将 **非** 已同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们仅做了最后几段配置。

1. 下 **设置**，单击 **Marketo配置**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，请尝试刷新页面。 如果问题仍然存在， [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) 或者尝试注销并重新登录。

1. 单击 **默认**.

   ![](assets/configure2.png)

1. 单击 **Marketo用户** 字段并选择同步用户。

   ![](assets/configure3.png)

1. 单击右下角的保存图标。

   ![](assets/configure4.png)

1. 单击 **发布所有自定义项**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >同步用户应具有对Marketo配置的读取权限。

## 在继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数， [设置自定义同步过滤器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 进程。 它验证初始设置是否正确完成。
* 登录到Microsoft Dynamics CRM中的“Marketo同步用户”。

>[!MORELIKETHIS]
>
>[安装Marketo for Microsoft Dynamics 2015本地步骤3（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md)
