---
title: 1491-البحث-لا إرجاع-المتوقع-النتائج
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510559"
---
# <a name="content-search-not-returning-expected-results"></a>البحث عن المحتوى لا إرجاع النتائج المتوقعة

عند تشغيل عمليات البحث عن المحتوى من مركز التوافق & أمان Microsoft 365، قد تتلقى نتائج بحث غير متوقعة. ضع في اعتبارك الأشياء التالية التي يمكن أن تؤثر على نتائج البحث:

- **مواقع المحتوى وظروف البحث:** تأكد من تحديد مواقع المحتوى المناسبة وظروف البحث. إذا قمت بتشغيل بحث كبير (مع العديد من المواقع)، ففكر في تقسيمه إلى عمليات بحث متعددة.

- **العناصر المفهرسة جزئيًا:** يتم تضمين [العناصر المفهرسة جزئيًا](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) من علب البريد في نتائج البحث المقدرة. ومع ذلك، لا يتم تضمين العناصر المفهرسة جزئيًا من المواقع في SharePoint و OneDrive في تقدير البحث.

- **فشل البحث:** عند البحث في عدد كبير من علب البريد (أكثر من 100,000 علب ة بريد)، قد تحصل على أخطاء البحث، مع رموز الخطأ مثل CS008-009 و CS012-002). في هذه الحالة، إعادة محاولة البحث فقط عن مواقع المحتوى الفاشلة. راجع [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) لمزيد من المعلومات.
