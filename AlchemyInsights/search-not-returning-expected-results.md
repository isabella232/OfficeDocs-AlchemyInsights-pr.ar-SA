---
title: 1491-بحث-لا-إرجاع النتائج المتوقعة
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740461"
---
# <a name="content-search-not-returning-expected-results"></a>لا يرجع بحث المحتوي النتائج المتوقعة

عند تشغيل عمليات البحث عن المحتوي من مركز توافق & أمان Microsoft 365 ، قد تتلقي نتائج بحث غير متوقعه. خذ في الاعتبار الأمور التالية التي يمكنها ان تؤثر علي نتائج البحث:

- **مواقع المحتوي وشروط البحث**: تاكد من انك قمت بتحديد مواقع المحتوي المناسبة وشروط البحث. إذا قمت بتشغيل بحث كبير (باستخدام العديد من المواقع) ، فيمكنك تقسيمها إلى عده عمليات بحث.

- **العناصر المفهرسة جزئيا**: يتم تضمين  [العناصر المفهرسة جزئيا](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) من علب البريد في نتائج البحث المقدرة. ومع ذلك ، لا يتم تضمين العناصر المفهرسة جزئيا من المواقع في SharePoint و OneDrive في تقدير البحث.

- **فشل البحث**: عند البحث في عدد كبير من علب البريد (عبر علب بريد 100,000) ، قد تحصل علي أخطاء في البحث ، مع رموز الخطا مثل CS008-009 و CS012-002). في هذه الحالة ، أعد محاولة البحث لمواقع المحتوي الفاشلة فقط. راجع  [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) للحصول علي مزيد من المعلومات.
