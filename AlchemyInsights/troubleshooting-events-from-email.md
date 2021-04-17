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
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834826"
---
# <a name="troubleshooting-events-from-email"></a>استكشاف الأخطاء في الأحداث وإصلاحها من البريد الإلكتروني

1. التحقق من تمكين الميزة لعلبة البريد: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. ثم انظر إلى سجلات 'الأحداث من البريد الإلكتروني' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. في سجلات "الأحداث من البريد الإلكتروني"، ابحث عن InternetMessageId الذي يتطابق مع العنصر في علبة البريد.  

4. يحدد TrustScore ما إذا كان العنصر مضافا أم لا. لن تضاف الأحداث إلا إذا كانت TrustScore = "موثوق به".

يتم تحديد TrustScore بواسطة خصائص SPF أو Dkim أو Dmarc، والتي توجد في رأس الرسالة.

لعرض هذه الخصائص:

**Outlook لسطح المكتب**

- فتح العنصر
- File -> Properties -> رؤوس الإنترنت

أو

**MFCMapi**

- الانتقال إلى العنصر في علبة الوارد
- ابحث عن PR_TRANSPORT_MESSAGE_HEADERS_W

يتم تحديد هذه الخصائص ويتم تسجيلها أثناء النقل التوجيه. لمزيد من استكشاف الأخطاء وإصلاحها، قد تحتاج إلى المتابعة مع دعم النقل حول حالات الفشل في SPF أو DKIM و.أو DMARC.