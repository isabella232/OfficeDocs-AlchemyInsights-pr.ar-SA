---
title: 902 (أخطاء المزامنة بسبب تكرار الكائنات)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737328"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>مزامنة الأخطاء بسبب تكرار العناصر

قد تظهر أحدي رسائل الخطا التالية عند انتهاء مزامنة الدليل في Microsoft 365:

- تعذر تحديث هذا الكائن في خدمات Microsoft عبر الإنترنت لان السمات التالية المقترنة بهذا الكائن تحتوي علي القيم التي قد تكون مقترنة بالفعل بكائن آخر في الدليل المحلي.

- يوجد كائن متزامن بنفس عنوان الوكيل بالفعل في دليل Microsoft Online Services.

- تعذر تحديث هذا الكائن لان السمات التالية المقترنة بهذا الكائن تحتوي علي القيم التي قد تكون مقترنة بالفعل بكائن آخر في خدمات الدليل المحلي:.

لتحديد المشكلة وإصلاحها ، قم بتنزيل [أداه تحديث الخطا أداه idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832)وتشغيلها.

لمزيد من المعلومات ، راجع [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
