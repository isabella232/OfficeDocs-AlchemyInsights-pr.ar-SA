---
title: تعذر إرسال/تلقي البريد الإلكتروني إلى/من Office 365 بسبب تعطيل TLS 1.0 و TLS 1.1
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50742933"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>تعذر إرسال/تلقي البريد الإلكتروني إلى/من Office 365 بسبب تعطيل TLS 1.0 و TLS 1.1

كما تم التأكيد من خلال نشر مركز الرسائل MC229914، بدأ إهمال TLS 1.0 و TLS 1.1 بفرض نقاط نهاية تدفق بريد Exchange Online. قريبا لن يقبل Office 365 اتصالات البريد الإلكتروني TLS 1.0 و TLS 1.1 من المصادر الخارجية. كما لن يستخدم Exchange Online أبدا TLS 1.0 أو 1.1 لإرسال البريد الإلكتروني الصادر. إذا كنت تواجه مشاكل بسبب تعطيل TLS 1.0 أو 1.1، فقد تواجه أحد الأخطاء التالية-

- المرسل يسترد رسائل البريد المرتد ل NDR - '421 4.4.2 تم إسقاط الاتصال بسبب SocketError'
- خطأ في "عارض قائمة الانتظار" للخادم "المحلية" الذي يرسل بريدا إلكترونيا إلى المسؤول 365- "تم إسقاط اتصال 421 4.4.2 بسبب "مأخذ التوصيل"
- خطأ في إرسال سجل بروتوكول [الموصل](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) على الخادم الذي يرسل بريدا إلكترونيا إلى Office 365- فشل التفاوض بشأن TLS مع خطأ SocketError
- خطأ في إرسال سجل بروتوكول الموصل أو تلقيه - '451 5.7.3 يجب أن يتم إصدار أمر STARTTLS أولا'

إذا واجهت أي من الأخطاء أعلاه، فالرجاء التأكد من تمكين TLS 1.2 على الخادم الذي يرسل بريدا إلكترونيا أو يتلقى البريد الإلكتروني من خلال التحقق من مفاتيح التسجيل التالية-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

إذا قمت بإجراء أي تغيير في مفاتيح التسجيل أعلاه لتمكين TLS 1.2، فأعيد تشغيل الخادم لكي يتم تفعيل التغييرات. تأكد أيضا من تثبيت آخر تحديثات Windows و Exchange.

لمزيد من المعلومات، اطلع على:

- [إرشادات Exchange Server TLS، الجزء 1: الاستعداد ل TLS 1.2 - مجتمع Microsoft التقني](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [الجزء 2 من إرشادات Exchange Server TLS: تمكين TLS 1.2 وتحديد العملاء الذين لا يستخدمونه - مجتمع Microsoft التقني](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [فهم سيناريوهات البريد الإلكتروني إذا لم يتم الاتفاق على إصدارات TLS مع Exchange Online - مجتمع Microsoft التقني](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
