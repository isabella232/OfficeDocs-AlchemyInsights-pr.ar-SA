---
title: 902 (أخطاء المزامنة بسبب العناصر المكررة)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998761"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>أخطاء المزامنة بسبب العناصر المكررة

قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء مزامنة الدليل في Microsoft 365:

- يتعذر تحديث هذا الكائن في Microsoft Online Services لأن السمات التالية المقترنة بهذا الكائن لها قيم قد تكون مقترنة بالفعل بكائن آخر في الدليل المحلي.

- يوجد بالفعل كائن متزامن مع عنوان الوكيل نفسه في دليل Microsoft Online Services.

- يتعذر تحديث هذا الكائن لأن السمات التالية المقترنة بهذا الكائن لها قيم قد تكون مقترنة بالفعل بعائن آخر في خدمات الدليل المحلي: UserPrincipalName.

لتحديد المشكلة وإصلاحها، قم بتنزيل أداة تصحيح الأخطاء [IdFix DirSync وتشغيلها](https://github.com/Microsoft/idfix).

لمزيد من المعلومات، [راجع KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
