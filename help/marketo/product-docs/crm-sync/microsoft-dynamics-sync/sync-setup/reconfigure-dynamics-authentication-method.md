---
description: 重新配置Dynamics身份验证方法 — Marketo文档 — 产品文档
title: 重新配置Dynamics身份验证方法
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 重新配置Dynamics身份验证方法 {#reconfigure-dynamics-authentication-method}

请按照以下步骤更新您的动态身份验证方法。

>[!PREREQUISITES]
>
>使用以下任一文章中的所需身份验证方法在Microsoft Dynamics和Active Directory (Azure AD/ADFS)中设置应用程序：
>
>* [第2步（共3步）：设置具有服务器到服务器连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
>* [第2步（共4步）：使用资源所有者密码控制连接设置Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. 在Marketo Engage中，单击 **[!UICONTROL 管理员]**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. 单击 **[!DNL Microsoft Dynamics]**，则 **[!UICONTROL 禁用同步]**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >必须暂时禁用全局同步才能更新身份验证方法。

1. 单击 **[!UICONTROL 重新配置新的身份验证方法]** 选项卡。

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. 选择所需的新身份验证方法（在本例中，我们选择Web API）。

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. 输入新身份验证方法所需的凭据，然后单击 **[!UICONTROL 验证]**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* 特定字段将因选择的身份验证方法而异，并且表单将根据之前的身份验证方法自动更新。
   >* 如果您之前已同步，则可以预先填充上述表单中的数据。 请重新输入所有凭据以确保值正确。

1. 如果一切正常，验证同步将生成所有绿色复选标记 ![](assets/green-check.png). 查看消息并单击 **[!UICONTROL 切换]** 以更新身份验证方法。

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >如果您看到 ![](assets/red-x.png)，该步骤有一个问题。 请参阅 [修复Dynamics验证同步问题](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"} 以识别和修复问题。 然后，重新运行同步验证步骤，直到结果类似于上图。

1. 单击 **[!UICONTROL 确认]** 以继续。

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. 单击 **[!UICONTROL 确认]** 再来一次。

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. 单击 **[!UICONTROL 确定]**.

   >[!IMPORTANT]
   >
   >系统需要15分钟才能接受新的身份验证模式。 请在切换后等待15分钟，然后再重新启用同步。
