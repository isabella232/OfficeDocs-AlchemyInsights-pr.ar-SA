---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964791"
---
# <a name="content-search-not-returning-expected-results"></a>البحث عن المحتوى لا يتم إرجاع النتائج المتوقعة

عند تشغيل "محتوى البحث" من & Office 365 أمان مركز التوافق، قد تتلقى نتائج غير متوقعة. خذ بعين الاعتبار الأمور التالية التي يمكن أن تؤثر على نتائج البحث:

- **مواقع المحتوى وشروط البحث**: تأكد من تحديد مواقع المحتوى المناسب وشروط البحث. إذا قمت بتشغيل بحث كبيرة (مع العديد من المواقع)، خذ بعين الاعتبار تقسيمه إلى عدة عمليات البحث.

- **فهرسة العناصر جزئيا**: [فهرسة العناصر جزئيا](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) من علب بريد المضمنة في نتائج البحث المقدر. ومع ذلك، لا يتم تضمين العناصر المفهرسة جزئيا من مواقع SharePoint وأندريف في تقدير البحث.

- **فشل البحث**: عند البحث في عدد كبير من علب البريد (أكثر من 000 100 علب البريد)، قد تتلقى أخطاء البحث، مع رموز الخطأ مثل CS008 009 و CS012-002). في هذه الحالة، أعد محاولة البحث عن مواقع المحتوى الفاشلة فقط. راجع [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) للحصول على مزيد من المعلومات.
