---
description: 隐私请求 — Marketo文档 — 产品文档
title: 隐私请求
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 5aa75cc35ef8d39983563ab34b075ae580f9a97b
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 隐私请求 {#privacy-requests}

本文档概述了如何管理可通过Privacy ServiceUI和Privacy ServiceAPI发送给Marketo Engage的单个数据隐私请求。

>[!NOTE]
>
>通过Privacy ServiceUI或API提交的Marketo Engage请求仅适用于以下内容：
>
>* Marketo Engage已载入AdobeIdentity Management系统的用户
>
>**-或-**
>
>* Marketo Engage用户使用AdobeIdentity Management系统上已有的其他Experience Cloud产品(例如RT-CDP、B2B和B2P版本、Audience Manager)。


您可以通过两种方式提交单个请求以从Marketo Engage中访问和删除消费者数据：

* 通过 [Privacy ServiceUI](https://privacyui.cloud.adobe.io/). 请参阅此文档 [此处](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html){target=&quot;_blank&quot;}。
* 通过Privacy ServiceAPI。 请参阅此文档 [此处](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target=&quot;_blank&quot;}和API信息 [此处](https://developer.adobe.com/experience-platform-apis/){target=&quot;_blank&quot;}。

的 [Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html){target=&quot;_blank&quot;}支持两种类型的请求：数据访问和数据删除。

让我们看看如何创建访问和删除请求。

## 发送Marketo Engage请求所需的设置 {#required-setup-to-send-requests-for-marketo-engage}

要请求访问和删除Marketo Engage数据，您必须：

1. 识别以下内容：

   a.IMS组织ID<br/>
b.要执行操作的人员的电子邮件地址

   IMS组织ID是一个由24个字符组成的字母数字字符串，其后附加有@AdobeOrg。 如果您的营销团队或内部Adobe系统管理员不知道您组织的IMS组织ID，请通过gdprsupport@adobe.com联系Adobe客户关怀团队。 您需要IMS组织ID才能向隐私API提交请求。

1. 在Privacy Service中，您可以提交访问和删除请求以Marketo Engage，并检查现有请求的状态。

## Marketo EngageJSON请求中的必填字段值 {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;users&quot;:

* &quot;action&quot;:e **访问** 或 **删除**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **电子邮件**
   * &quot;type&quot;: **标准**
   * &quot;value&quot;: `<Data Subject’s Email Address>`

&quot;include&quot;:

* **marketo** (即适用于请求的Adobe产品)

&quot;regulation&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra**&#x200B;或 **nzpa_nzl**  （即适用于该请求的隐私法规）

## 示例一：GDPR删除请求 {#gdpr-delete-request}

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
