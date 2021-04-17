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
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826366"
---
# <a name="teams-admin-center"></a>مركز مسؤولي Teams

تعرّف على ماهية الإدارة في Teams مع [مركز مسؤولي Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

إذا لم تكن قادراً على الوصول إلى مركز مسؤولي Teams، فالرجاء التحقق مما يلي:

- تحقق من أنك قمت بالسماح [بعناوين IP وURL المناسبة لـ Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) على أجهزة المراقبة (جدار الحماية وغير ذلك) أو قواعد جدار الحماية على جهازك المحلي.
- تحقق من أن معلومات تسجيل الدخول التي تستخدمها للوصول إلى مدخل مسؤولي Teams متطابقة مع اسم المستخدم المدرج في [مدخل مسؤولي Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

إذا لم يظهر المستخدمون في مركز مسؤولي Teams، فالرجاء التحقق مما يلي:

- هل قمت بإنشاء مستخدمين أو بتعيين تراخيص خلال 24 ساعة السابقة؟ قبل فتح تذكرة الدعم، الرجاء الانتظار لمدة 24 ساعة على الأقل.
- هل تريد التحقق من أنك قمت بتعيين التراخيص المناسبة؟
- إذا كان لديك Active Directory محلي، فتحقق من أن قيمة [msRTCSIP-PrimaryUserAddress أو عنوان SIP](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) في حقل ProxyAddresses في Active Directory المحلي فريدة ويطابق التنسيق sip: اسم المستخدم من مركز إدارة Microsoft [365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- إذا كنت تنوي الاحتفاظ بنشر Skype for Business Server وكان المستخدمون في وضع النزل وعلى الإنترنت: اتبع "إعداد مختلط مع Teams وسكايب **for Business Online"** في لوحة التحكم في Skype for Business Server وحرك المستخدمين عبر الإنترنت.
