---
title: تكوين وكيل التطبيق
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951552"
---
# <a name="app-proxy-configuration"></a>تكوين وكيل التطبيق

1. لفهم كيفية تكوين تطبيق وكيل التطبيق داخل Azure AD لكشف التطبيقات في السحابة، راجع كيفية تكوين [تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. تسجيل الدخول الفردي (SSO) يسمح للمستخدمين بالوصول إلى تطبيق دون المصادقة عدة مرات. ويسمح بالمصادقة الفردية أن تحدث في السحابة، مقابل Azure Active Directory، ويسمح للخدمة أو الموصل بانتحال هوية المستخدم لإكمال أي تحديات مصادقة إضافية من التطبيق. لمعرفة المزيد، [راجع كيفية تكوين](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)تسجيل الدخول الفردي إلى تطبيق وكيل التطبيق .
3. استخدم [هذه المقالة](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) لا استكشاف المشاكل الشائعة التي يواجهها الأشخاص عند إنشاء تطبيق وكيل تطبيق جديد وإصلاحها.
4. إذا كنت تواجه مشكلة في إعداد مصادقة الخادم للتطبيق، فقد تحتاج إلى استكشاف الأخطاء في تكوينات [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) المقيدة للوفود لوكيل التطبيق وإصلاحها أو اتباع إرشادات حول تكوين التطبيق باستخدام [PingAccess لحل](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) المشكلة.
