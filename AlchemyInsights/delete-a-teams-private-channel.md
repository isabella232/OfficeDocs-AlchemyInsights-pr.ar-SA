---
title: حذف القناة الخاصة بالفرق
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730902"
---
# <a name="delete-a-teams-private-channel"></a>حذف القناة الخاصة بالفرق

ان Microsoft علي علم بوجود مشكله في حذف القناة الخاصة بفرق العمل الخاصة إذا كان لديك نهج استبقاء SharePoint ممكنة لموقع SharePoint الأساسي. تعمل Microsoft علي تصحيح. في الوقت نفسه ، يمكنك استخدام الحلول البديلة التالية لحذف القناة الخاصة.

**استبعاد الفريق/مجموعه المواقع المشتركة من نهج الاستبقاء في Sharepoint.**

1. انتقل إلى مدخل أداره Office 365 ، وحدد **إظهار الكل** في جزء التنقل الأيمن.
2. ضمن **مراكز الاداره**، انتقل إلى نهج تفادي فقدان بيانات **التوافق في & الأمان**  >  **Data Loss Prevention**  >  **Policy**.
3. حدد اي نهج ينطبق علي مواقع Sharepoint ، وقم بتعديل النهج بحيث لا يتم تضمين موقع Sharepoint للفريق الذي يحتوي علي القناة الخاصة ضمن نهج الاستبقاء.
4. احفظ النهج.
    قد يستغرق الأمر مده تصل إلى 24 ساعة لكي تدخل إعدادات النهج حيز التنفيذ.
    بعد استبعاد الموقع ، يمكنك حذف القناة الخاصة.  
    
***قد*** تتمكن من حذف القناة الخاصة باستخدام فرق Microsoft علي جهازك الذي يعمل بنظام Android. 

للحصول علي معلومات SharePoint ذات الصلة ، راجع [تعذر حذف العناصر في SharePoint Online أو OneDrive For business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).