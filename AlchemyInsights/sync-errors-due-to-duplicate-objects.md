---
title: 902 (أخطاء المزامنة سبب كائنات مكررة)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420845"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>أخطاء المزامنة نظراً لمضاعفة الكائنات

قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء المزامنة الدليل:

- غير قادر على تحديث هذا الكائن في خدمة Microsoft لأن القيم التي قد تكون مقترنة بكائن آخر في الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن.

- يوجد بالفعل كائن متزامنة بنفس عنوان الوكيل في دليل "خدمات Microsoft عبر إنترنت".

- غير قادر على تحديث هذا الكائن لأن القيم التي قد تكون مقترنة بكائن آخر في خدمات الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن: UserPrincipalName.

لتحديد المشكلة وإصلاحها، تحميل وتشغيل [أداة التحديث خطأ DirSync إيدفيكس](https://www.microsoft.com/download/details.aspx?id=36832).

لمزيد من المعلومات، انظر [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
