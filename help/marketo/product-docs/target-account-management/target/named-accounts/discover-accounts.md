---
unique-page-id: 11378812
description: Discover帐户 — Marketo文档 — 产品文档
title: Discover帐户
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Discover帐户 {#discover-accounts}

使用Discover选项确定潜在的目标帐户。

## 发现CRM帐户 {#discover-crm-accounts}

从您的CRM中确定潜在的目标帐户。

>[!NOTE]
>
>将CRM与Marketo TAM连接后， **发现CRM帐户** 将显示所有CRM帐户和相关信息，以帮助您选择正确的指定帐户。 Marketo会根据从CRM收到的内容添加其他信息。

**人员** (在Discover CRM帐户和Discover Marketo公司中):包括联系人和潜在客户。 使用Marketo [潜在客户到帐户匹配](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**潜在人员** (在Discover CRM帐户和Discover Marketo公司中):显示Marketo发现的可能属于CRM帐户的潜在客户数量。

**自定义CRM字段** （仅在Discover CRM帐户中）：这将帮助您调整销售和营销组织，以选择正确的目标帐户。 一旦 [映射自定义CRM字段](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) 通过Marketo TAM，我们将向您显示映射的数据，以帮助您识别目标帐户。

1. 在指定帐户中，单击 **新建** 下拉框并选择 **发现CRM帐户**.

   ![](assets/disc-crm-one.png)

1. 将打开一个新窗口/选项卡。 选择要添加到指定帐户的CRM帐户，然后单击 **下一个**.

   ![](assets/disc-crm-two.png)

1. 预览屏幕可确认您的选择量。 单击&#x200B;**创建**。

   ![](assets/disc-three.png)

   就这样！

   ![](assets/disc-four.png)

## 了解Marketo公司 {#discover-marketo-companies}

确定要定位的正确公司。

>[!NOTE]
>
>在Discover Marketo公司中，您将看到未来自您的CRM的Marketo公司。

1. 在指定帐户中，单击 **新建** 下拉框并选择 **了解Marketo公司**.

   ![](assets/one-1.png)

1. 将打开一个新窗口/选项卡。 选择要添加到指定帐户的公司，然后单击 **下一个**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >在Discover Marketo公司和Discover CRM中，Marketo会自动：
   >
   >* 查找您的Marketo数据库中记录了该公司的人员。 如果您看到某些属性（例如，行业）的多个值，那是因为Marketo找到了针对这些个人列出的不同值。 点击量最大的属性获胜
   >
   >在 **发现CRM** 仅，Marketo自动：
   >
   >* 同步CRM联系人并将其与指定帐户关联
   >
   >在 **了解Marketo公司** 仅，Marketo自动：
   >
   >* 将大多数互联网服务提供商和公共域名（如yahoo.com、gmail.com）过滤为公司名称
   >
   >* 删除重复的CRM帐户。 如果您在一个记录中有“Acme”和“Acme Inc”（或以下任何后缀）：Co， Corp， Corporation， Gmbh， Inc， Incorporated， LLC， LLP， LP， Ltd， PA， PC， PLC， PLLC)，我们将在TAM中将它们合并为“Acme”

   >
   >如果您希望Marketo按CRM ID或帐户所有者而不是按公司名称来消除重复数据帐户，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

1. 单击“指定帐户”列下方的向下箭头以显示下拉菜单。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今后，这些选定公司的任何新人员都将自动分配给其各自的指定帐户。 请仔细检查这些公司，并确保它们被分配到正确的指定帐户。

1. 要选择现有帐户，请单击 **指定帐户** 下拉菜单，选择所需的帐户，然后单击 **下一个**.

   ![](assets/disc-comp-four.png)

   您还可以选择直接在下拉框中键入所需的名称，以创建新的命名帐户。 完成后，单击离开框……

   ![](assets/disc-comp-five.png)

   ...你会看到你的新命名账户。 此时，只需单击 **下一个** 如步骤4中所示。

   ![](assets/disc-comp-six.png)

1. 单击&#x200B;**创建**。

   ![](assets/disc-comp-seven.png)

   干得好！

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>如果您看到所选的CRM帐户与Discover CRM网格中的内容不匹配，则可能是由于以下一个或多个原因造成的：
>
>* 拥有名称相似且已删除重复的不同CRM帐户
>* 尚未发生下次计划同步


>[!MORELIKETHIS]
>
>[导致帐户匹配](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
