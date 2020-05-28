---
title: هل يتوقف عميل Teams عن العمل؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354039"
---
# <a name="teams-client-crashing"></a>هل يتوقف عميل Teams عن العمل؟

إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:

- إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- تأكد من إمكانية الوصول إلى كافة [عناوين URL ونطاقات العناوين من Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- سجّل الدخول باستخدام حساب مسؤول المستأجر وتحقق من [لوحة معلومات صحة الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) للتحقق من عدم وجود انقطاع أو تدهور في الخدمة.

- إلغاء تثبيت تطبيق الفرق وإعادة تثبيته (رابط)
    - استعراض إلى %appdata%\Microsoft\teams\المجلد على جهاز الكمبيوتر الخاص بك وحذف كافة الملفات في هذا الدليل.
    - [قم بتنزيل تطبيق Teams وتثبيته](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)، وإذا كان ذلك ممكنًا ، قم بتثبيت Teams كمسؤول (انقر على مثبت الفرق وحدد "تشغيل كمسؤول" إذا كان متاحًا).

إذا كان عميل Teams لا يزال يتعطل، هل يمكنك إعادة إنشاء المشكلة؟ إذا كان الأمر كذلك:

1. استخدم مسجل الخطوات لالتقاط خطواتك.
    - إغلاق كافة التطبيقات غير الضرورية أو السرية.
    - تشغيل مسجل الخطوات وإعادة إنتاج المشكلة أثناء تسجيل الدخول باستخدام حساب المستخدم المتأثر.
    - [جمع سجلات الفرق التي تلتقط الخطوات repro المسجلة](https://docs.microsoft.com/microsoftteams/log-files). **ملاحظة:** تأكد من التقاط عنوان تسجيل الدخول للمستخدم المتأثر.
    - جمع تفريغ و / أو خطأ دلو معلومات (ويندوز). تشغيل Windows Powershell على الجهاز حيث يحدث التعطل وتشغيل الأوامر التالية:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. إرفاق الملف بحالة الدعم الخاصة بك.
