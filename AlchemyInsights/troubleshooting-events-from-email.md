---
title: استكشاف الأخطاء في الأحداث وإصلاحها من البريد الإلكتروني
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105339"
---
# <a name="troubleshooting-events-from-email"></a>استكشاف الأخطاء في الأحداث وإصلاحها من البريد الإلكتروني

1. التحقق من تمكين الميزة لعلبة البريد: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. ثم انظر إلى سجلات 'الأحداث من البريد الإلكتروني' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. في سجلات "الأحداث من البريد الإلكتروني"، ابحث عن InternetMessageId الذي يتطابق مع العنصر في علبة البريد.  

4. يحدد TrustScore ما إذا كان العنصر مضافا أم لا. لن تضاف الأحداث إلا إذا كانت TrustScore = "موثوق به".

يتم تحديد TrustScore بواسطة خصائص SPF أو Dkim أو Dmarc، والتي توجد في رأس الرسالة.

لعرض هذه الخصائص:

**سطح المكتب Outlook**

- فتح العنصر
- File -> Properties -> رؤوس الإنترنت

أو

**MFCMapi**

- الانتقال إلى العنصر في علبة الوارد
- ابحث عن PR_TRANSPORT_MESSAGE_HEADERS_W

يتم تحديد هذه الخصائص ويتم تسجيلها أثناء النقل التوجيه. لمزيد من استكشاف الأخطاء وإصلاحها، قد تحتاج إلى المتابعة مع دعم النقل حول حالات الفشل في SPF أو DKIM و.أو DMARC.