---
title: 导入 — 资产 — 与adobe-experience-manager
description: 使用Adobe Experience Manager导入资源
exl-id: f22be520-c1ea-4e7e-9fc4-cdbee34d27a4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# 使用Adobe Experience Manager导入资源

<br> 

资产选取器允许[!DNL Marketo]客户访问、选择AEM资产并将其导入[!DNL Marketo's] [!UICONTROL Design Studio]。 您必须是管理员才能执行这些步骤。

>[!NOTE]
>[!DNL Adobe Experience Manager (AEM)] 是独立产品，必须单独购买。 请联系您的客户成功经理以了解更多信息。

>[!IMPORTANT]
>请确保已在[!DNL Marketo Classic]中执行[AEM配置](https://docs.marketo.com/x/FwPLAQ)。

>[!CAUTION]
>
>目前，仅Firefox完全支持此功能。 Safari中不支持此功能，并且可能无法在最新版Chrome中工作，具体取决于您的SameSite Cookie设置。

1. 在[!UICONTROL Design Studio]中，选择&#x200B;**[!UICONTROL Images and Files]**。

   ![图像1](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-1.png)

1. 单击[!UICONTROL Images and Files]下拉框并选择&#x200B;**[!UICONTROL Import Image or File]**。

   ![图2](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-2.png)

1. 单击[!DNL Adobe Experience Manager]旁边的单选按钮，然后单击&#x200B;**[!UICONTROL Next]**。

   ![图3](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-3.png)

1. 登录到[!DNL Adobe Experience Manager]。

   ![图4](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-4.png)

1. 选择您的文件夹。 选择所需的图像（最多可选择10张），然后单击&#x200B;**[!UICONTROL Select]**。

   ![图像5](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-5.png)

   >[!NOTE]
   >
   >图像大小不能超过100MB。

1. 验证您选择的图像，选择目标文件夹（[!UICONTROL Images and Files]是默认文件夹），然后单击&#x200B;**[!UICONTROL Next]**。

   ![图6](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-6.png)

就这样！ 单击&#x200B;**[!UICONTROL Close]**&#x200B;返回到“Images and Files（图像和文件）”。

![图七](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-7.png)

## 注意事项

* [!DNL Marketo] 目前支 [!DNL Adobe Experience Manager] 持版本6.4和6.5。
* 实例中的所有用户都将能够视图/访问您导入的图像。
* 图像不会自动更新。 如果导入到[!DNL Marketo] [!UICONTROL Design Studio]中的图像在AEM中更新，则必须手动将其重新导入到[!DNL Marketo]中。
