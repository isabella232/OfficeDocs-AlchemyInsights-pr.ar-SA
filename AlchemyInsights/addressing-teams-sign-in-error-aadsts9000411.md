---
title: AADSTS9000411 خطا تسجيل الدخول إلى الفرق
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
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687025"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>AADSTS9000411 خطا تسجيل الدخول إلى الفرق

عند تسجيل الدخول إلى فرق Microsoft ، قد تتلقي رسالة الخطا: **عذرا ، ولكننا نواجه مشكله في تسجيل الدخول AADSTS9000411: لم يتم تنسيق الطلب بشكل صحيح. المعلمة "login_hint" مكرره.**

لمعالجه هذه المشكلة ، يرجى التاكد من تحديث عملاء فرق العمل في Microsoft. للحصول علي مزيد من المعلومات حول تحديث العميل ، راجع [تحديث فرق Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

إذا لم تتمكن من تحديث العميل لسبب ما ، سيمسح تسجيل خروج العميل معظم البيانات المخزنة مؤقتا. ومع ذلك ، إذا كنت لا تزال تواجه مشاكل بعد تسجيل الخروج/تسجيل الدخول ، فقم بإنهاء الفرق والرجاء مسح ذاكره التخزين المؤقت للعميل عن طريق القيام بما يلي:
1. اغلق فرق Microsoft.
2. انتقل إلى:%appdata%\microsoft\teams واحذف كافة الملفات.
3. أعاده فتح فرق Microsoft.
