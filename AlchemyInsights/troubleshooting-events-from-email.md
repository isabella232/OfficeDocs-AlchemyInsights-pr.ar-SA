---
title: استكشاف الأخطاء وإصلاحها من البريد الكتروني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658721"
---
# <a name="troubleshooting-events-from-email"></a>استكشاف الأخطاء وإصلاحها من البريد الكتروني

1. تاكد من تمكين الميزة لعلبه البريد: **الحصول علي افينتسفروميميلكونفيجوريشن <mailbox> الهوية**

2. ثم انظر علي سجلات "الاحداث من **البريد الكتروني" التصدير-ميلبوكسدياجنوستيكلوجس <mailbox> -مكون تيميبروفيلي**

3. في سجلات "الاحداث من البريد الكتروني" ، ابحث عن إينتيرنيتميساجيد الذي يتطابق مع العنصر في علبه البريد.  

4. يحدد تروستسكوري ما إذا تمت أضافه العنصر ام لا. ستتم أضافه الاحداث فقط إذا كانت تروستسكوري = "موثوق بها".

يتم تحديد تروستسكوري بواسطة SPF أو Dkim أو Dmarc الخصائص ، وهي موجودة في راس الرسالة.

لعرض الخصائص التالية:

**سطح المكتب Outlook**

- فتح العنصر
- خصائص الملفات >-> رؤوس الإنترنت

or

**مفكمابي**

- الانتقال إلى العنصر الموجود في علبه الوارد
- البحث عن PR_TRANSPORT_MESSAGE_HEADERS_W

يتم تحديد هذه الخصائص وتسجيلها اثناء النقل والتوجيه. لمزيد من استكشاف الأخطاء وإصلاحها ، قد تحتاج إلى متابعه دعم النقل حول حالات الفشل في SPF و DKIM و. أو DMARC.