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
# <a name="set-up-dkim-with-custom-domains"></a>إعداد DKIM باستخدام المجالات المخصصة

يجب نشر سجلي CNAME لكل مجال مخصص في DNS. للقيام بذلك، استخدم التنسيق التالي:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** هو النص إلى يسار **.mail.protection.outlook.com** في سجل MX المخصص للمجال المخصص (على سبيل المثال، contoso-com لمجال **contoso.com).** **المجال الأولي** هو المجال الذي استخدمته عند تسجيل الدخول إلى Office 365 (على سبيل **المثال،** contoso.onmicrosoft.com).

لمزيد من المعلومات حول سجلات DNS، راجع ["إنشاء سجلات DNS" على أي موفر استضافة DNS ل Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)