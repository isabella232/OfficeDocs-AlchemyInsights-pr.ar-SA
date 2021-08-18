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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332294"
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
**ملاحظة**: **DomainGUID** هو النص إلى يسار **.mail.protection.outlook.com** في سجل MX المخصص للمجال المخصص (على سبيل المثال، contoso-com لمجال **contoso.com).** **InitialDomain** هو المجال الذي استخدمته عند تسجيل Office 365 (على سبيل **المثال، contoso.onmicrosoft.com).**

لمزيد من المعلومات حول سجلات DNS، راجع إنشاء [سجلات DNS لدى أي موفر استضافة DNS Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).