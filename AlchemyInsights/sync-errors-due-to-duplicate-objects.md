---
title: 902 (أخطاء المزامنة بسبب الكائنات المكررة)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767102"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>مزامنة الأخطاء بسبب الكائنات المكررة

قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء مزامنة الدليل في Microsoft 365:

- غير قادر على تحديث هذا الكائن في Microsoft Online Services لأن السمات التالية المقترنة بهذا الكائن تحتوي على قيم قد تكون مقترنة بالفعل بكائن آخر في الدليل المحلي.

- يوجد كائن متزامن بنفس عنوان الوكيل بالفعل في دليل خدمات Microsoft عبر الإنترنت.

- غير قادر على تحديث هذا الكائن لأن السمات التالية المقترنة بهذا الكائن لها قيم قد تكون مقترنة بالفعل بكائن آخر في خدمات الدليل المحلي: UserPrincipalName.

لتحديد المشكلة وإصلاحها، قم بتنزيل وتشغيل [أداة معالجة الأخطاء في IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

لمزيد من المعلومات، راجع [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
