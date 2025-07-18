---
unique-page-id: 3571807
description: 第2步（共3步） — 在Dynamics中设置Marketo同步用户（2011年内部部署） - Marketo文档 — 产品文档
title: 第2步（共3步） — 在Dynamics中设置Marketo同步用户（2011年内部部署）
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 1%

---

# 步骤2（共3步）：在Dynamics中设置Marketo同步用户（2011内部部署） {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

出色完成了前面的步骤，让我们继续介绍这些步骤。

>[!PREREQUISITES]
>
>[第1步（共3步）：安装Marketo解决方案（2011年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## 分配同步用户角色 {#assign-sync-user-role}

仅将Marketo同步用户角色分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo插件版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅[升级MarketoMicrosoft Dynamics解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}。

>[!IMPORTANT]
>
>同步用户[的语言设置应设置为“英语](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}”。

1. 在左下方的菜单中，选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. 在树中选择&#x200B;**[!UICONTROL Administration]**。

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 选择 **[!UICONTROL Users]**。

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. 您将在此处看到用户列表。 选择您的专用Marketo同步用户或联系您的[Active Directory联合身份验证服务(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"}管理员以创建专用于Marketo的新用户。 单击 **[!UICONTROL Manage Roles]**。

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 检查&#x200B;**[!UICONTROL Marketo Sync User]**&#x200B;并单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >如果未看到该角色，请返回3[&#128279;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}的步骤1并导入解决方案。

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都&#x200B;_不会_&#x200B;同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们仅做了最后几段配置。

1. 选择&#x200B;**[!UICONTROL Settings]**。 然后在树中选择&#x200B;**[!UICONTROL Marketo Config]**。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，请尝试刷新页面。 如果问题仍然存在，请[再次发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}或注销并重新登录。

1. 单击 **[!UICONTROL Default]**。

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. 单击![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. 在弹出窗口中，选择同步用户。 接着，单击 **[!UICONTROL OK]**。

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;保存更改。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 单击 **[!UICONTROL Publish All Customizations]**。

   ![](assets/publish-all-customizations1.png)

## 在继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步记录数，请立即[设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}。
* 运行[验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}进程。 它验证初始设置是否正确完成。
* 登录到Microsoft Dynamics CRM中的Marketo同步用户。

  做得好！

>[!MORELIKETHIS]
>
>[第3步（共3步）：将Microsoft Dynamics与Marketo连接（2011年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md){target="_blank"}
