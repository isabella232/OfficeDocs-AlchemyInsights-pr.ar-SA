---
title: استكشاف الأخطاء OneDrive وإصلاحها
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53920994"
---
# <a name="troubleshoot-onedrive-crashes"></a>استكشاف الأخطاء OneDrive وإصلاحها

إذا OneDrive تعطل بشكل متكرر، فجرب خطوات استكشاف الأخطاء وإصلاحها التالية:

**تأكد من عدم تعيين مفاتيح التسجيل:**

1. باستخدام محرر السجل، انتقل إلى HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. إذا كان DisableFileSyncNGSC موجودا وحدد إلى 1، فافتح المفتاح ثم غير القيمة إلى 0.
3. تشغيل OneDrive يدويا عن طريق الذهاب إلى البدء ![اضغط على Windows المفتاح](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، OneDrive في مربع البحث، ثم انقر فوق OneDrive سطح المكتب.

**إعادة OneDrive:**

ملاحظات:

- إن إعادة OneDrive قطع اتصال كل اتصالات المزامنة الحالية (بما في ذلك اتصالات OneDrive إذا تم إعدادها).
- لن تفقد الملفات أو البيانات عن طريق إعادة OneDrive الكمبيوتر.

**لإعادة تعيين OneDrive:**

1. افتح مربع الحوار تشغيل بالضغط على Windows وR.
2. اكتب ٪localappdata٪\Microsoft\OneDrive\onedrive.exe /reset واضغط على موافق. قد تظهر نافذة الأمر لفترة قصيرة.
3. تشغيل OneDrive يدويا عن طريق الذهاب إلى البدء ![اضغط على Windows المفتاح](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، OneDrive في مربع البحث، ثم انقر فوق OneDrive سطح المكتب.

ملاحظات:

- إذا اخترت مزامنة بعض المجلدات فقط قبل إعادة التعيين، ستحتاج إلى القيام بذلك مرة أخرى بعد اكتمال المزامنة. اقرأ اختر OneDrive المجلدات التي تريد [مزامنتها مع الكمبيوتر](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   للحصول على مزيد من المعلومات.
- ستحتاج إلى إكمال ذلك لمكاتب OneDrive OneDrive for Business.