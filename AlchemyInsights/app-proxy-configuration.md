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
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884771"
---
# <a name="app-proxy-configuration"></a>تكوين وكيل التطبيق

1. لفهم كيفيه تكوين تطبيق وكيل التطبيق داخل Azure AD لعرض تطبيقاتك المحلية إلى السحابة ، راجع [كيفيه تكوين تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. يسمح تسجيل الدخول الأحادي (SSO) للمستخدمين بالوصول إلى أحد التطبيقات من دون المصادقة عده مرات. يسمح هذا الأمر للمصادقة بان تحدث في السحابة ، مقابل Azure Active Directory ، وتسمح للخدمة أو الموصل بانتحال المستخدم لإكمال اي تحديات مصادقه اضافيه من التطبيق. لمعرفه المزيد ، راجع [كيفيه تكوين تسجيل الدخول الأحادي إلى تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. استخدم [هذه المقالة](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) لاستكشاف المشاكل الشائعة التي تواجه الأشخاص وإصلاحها عند إنشاء تطبيق جديد لوكيل التطبيق.
4. إذا كنت تواجه مشكله في اعداد المصادقة النهائية للتطبيق ، فقد تحتاج إلى [استكشاف الأخطاء في تكوينات التفويض المقيدة ل Kerberos لوكيل التطبيق](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) أو اتباع الإرشادات المتعلقة [بتكوين التطبيق باستخدام بينجاكسيس](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) لحل مشكلتك.
