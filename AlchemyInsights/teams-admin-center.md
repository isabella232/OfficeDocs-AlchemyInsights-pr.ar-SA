---
title: مركز مسؤولي Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049331"
---
# <a name="teams-admin-center"></a>مركز مسؤولي Teams

تعرّف على ماهية الإدارة في Teams مع [مركز مسؤولي Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

إذا لم تكن قادراً على الوصول إلى مركز مسؤولي Teams، فالرجاء التحقق مما يلي:

- تحقق من أنك قمت بالسماح [بعناوين IP وURL المناسبة لـ Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) على أجهزة المراقبة (جدار الحماية وغير ذلك) أو قواعد جدار الحماية على جهازك المحلي.
- تحقق من أن معلومات تسجيل الدخول التي تستخدمها للوصول إلى مدخل مسؤولي Teams متطابقة مع اسم المستخدم المدرج في [مدخل مسؤولي Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

إذا لم يظهر المستخدمون في مركز مسؤولي Teams، فالرجاء التحقق مما يلي:

- هل قمت بإنشاء مستخدمين أو بتعيين تراخيص خلال 24 ساعة السابقة؟ قبل فتح تذكرة الدعم، الرجاء الانتظار لمدة 24 ساعة على الأقل.
- هل تريد التحقق من أنك قمت بتعيين التراخيص المناسبة؟
- إذا كان لديك Active Directory محلي، فتحقق من أن قيمة [msRTCSIP-PrimaryUserAddress أو عنوان SIP](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) في حقل ProxyAddresses في Active Directory المحلي فريدة ويطابق التنسيق sip: اسم المستخدم من [مركز مسؤولي Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- إذا كنت تنوي الاحتفاظ بنشر Skype for Business Server وكان المستخدمون في وضع النزل و"متصل": اتبع "إعداد مختلط مع Teams و Skype for Business **Online"** في لوحة التحكم في Skype for Business Server وحرك المستخدمين عبر الإنترنت.
