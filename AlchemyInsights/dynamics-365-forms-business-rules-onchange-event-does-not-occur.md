---
title: قواعد الأعمال في Dynamics 365 Forms - قاعدة العمل لا يتم فيها إطلاق نموذج
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947286"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>لا يقع الحدث OnChange إذا تم تغيير الحقل برمجيا

لا *يقع الحدث OnChange* إذا تم تغيير الحقل برمجيا باستخدام *السمة.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method. إذا كنت تريد تشغيل معالجات الأحداث لحدث *OnChange* بعد تعيين القيمة، فيجب استخدام *أسلوب سمة formContext.data.entity* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) في التعليمة البرمجية.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
