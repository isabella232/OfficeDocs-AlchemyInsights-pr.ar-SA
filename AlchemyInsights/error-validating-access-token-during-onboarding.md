---
title: حدث خطأ في التحقق من صحة رمز الوصول المميز أثناء "تحليلات سطح المكتب" على متن الطائرة
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946602"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>رسالة الخطأ "حدث خطأ في التحقق من صحة رمز الوصول المميز" أثناء تشغيل "تحليلات سطح المكتب"

يتم ملاحظة هذا الخطأ عادة عند انتهاء صلاحية رمز المصادقة المميز. عادة، يحدث تحديث الصفحة الرمز المميز. ومع ذلك، يمكن أن تستمر هذه المشكلة إذا كانت هناك أي سياسات وصول شرطي مطبقة على الحساب المستخدم في تحليلات سطح المكتب على اللوحة. يمكنك مراجعة سجلات تسجيل الدخول إلى Azure AD في مدخل Azure لمعرفة ما إذا كان هناك أي حالات فشل في تسجيل الدخول للحساب الذي يتم استخدامه لتكمبيوتر "تحليلات سطح المكتب".

لمزيد من المعلومات حول الوصول الشرطي، تفضل بزيارة [تخطيط نشر الوصول الشرطي.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)