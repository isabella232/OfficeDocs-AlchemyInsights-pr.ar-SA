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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529006"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>لا يحدث الحدث OnChange إذا تم تغيير الحقل برمجيا

لا يحدث الحدث *Onchange* إذا تم تغيير الحقل برمجيا باستخدام *السمة.* أسلوب [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . إذا كنت تريد معالجات الاحداث للحدث *Onchange* لتشغيل بعد تعيين القيمة يجب عليك استخدام *السمة formcontext. data. الوحدة.* أسلوب [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) في التعليمات البرمجية الخاصة بك.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
