---
title: معالجة Teams تسجيل الدخول AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952993"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>معالجة Teams تسجيل الدخول AADSTS9000411

عند تسجيل الدخول إلى Microsoft Teams، قد تتلقى رسالة الخطأ: عذرا، ولكننا نواجه مشكلة في تسجيل الدخول في **AADSTS9000411: لم يتم تنسيق الطلب بشكل صحيح. يتم تكرار المعلمة "login_hint".**

لمعالجة هذه المشكلة، الرجاء التأكد من تحديث Microsoft Teams العملاء. لمزيد من المعلومات حول تحديث العميل، راجع [تحديث](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)Microsoft Teams .

إذا لم تتمكن من تحديث العميل لسبب ما، فإن تسجيل الخروج من العميل سيمسح معظم البيانات المخزنة مؤقتا. ومع ذلك، إذا كانت لا تزال لديك مشاكل بعد تسجيل/تسجيل Teams، يرجى مسح ذاكرة التخزين المؤقت للعميل من خلال القيام بما يلي:
1. أغلق Microsoft Teams.
2. انتقل إلى: ٪appdata٪\microsoft\teams واحذف كل الملفات.
3. أعد فتح Microsoft Teams.
