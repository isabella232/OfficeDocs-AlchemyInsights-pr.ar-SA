---
title: تعذر إرسال/تلقي البريد الإلكتروني من/Office 365 بسبب تعطيل TLS 1.0 و TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054893"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>تعذر إرسال/تلقي البريد الإلكتروني من/Office 365 بسبب تعطيل TLS 1.0 و TLS 1.1

كما تم تأكيد ذلك في منشور مركز الرسائل MC229914، بدأ إهمال TLS 1.0 و TLS 1.1 بفرض نقاط نهاية تدفق Exchange Online البريد الإلكتروني. قريبا Office 365 قبول اتصالات البريد الإلكتروني TLS 1.0 و TLS 1.1 من المصادر الخارجية. أيضا، Exchange Online تستخدم TLS 1.0 أو 1.1 لإرسال البريد الإلكتروني الصادر. إذا كنت تواجه مشاكل بسبب تعطيل TLS 1.0 أو 1.1، فقد تواجه أحد الأخطاء التالية-

- المرسل يسترد رسائل البريد المرتد ل NDR - '421 4.4.2 تم إسقاط الاتصال بسبب SocketError'
- خطأ في "عارض قائمة الانتظار" للخادم "المحلية" الذي يرسل بريدا إلكترونيا إلى المسؤول 365- "تم إسقاط اتصال 421 4.4.2 بسبب "مأخذ التوصيل"
- خطأ في إرسال سجل [بروتوكول الموصل](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) على الخادم الذي يرسل بريدا إلكترونيا إلى Office 365- فشل التفاوض بشأن TLS مع خطأ SocketError
- خطأ في إرسال سجل بروتوكول الموصل أو تلقيه - '451 5.7.3 يجب أن يتم إصدار أمر STARTTLS أولا'

إذا واجهت أي من الأخطاء أعلاه، فالرجاء التأكد من تمكين TLS 1.2 على الخادم الذي يرسل بريدا إلكترونيا أو يتلقى البريد الإلكتروني من خلال التحقق من مفاتيح التسجيل التالية-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

إذا قمت بإجراء أي تغيير في مفاتيح التسجيل أعلاه لتمكين TLS 1.2، فأعيد تشغيل الخادم لكي يتم تفعيل التغييرات. تأكد أيضا من تثبيت التحديثات Windows Exchange الأخيرة.

لمزيد من المعلومات، اطلع على:

- [Exchange Server إرشادات TLS، الجزء 1: الاستعداد ل TLS 1.2 - مجتمع Microsoft التقني](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server الجزء 2 من إرشادات TLS: تمكين TLS 1.2 وتحديد العملاء الذين لا يستخدمونه - مجتمع Microsoft التقني](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [فهم سيناريوهات البريد الإلكتروني إذا لم يتم الاتفاق على إصدارات TLS مع Exchange Online - مجتمع Microsoft التقني](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
