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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030498"
---
# <a name="teams-client-crashing"></a>هل يتوقف عميل Teams عن العمل؟

إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:

- إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- تأكد من توفر إمكانية الوصول إلى جميع [نطاقات URL الخاصة بـ Office 365 وعناوينه](https://docs.microsoft.com/microsoftteams/connectivity-issues).

- سجّل الدخول باستخدام حساب المسؤول الخاص بك وتحقق من[لوحة معلومات حالة الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) للتحقق من عدم وجود انقطاع بالخدمة أو عدم تدنيها.

 - تكمن الخطوة الأخيرة في أن تحاول مسح ذاكرة التخزين المؤقت لعميل Teams لديك:

    1.  قم بالخروج من عميل تطبيق سطح المكتب من Microsoft Teams بشكل كامل. انقر بزر الماوس الأيمن فوق **Teams** من مقطع شريط مهام الأيقونات وانقر فوق **إنهاء** أو قم بتشغيل إدارة المهام وقم بإنهاء العملية بالكامل.

    2.  انتقل إلى مستكشف الملفات واكتب %appdata%\Microsoft\teams.

    3.  بعد الانتقال، سترى بعض الملفات التالية:

         - من داخل **ذاكرة التخزين المؤقت للتطبيق**، انتقل إلى ذاكرة التخزين المؤقت واحذف أي ملفات موجودة في موقع ذاكرة التخزين المؤقت:  %appdata%\Microsoft\teams\application cache\cache.

        - من داخل **Blob_storage**، احذف كل الملفات: %appdata%\Microsoft\teams\blob_storage.

        - من داخل **ذاكرة التخزين المؤقت**، احذف الملفات: %appdata%\Microsoft\teams\Cache.

        - من داخل **قواعد البيانات**، احذف كل الملفات: %appdata%\Microsoft\teams\databases.

        - من داخل **GPUCache**، احذف كل الملفات: %appdata%\Microsoft\teams\GPUcache.

        - من داخل **IndexedDB**، احذف ملف .db file: %appdata%\Microsoft\teams\IndexedDB.

        - من داخل **سعة التخزين المحلية**، احذف كل الملفات: %appdata%\Microsoft\teams\Local Storage.

        - وأخيراً، من داخل **tmp**، احذف أي ملف: %appdata%\Microsoft\teams\tmp.

    4. إعادة تشغيل عميل Teams لديك.
