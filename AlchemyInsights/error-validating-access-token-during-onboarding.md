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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813675"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>رسالة الخطأ "حدث خطأ في التحقق من صحة رمز الوصول المميز" أثناء تشغيل "تحليلات سطح المكتب"

يتم ملاحظة هذا الخطأ عادة عند انتهاء صلاحية رمز المصادقة المميز. عادة، يحدث تحديث الصفحة الرمز المميز. ومع ذلك، يمكن أن تستمر هذه المشكلة إذا كانت هناك أي سياسات وصول شرطي مطبقة على الحساب المستخدم في تحليلات سطح المكتب على اللوحة. يمكنك مراجعة سجلات تسجيل الدخول إلى Azure AD في مدخل Azure لمعرفة ما إذا كان هناك أي حالات فشل في تسجيل الدخول للحساب الذي يتم استخدامه لتكمبيوتر "تحليلات سطح المكتب".

لمزيد من المعلومات حول الوصول الشرطي، تفضل بزيارة [تخطيط نشر الوصول الشرطي.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)