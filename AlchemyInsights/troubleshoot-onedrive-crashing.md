---
title: استكشاف أعطل OneDrive وإصلاحها
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826186"
---
# <a name="troubleshoot-onedrive-crashes"></a>استكشاف أعطل OneDrive وإصلاحها

إذا تعطل OneDrive بشكل متكرر، فجرب خطوات استكشاف الأخطاء وإصلاحها التالية:

**تأكد من عدم تعيين مفاتيح التسجيل:**

1. باستخدام محرر السجل، انتقل إلى HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. إذا كان DisableFileSyncNGSC موجودا وحدد إلى 1، فافتح المفتاح ثم غير القيمة إلى 0.
3. تشغيل OneDrive يدويا عن طريق الذهاب إلى البدء ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، اكتب OneDrive في مربع البحث، ثم انقر فوق تطبيق OneDrive لسطح المكتب.

**إعادة تعيين OneDrive:**

ملاحظات:

- تفصل إعادة تعيين OneDrive كل اتصالات المزامنة الموجودة لديك (بما في ذلك OneDrive الشخصي في حالة إعداده).
- لن تفقد الملفات أو البيانات عن طريق إعادة تعيين OneDrive على الكمبيوتر.

**لإعادة تعيين OneDrive:**

1. افتح مربع الحوار تشغيل بالضغط على مفتاح Windows وR.
2. اكتب ٪localappdata٪\Microsoft\OneDrive\onedrive.exe /reset واضغط على موافق. قد تظهر نافذة الأمر لفترة قصيرة.
3. تشغيل OneDrive يدويا عن طريق الذهاب إلى البدء ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، اكتب OneDrive في مربع البحث، ثم انقر فوق تطبيق OneDrive لسطح المكتب.

ملاحظات:

- إذا اخترت مزامنة بعض المجلدات فقط قبل إعادة التعيين، ستحتاج إلى القيام بذلك مرة أخرى بعد اكتمال المزامنة. اقرأ [اختر مجلدات OneDrive التي تريد مزامنتها مع الكمبيوتر للحصول](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)على مزيد من   المعلومات.
- ستحتاج إلى إكمال ذلك ل OneDrive الشخصي و OneDrive for Business.