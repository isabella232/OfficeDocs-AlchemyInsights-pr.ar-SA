---
title: حدث خطا في التحقق من صحة خطا الرمز المميز للوصول اثناء تحليلات سطح المكتب علي البواردينج
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783538"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>ظهور رسالة الخطا "حدث خطا في التحقق من صحة الرمز المميز للوصول" اثناء إلحاق تحليلات سطح المكتب

هذا الخطا عاده ما يكون عند انتهاء صلاحيه رمز المصادقة. يؤدي تحديث الصفحة عاده إلى تحديث الرمز المميز. ومع ذلك ، يمكن ان تستمر هذه المشكلة في حاله وجود اي نهج وصول شرطي تم تطبيقه علي الحساب الذي يتم استخدامه لتحليلات سطح المكتب علي اللوحة. يمكنك مراجعه سجلات تسجيل الدخول إلى Azure AD في مدخل Azure لمعرفه ما إذا كان هناك اي عمليات فشل في تسجيل الدخول إلى الحساب الذي يتم استخدامه للحاق تحليلات سطح المكتب.

لمزيد من المعلومات حول الوصول الشرطي ، تفضل بزيارة [تخطيط نشر Access الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).