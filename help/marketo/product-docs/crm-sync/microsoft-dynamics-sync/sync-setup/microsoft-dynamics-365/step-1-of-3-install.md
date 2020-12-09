---
unique-page-id: 3571822
description: 步骤1（共3步）-安装Marketo解决方案（在线）- Marketo文档——产品文档
title: 第1步（共3步）-安装Marketo Solution（在线）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# 第1步，共3步：安装Marketo Solution（在线） {#step-of-install-the-marketo-solution-online}

在同步Microsoft Dynamics 365和Marketo之前，您首先需要在Dynamics中安装Marketo解决方案。 **需要动态管理员权限。**

>[!CAUTION]
>
>* `Do not enable custom entity sync before the initial sync is completed. You will be notified via email once the initial sync is completed.`
>* 如果您为Dynamics同步启用了多因素身份验证(MFA)，则必须禁用它，Dynamics才能与Marketo正确同步。 如需其他信息，请与Marketo [支持部门联系](http://nation.marketo.com/community/support_solutions)。

>



>[!NOTE]
>
>将Market同步到CRM后，无法在不替换实例的情况下执行新同步。

>[!PREREQUISITES]
>
>[下载Marketo Lead Management解决方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. 登录** [Microsoft Office 365](https://login.microsoftonline.com/) **。

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. 单击 ![](assets/image2015-3-16-16-3a1-3a13.png)菜单并选 **择CRM**。

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. 单击 ![](assets/image2015-5-13-10-3a5-3a8.png) 菜单。 在下拉菜单中，选择**设置**，然后选择解 **决方案**。

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 单击“ **导入”。**

   ** ![](assets/image2015-3-19-8-3a34-3a8.png)

   **

1. 单击“ **选择文件”。** 选择您下载的Marketo Lead Management解决 [方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 单击“ **下一步**”。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. 视图解决方案信息，然后单击 **视图解决方案包详细信息**。

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. 检查完所有详细信息后，单击“关闭 **”**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 现在，返回“解决方案信息”页面，单击“下 **一步**”。

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 确保选中“SDK选项”复选框。 单击“ **导入**”。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >您需要在浏览器上启用弹出窗口才能完成安装过程。

1. 现在，请等待导入完成。 起来，好好休息一下。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 单击 **关闭。**

   >[!NOTE]
   >
   >您可能会看到一条消息，说明“Marketo Lead Management已完成，但有警告”。 这完全是意料之中的。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo Lead Management现在将出现在解决方案列表中。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 选择“ **Marketto Lead Management** ”，然后单 **击“Publish All Customizations”。**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   击掌！ 安装完成。

   >[!MORELIKETHIS]
   >
   >[第2步，共3步：在Dynamics中设置Marketo同步用户](step-2-of-3-set-up.md)
