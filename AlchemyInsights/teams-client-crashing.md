---
title: Teams تعطل العميل
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321612"
---
# <a name="teams-client-crashing"></a>Teams تعطل العميل

إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:

- إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- تأكد من أن كل Microsoft 365 [عناوين URL ونطاقات](https://docs.microsoft.com/microsoftteams/connectivity-issues) العنوان يمكن الوصول إليها.

- سجل الدخول باستخدام حساب مسؤول [](https://docs.microsoft.com/office365/enterprise/view-service-health) المستأجر وتحقق من لوحة معلومات حالة الخدمة للتحقق من عدم وجود انقطاع أو انخفاض في الخدمة.

- إلغاء تثبيت التطبيق Teams تثبيته
    - استعرض بحثا عن المجلد ٪appdata٪\Microsoft\Teams\ على الكمبيوتر واحذف كل الملفات الموجودة في هذا الدليل.
    - [قم بتنزيل Teams App](https://www.microsoft.com/microsoft-teams/download-app)وتثبيته، وإذا أمكن، Teams كمسؤول (انقر بزر الماوس الأيمن فوق مثبت Teams، وحدد تشغيل **كمسؤول** إذا كان متوفرا).

إذا كان Teams عميلك لا يزال يعطل، فحاول إعادة إنتاج المشكلة. إذا كان ممكنا:

1. استخدم "مسجل الخطوات" لتسجيل الخطوات.
    - أغلق جميع التطبيقات السرية أو غير الضرورية.
    - تشغيل مسجل الخطوات وإعادة إنتاج المشكلة أثناء تسجيل الدخول باستخدام حساب المستخدم المتأثر.
    - [قم بجمع سجلات الفرق التي تسجل خطوات إعادة الحماية المسجلة](https://docs.microsoft.com/microsoftteams/log-files). 
    
    **ملاحظة:** تأكد من تسجيل عنوان تسجيل الدخول للمستخدم الذي تم التأثير عليه.
    - جمع معلومات مستودع تفريغ و/أو خطأ (Windows). تشغيل Windows Powershell على الجهاز الذي يحدث فيه العطل وتشغيل الأوامر التالية (بعد كل أمر، اضغط على Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. بعد إنشاء الملف النصي ويظهر على الشاشة، احفظ الملف وأرفقه بطلب الخدمة. 
