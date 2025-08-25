---
unique-page-id: 10098433
description: 为基于IP的API访问创建允许列表- Marketo文档 — 产品文档
title: 为基于 IP 的 API 访问创建允许列表
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
source-git-commit: 5d6269ca9b229311ed4260d5340aad6cd1ea0067
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 12%

---

# 为基于 IP 的 API 访问创建允许列表 {#create-an-allowlist-for-ip-based-api-access}

有时，您只想授予API访问特定IP地址或某个地址范围的权限。 为此，首先要启用限制，然后指定允许使用API的IP地址。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>此功能独立于Marketo Engage基于IP的登录限制运行(将由Admin Console的IP访问列表*取代)，并且在[Adobe IMS迁移](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md)后将继续运行。
>> 
>>&#42;IP访问列表计划于2025年第4季度正式发布。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. 单击 **[!UICONTROL Web Services]**。

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. 在&#x200B;**[!UICONTROL IP Restrictions]**&#x200B;区域中，单击&#x200B;**[!UICONTROL Edit]、**&#x200B;或单击左上角的&#x200B;**[!UICONTROL Edit IP Restrictions]**。

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. 选中&#x200B;**[!UICONTROL Enable IP Restrictions]**&#x200B;框并输入要列入允许列表的IP地址。

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >您可以输入单个IP地址或一个IP地址范围，也可以使用通配符。

1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;可打开其他字段以输入更多IP地址。

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
