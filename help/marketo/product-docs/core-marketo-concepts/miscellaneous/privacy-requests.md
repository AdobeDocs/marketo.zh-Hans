---
description: 隐私请求 — Marketo文档 — 产品文档
title: 隐私请求
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 15%

---

# 隐私请求 {#privacy-requests}

本文档概要介绍如何管理可通过Marketo Engage UI和Privacy Service API发送到Privacy Service的单个数据隐私请求。

>[!NOTE]
>
>通过Privacy Service UI或Marketo Engage API提交的隐私请求仅适用于以下内容：
>
>* 已登记到Adobe Identity Management System的Marketo Engage用户
>
>**— 或 —**
>
>* Marketo Engage用户使用Adobe Identity Management System中已存在的其他Experience Cloud产品(例如RT-CDP、B2B和B2P版本、Audience Manager)。

您可以通过两种方式提交单个请求以从Marketo Engage访问和删除消费者数据：

* 通过Privacy Service UI： `https://experience.adobe.com/#/@YOURCOMPANYNAME/privacy`。 请参阅[此处](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=zh-Hans#){target="_blank"}的文档。
* 通过Privacy Service API。 请参阅[此处](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"}的文档和[此处](https://developer.adobe.com/experience-platform-apis/){target="_blank"}的 API 信息。

[Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=zh-Hans){target="_blank"}支持两种类型的请求：数据访问和数据删除。

我们来看看如何创建访问和删除请求。

## 发送Marketo Engage请求所需的设置 {#required-setup-to-send-requests-for-marketo-engage}

要请求访问和删除Marketo Engage的数据，您必须：

1. 确认以下各项：

   a. IMS组织ID<br/>
b.要执行操作的人员的电子邮件地址

   IMS 组织 ID 是一个由 24 个字符组成的字母数字字符串，其后附加有 @AdobeOrg。如果您的营销团队或内部Adobe系统管理员不知道您组织的IMS组织ID，请通过`gdprsupport@adobe.com`联系Adobe客户关怀部门。 您需要 IMS 组织 ID 才能将请求提交到 Privacy API。

1. 在Privacy Service中，您可以将访问和删除请求提交到Marketo Engage，并检查现有请求的状态。

## Marketo Engage JSON请求中的必填字段值 {#required-field-values-in-marketo-engage-json-requests}

“companyContexts”：

* &quot;namespace&quot;：**imsOrgID**
* &quot;value&quot;： `<Your IMS Org ID Value>`

&quot;users&quot;：

* &quot;action&quot;：**access** 或 **delete**
* &quot;userIDs&quot;：
   * &quot;namespace&quot;：**电子邮件**
   * &quot;type&quot;： **standard**
   * &quot;value&quot;： `<Data Subject's Email Address>`

&quot;include&quot;：

* **marketo**(适用于该请求的Adobe产品)

“监管”：

* **gdpr**、**ccpa**、**pdpa**、**lgpd_bra**&#x200B;或&#x200B;**nzpa_nzl**（适用于该请求的隐私法规）

## 示例1：GDPR删除请求 {#gdpr-delete-request}

JSON请求

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

JSON响应

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## 示例二：CCPA访问请求 {#ccpa-access-request}

JSON请求

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

JSON响应

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[隐私管理](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
