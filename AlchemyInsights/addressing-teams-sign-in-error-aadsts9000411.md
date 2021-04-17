---
title: خطأ تسجيل الدخول إلى Teams AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821974"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>خطأ تسجيل الدخول إلى Teams AADSTS9000411

عند تسجيل الدخول إلى Microsoft Teams، قد تتلقى رسالة الخطأ: عذرا، ولكننا نواجه مشكلة في تسجيل الدخول في **AADSTS9000411: لم يتم تنسيق الطلب بشكل صحيح. يتم تكرار المعلمة "login_hint".**

لمعالجة هذه المشكلة، يرجى التأكد من تحديث عملاء Microsoft Teams. لمزيد من المعلومات حول تحديث العميل، راجع [تحديث Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

إذا لم تتمكن من تحديث العميل لسبب ما، فإن تسجيل الخروج من العميل سيمسح معظم البيانات المخزنة مؤقتا. ومع ذلك، إذا كانت لا تزال لديك مشاكل بعد تسجيل/تسجيل، فتوقف عن Teams ويرجى مسح ذاكرة التخزين المؤقت للعميل من خلال القيام بما يلي:
1. أغلق Microsoft Teams.
2. انتقل إلى: ٪appdata٪\microsoft\teams واحذف كل الملفات.
3. أعد فتح Microsoft Teams.
