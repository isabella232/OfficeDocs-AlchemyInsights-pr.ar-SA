---
title: استكشاف أخطاء تعطل OneDrive وإصلاحها
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664985"
---
# <a name="troubleshoot-onedrive-crashes"></a>استكشاف أخطاء تعطل OneDrive وإصلاحها

إذا تعطل OneDrive بشكل متكرر ، فجرب خطوات استكشاف الأخطاء وإصلاحها هذه:

**تاكد من عدم تعيين مفاتيح التسجيل:**

1. باستخدام "محرر السجل" ، انتقل إلى HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. إذا كانت ديسابليفيليسينكنجسك موجودة وتم تعيينها إلى 1 ، فافتح المفتاح وغير القيمة إلى 0.
3. تشغيل OneDrive يدويا بالانتقال إلى البدء ![اضغط علي مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، واكتب OneDrive في مربع البحث ، ثم انقر فوق تطبيق OneDrive لسطح المكتب.

**أعاده تعيين OneDrive:**

"

- تؤدي أعاده تعيين OneDrive إلى قطع جميع اتصالات المزامنة الحالية (بما في ذلك OneDrive الشخصي في حاله اعداده).
- لن تفقد الملفات أو البيانات عن طريق أعاده تعيين OneDrive علي الكمبيوتر.

**لأعاده تعيين OneDrive:**

1. افتح مربع الحوار "تشغيل" بالضغط علي مفتاح Windows و R.
2. اكتب% لوكالابداتا% \Microsoft\OneDrive\onedrive.exe/أعاده تعيين واضغط علي موافق. قد تظهر نافذه الأوامر باختصار.
3. تشغيل OneDrive يدويا بالانتقال إلى البدء ![اضغط علي مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)، واكتب OneDrive في مربع البحث ، ثم انقر فوق تطبيق OneDrive لسطح المكتب.

"

- إذا اخترت مزامنة بعض المجلدات فقط قبل أعاده التعيين ، ستحتاج إلى القيام بذلك مره أخرى بعد اكتمال المزامنة. أقرا [اختيار مجلدات OneDrive المراد مزامنتها مع الكمبيوتر](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   للحصول علي مزيد من المعلومات.
- ستحتاج إلى إكمال هذا الاجراء ل OneDrive و OneDrive for Business الشخصي.