---
title: المشاكل المتعلقة بتكامل SSO السلسة مع التطبيقات المحلية
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868634"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>المشاكل المتعلقة بتكامل SSO السلسة مع التطبيقات المحلية

لاستكشاف المشاكل المتعلقة بتكامل SSO والتطبيقات المحلية وإصلاحها ، قم بما يلي:

**الخطوات الموصي بها**

1. لتكوين **تطبيق محلي** **لتسجيل الدخول الأحادي عبر وكيل التطبيق**، راجع [فاولتينج كلمه المرور لتسجيل الدخول الأحادي باستخدام وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **استكشاف مشاكل وكيل التطبيق وإصلاحها**: من المستحسن ان تبدا بمراجعه تدفق استكشاف الأخطاء وإصلاحها ، [ومشاكل موصل وكيل التطبيق في Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)، لتحديد ما إذا تم تكوين موصلات وكيل التطبيق بشكل صحيح. إذا كنت لا تزال تواجه مشكله في الاتصال بالتطبيق ، فاتبع خطوات استكشاف الأخطاء وإصلاحها في [تصحيح مشاكل تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). يمكنك [تحديد مشاكل كورس](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) باستخدام أدوات تصحيح المستعرض التالية:
    1. أبدا تشغيل المستعرض واستعرض وصولا إلى تطبيق ويب.
    1. اضغط علي **F12** لإظهار وحده التحكم بالتصحيح.
    1. حاول أعاده إنشاء المعاملة ، ومراجعه رسالة وحده التحكم. ينتج انتهاك كورس خطا في وحده التحكم تتعلق بالأصل.
    1. لا يمكن حل بعض مشاكل كورس ، علي سبيل المثال عندما تتم أعاده توجيه التطبيق إلى login.microsoftonline.com للمصادقة عليه ، وتنتهي صلاحيه الرمز المميز للوصول. ستفشل مكالمة كورس. الحل البديل لهذا السيناريو هو تمديد مده بقاء الرمز المميز للوصول ، لمنع انتهاء صلاحيته اثناء جلسة المستخدم. للحصول علي مزيد من المعلومات حول كيفيه القيام بذلك ، راجع فترات [بقاء الرموز القابلة للتكوين في النظام الأساسي للهوية في Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**المستندات المستحسنة**

- [كيفيه تكوين تسجيل الدخول الأحادي إلى تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML تسجيل الدخول الأحادي للتطبيقات المحلية باستخدام وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [فهم مشاكل كورس وكيل تطبيق Active Directory وحلها](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [استكشاف أخطاء تكوينات التفويض المقيدة ل Kerberos لوكيل التطبيق وإصلاحها](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)