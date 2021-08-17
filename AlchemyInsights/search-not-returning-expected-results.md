---
title: 1491-search-not-returning-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052697"
---
# <a name="content-search-not-returning-expected-results"></a>لا يؤدي البحث في المحتوى إلى إرجاع النتائج المتوقعة

عند تشغيل "عمليات البحث في Microsoft 365" & مركز التوافق، قد تتلقى نتائج بحث غير متوقعة. يجب عليك التفكير في الأمور التالية التي يمكن أن تؤثر على نتائج البحث:

- **مواقع المحتوى وشروط البحث**: تأكد من تحديد مواقع المحتوى المناسبة وشروط البحث. إذا أجريت عملية بحث كبيرة (مع مواقع متعددة)، ف فكر في تقسيمها إلى عمليات بحث متعددة.

- **العناصر المفهرسة جزئيا**:  [يتم](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) تضمين العناصر المفهرسة جزئيا من علب البريد في نتائج البحث المقدرة. ومع ذلك، لا يتم تضمين العناصر المفهرسة جزئيا من المواقع SharePoint OneDrive في تقدير البحث.

- **حالات** فشل البحث : عند البحث في عدد كبير من علب البريد (أكثر من 100000 علبة بريد)، قد تحصل على أخطاء في البحث، مع رموز الخطأ مثل CS008-009 و CS012-002). في هذه الحالة، ا إعادة محاولة البحث عن مواقع المحتوى الفاشلة فقط. راجع  [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) للحصول على مزيد من المعلومات.
