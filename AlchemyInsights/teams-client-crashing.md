---
title: هل يتوقف عميل Teams عن العمل؟
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826258"
---
# <a name="teams-client-crashing"></a>هل يتوقف عميل Teams عن العمل؟

إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:

- إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- تأكد من إمكانية الوصول إلى كل عناوين URL في [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) ونطاقات عناوينه.

- سجل الدخول باستخدام حساب مسؤول [](https://docs.microsoft.com/office365/enterprise/view-service-health) المستأجر وتحقق من لوحة معلومات حالة الخدمة للتحقق من عدم وجود انقطاع أو انخفاض في الخدمة.

- إلغاء تثبيت تطبيق Teams (ارتباط) وإعادة تثبيته
    - استعرض بحثا عن المجلد ٪appdata٪\Microsoft\teams\ على الكمبيوتر واحذف كل الملفات الموجودة في ذلك الدليل.
    - [قم بتنزيل تطبيق Teams وتثبيته،](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)وإذا أمكن، قم بتثبيت Teams كمسؤول (انقر بزر الماوس الأيمن فوق مثبت Teams وحدد "تشغيل كمسؤول" إذا كان متوفرا).

إذا كان عميل Teams لا يزال يعطل، هل يمكنك إعادة إنتاج المشكلة؟ إذا كان الأمر كذلك:

1. استخدم "مسجل الخطوات" لتسجيل الخطوات.
    - أغلق جميع التطبيقات السرية أو غير الضرورية.
    - تشغيل مسجل الخطوات وإعادة إنتاج المشكلة أثناء تسجيل الدخول باستخدام حساب المستخدم المتأثر.
    - [قم بجمع سجلات الفرق التي تسجل خطوات إعادة الحماية المسجلة](https://docs.microsoft.com/microsoftteams/log-files). **ملاحظة:** تأكد من تسجيل عنوان تسجيل الدخول للمستخدم الذي تم التأثير عليه.
    - جمع معلومات مستودع تفريغ و/أو خطأ (Windows). تشغيل Windows Powershell على الجهاز الذي يحدث فيه العطل وتشغيل الأوامر التالية:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. أرفق الملف بقضيه الدعم.
