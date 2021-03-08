---
title: إعداد DKIM باستخدام المجالات المخصصة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523126"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="13072-102">إعداد DKIM باستخدام المجالات المخصصة</span><span class="sxs-lookup"><span data-stu-id="13072-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="13072-103">يجب نشر سجلي CNAME لكل مجال مخصص في DNS.</span><span class="sxs-lookup"><span data-stu-id="13072-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="13072-104">للقيام بذلك، استخدم التنسيق التالي:</span><span class="sxs-lookup"><span data-stu-id="13072-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="13072-105">**DomainGUID** هو النص إلى يسار **.mail.protection.outlook.com** في سجل MX المخصص للمجال المخصص (على سبيل المثال، contoso-com لمجال **contoso.com).**</span><span class="sxs-lookup"><span data-stu-id="13072-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="13072-106">**المجال الأولي** هو المجال الذي استخدمته عند تسجيل الدخول إلى Office 365 (على سبيل **المثال،** contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="13072-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="13072-107">لمزيد من المعلومات حول سجلات DNS، راجع ["إنشاء سجلات DNS" على أي موفر استضافة DNS ل Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="13072-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>