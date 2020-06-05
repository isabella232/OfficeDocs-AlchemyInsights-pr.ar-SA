---
title: استكشاف الأخطاء وإصلاحها الأحداث من البريد الإلكتروني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568877"
---
# <a name="troubleshooting-events-from-email"></a>استكشاف الأخطاء وإصلاحها الأحداث من البريد الإلكتروني

1. التحقق من تمكين الميزة لصندوق البريد: **Get-EventsFromEmailConfiguration-الهوية <mailbox> **

2. ثم ننظر في 'الأحداث من البريد الإلكتروني' سجلات **تصدير-MailboxDiagnosticLogs <mailbox> -مكون TimeProfile**

3. في سجلات "الأحداث من البريد الإلكتروني"، ابحث عن InternetMessageId الذي يطابق العنصر في علبة البريد.  

4. يحدد TrustScore ما إذا تمت إضافة العنصر أم لا. سيتم إضافة الأحداث فقط إذا كان TrustScore = "موثوق به".

يتم تحديد نقاط الثقة بواسطة خصائص SPF أو Dkim أو Dmarc الموجودة في رأس الرسالة.

لعرض هذه الخصائص:

**توقعات سطح المكتب**

- فتح العنصر
- خصائص > الملف -> رؤوس إنترنت

او

**MFCMapi**

- الانتقال إلى العنصر الموجود في البريد الوارد
- ابحث عن PR_TRANSPORT_MESSAGE_HEADERS_W

يتم تحديد هذه الخصائص وتسجيلها أثناء النقل والتوجيه. لمزيد من استكشاف الأخطاء وإصلاحها، قد تحتاج إلى متابعة مع دعم النقل حول الفشل في SPF و DKIM و.أو DMARC.