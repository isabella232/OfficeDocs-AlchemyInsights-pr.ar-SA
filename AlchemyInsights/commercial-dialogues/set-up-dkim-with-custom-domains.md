---
title: إعداد DKIM باستخدام مجالات مخصصة
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50742973"
---
# <a name="set-up-dkim-with-custom-domains"></a>إعداد DKIM باستخدام مجالات مخصصة

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
> **DomainGUID** هو النص إلى يسار **.mail.protection.outlook.com** في سجل MX المخصص للمجال المخصص (على سبيل المثال، contoso-com للمجال **contoso.com).** **InitialDomain** هو المجال الذي استخدمته عند تسجيل الدخول إلى Office 365 (على سبيل المثال، **contoso.onmicrosoft.com).**

لمزيد من المعلومات حول سجلات DNS، راجع [إنشاء سجلات DNS لدى أي موفر استضافة DNS ل Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).