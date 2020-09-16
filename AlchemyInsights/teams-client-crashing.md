---
title: هل يتوقف عميل Teams عن العمل؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691094"
---
# <a name="teams-client-crashing"></a>هل يتوقف عميل Teams عن العمل؟

إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:

- إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- تاكد من امكانيه الوصول إلى كل [عناوين url ونطاقات عناوين Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) .

- سجل الدخول باستخدام حساب مسؤول المستاجر الخاص بك ، وتحقق من [لوحه معلومات حماية الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) للتحقق من عدم وجود اي انقطاع أو انخفاض في الخدمة.

- إلغاء تثبيت تطبيق الفرق وأعاده تثبيته (ارتباط)
    - استعرض وصولا إلى المجلد%appdata%\Microsoft\teams\ علي الكمبيوتر واحذف كل الملفات في هذا الدليل.
    - قم [بتنزيل تطبيق الفرق وتثبيته](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)، ويمكنك تثبيت الفرق كمسؤول (بالنقر بزر الماوس الأيمن فوق مثبت الفرق وتحديد "تشغيل كمسؤول" في حال توفره).

إذا ما زال عميل الفرق معطلا ، فهل يمكنك أعاده إنتاج المشكلة ؟ إذا كان الأمر كذلك:

1. استخدم مسجل الخطوات لتسجيل الخطوات.
    - اغلق جميع التطبيقات غير الضرورية أو السرية.
    - أبدا تشغيل مسجل الخطوات واعد إنشاء المشكلة اثناء تسجيل الدخول باستخدام حساب المستخدم المتاثر.
    - [جمع سجلات الفرق التي تلتقط خطوات أعاده المسجلة](https://docs.microsoft.com/microsoftteams/log-files). **ملاحظه**: تاكد من انك تلتقط عنوان تسجيل الدخول الخاص بالمستخدم المتاثر.
    - جمع معلومات التفريغ الخاصة بالنسخة الاحتياطية و/أو الخطا (Windows). شغل Windows Powershell علي الجهاز الذي تحدث فيه التعطل وشغل الأوامر التالية:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. قم بإرفاق الملف بحاله الدعم.
