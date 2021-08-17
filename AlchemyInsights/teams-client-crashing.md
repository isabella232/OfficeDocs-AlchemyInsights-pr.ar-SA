---
title: Teams عميلك
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890325"
---
# <a name="teams-client-crashing"></a>Teams عميلك

إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:

- إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- تأكد من أنه Microsoft 365 [عناوين URL ونطاقات](https://docs.microsoft.com/microsoftteams/connectivity-issues) عناوين يمكن الوصول إليها.

- سجل الدخول باستخدام حساب مسؤول [](https://docs.microsoft.com/office365/enterprise/view-service-health) المستأجر وتحقق من لوحة معلومات حالة الخدمة للتحقق من عدم وجود انقطاع أو انخفاض في الخدمة.

- إلغاء تثبيت التطبيق Teams تثبيته
    - استعرض إلى المجلد ٪appdata٪\Microsoft\Teams\ على الكمبيوتر واحذف كل الملفات الموجودة في هذا الدليل.
    - [قم بتنزيل Teams التطبيق](https://www.microsoft.com/microsoft-teams/download-app)، وإذا أمكن، Teams كمسؤول (انقر بزر الماوس الأيمن فوق مثبت Teams، وحدد تشغيل **كمسؤول** إذا كان متوفرا).

إذا كان Teams عميلك لا يزال يعطل، فحاول إعادة إنتاج المشكلة. إذا كان ممكنا:

1. استخدم "مسجل الخطوات" لتسجيل الخطوات.
    - أغلق جميع التطبيقات السرية أو غير الضرورية.
    - تشغيل مسجل الخطوات وإعادة إنتاج المشكلة أثناء تسجيل الدخول باستخدام حساب المستخدم المتأثر.
    - [قم بجمع سجلات الفرق التي تسجل خطوات إعادة الحماية المسجلة](https://docs.microsoft.com/microsoftteams/log-files). **ملاحظة:** تأكد من تسجيل عنوان تسجيل الدخول للمستخدم الذي تم التأثير عليه.
    - تجميع معلومات مستودع تفريغ و/أو خطأ (Windows). تشغيل Windows Powershell على الجهاز الذي يحدث فيه العطل وتشغيل الأوامر التالية (بعد كل أمر، اضغط على Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. بعد إنشاء الملف النصي ويظهر على الشاشة، احفظ الملف وأرفقه بطلب الخدمة. 
