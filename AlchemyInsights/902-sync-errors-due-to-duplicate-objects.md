---
title: 902 (أخطاء المزامنة سبب كائنات مكررة)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456371"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>أخطاء المزامنة نظراً لمضاعفة الكائنات

قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء المزامنة الدليل:
  
- غير قادر على تحديث هذا الكائن في خدمة Microsoft لأن القيم التي قد تكون مقترنة بكائن آخر في الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن.
    
- يوجد بالفعل كائن متزامنة بنفس عنوان الوكيل في دليل "خدمات Microsoft عبر إنترنت".
    
- غير قادر على تحديث هذا الكائن لأن القيم التي قد تكون مقترنة بكائن آخر في خدمات الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن: UserPrincipalName.
    
لتحديد المشكلة وإصلاحها، تحميل وتشغيل [أداة التحديث خطأ DirSync إيدفيكس](https://www.microsoft.com/download/details.aspx?id=36832).
  
لمزيد من المعلومات، انظر [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

