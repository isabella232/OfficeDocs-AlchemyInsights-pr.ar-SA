---
title: ديناميات 365 نماذج قواعد العمل-قاعده الاعمال لا إطلاق النار لنموذج
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769326"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>لا يحدث الحدث OnChange إذا تم تغيير الحقل برمجيا

لا يحدث الحدث *Onchange* إذا تم تغيير الحقل برمجيا باستخدام *السمة.* أسلوب [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . إذا كنت تريد معالجات الاحداث للحدث *Onchange* لتشغيل بعد تعيين القيمة يجب عليك استخدام *السمة formonchange. بيانات. الوحدة* [](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) في التعليمات البرمجية الخاصة بك.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
