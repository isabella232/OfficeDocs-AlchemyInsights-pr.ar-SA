---
title: استكشاف أخطاء تعطل OneDrive وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748703"
---
# <a name="troubleshoot-onedrive-crashes"></a>استكشاف أخطاء تعطل OneDrive وإصلاحها

إذا تعطل OneDrive بشكل متكرر، حاول تنفيذ الخطوات التالية لاستكشاف الأخطاء وإصلاحها:

**تأكد من عدم تعيين مفاتيح التسجيل:**

1. باستخدام محرر التسجيل، انتقل إلى HKEY_LOCAL_MACHINE\SOFTWARE\نُهج\Microsoft\OneDrive
2. إذا كان DisableFileSyncNGSC موجوداً وتعيين إلى 1، افتح المفتاح وتغيير القيمة إلى 0.
3. تشغيل OneDrive يدويًا عن طريق الانتقال إلى Start ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، اكتب أندريف في مربع البحث، ثم انقر فوق تطبيق سطح المكتب OneDrive.

**إعادة تعيين أندريف:**

تلاحظ:

- تؤدي إعادة تعيين OneDrive إلى قطع اتصال كافة اتصالات المزامنة الموجودة لديك (بما في ذلك OneDrive الخاص بك في حالة الإعداد).
- لن تفقد الملفات أو البيانات عن طريق إعادة تعيين OneDrive على الكمبيوتر.

**لإعادة تعيين أندريف:**

1. افتح مربع حوار تشغيل بالضغط على مفتاح Windows و R.
2. اكتب %localappdata%\Microsoft\OneDrive\onedrive.exe /إعادة تعيين ثم اضغط موافق. قد يظهر إطار أمر لفترة وجيزة.
3. تشغيل OneDrive يدويًا عن طريق الانتقال إلى Start ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، اكتب أندريف في مربع البحث، ثم انقر فوق تطبيق سطح المكتب OneDrive.

تلاحظ:

- إذا اخترت مزامنة بعض المجلدات فقط قبل إعادة التعيين، فستحتاج إلى القيام بذلك مرة أخرى بمجرد اكتمال المزامنة. اقرأ [اختر المجلدات OneDrive التي تريد مزامنتها مع الكمبيوتر للحصول](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)على مزيد من   المعلومات.
- ستحتاج إلى إكمال هذا لـ OneDrive وOneDrive الخاصين بك.