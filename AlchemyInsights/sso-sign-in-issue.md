---
title: مشاكل تسجيل الدخول السلسة لمستخدم تسجيل الدخول إلى تسجيل الدخول
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935072"
---
# <a name="seamless-sso-user-sign-in-issues"></a>مشاكل تسجيل الدخول السلسة لمستخدم تسجيل الدخول إلى تسجيل الدخول

بعد مصادقة المستخدم، سيتم تخزين بيانات اعتماد المستخدم مؤقتا في المستعرض نفسه، بحيث يقوم التطبيق تلقائيا تسجيل الدخول باستخدام الحساب نفسه. قد يصعب هذا الأمر على مستخدم آخر أو مستخدم واحد تسجيل الدخول إلى حسابات متعددة على جهاز واحد. لحل هذه المشكلة: 1. حاول تسجيل الدخول على مستعرض آخر. 2. أمسح ذاكرة التخزين المؤقت للمستعرض و/أو ملفات تعريف الارتباط وحاول تسجيل الدخول مرة أخرى.

إذا كنت لا تزال تواجه مشاكل في تسجيل الدخول، نوصي بما يلي لتشخيص خطوات الحل وأتمتةها:

1. ثبت [ملحق](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) مستعرض "التطبيقات الآمنة" لمساعدة Azure Active Directory (Azure AD) لتوفير أفضل تشخيصات و دقة عند استخدام تجربة الاختبار في مدخل Azure.
2. إعادة إنتاج الخطأ باستخدام تجربة الاختبار في صفحة تكوين التطبيق في مدخل Azure. لمعرفة المزيد، راجع تطبيقات تسجيل الدخول الفردية المستندة إلى [Debug SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. إذا كنت تستخدم تجربة الاختبار في مدخل Azure مع ملحق مستعرض التطبيقات الآمنة، يمكنك **تخطي الخطوة 4.**
4. لفتح صفحة تكوين تسجيل الدخول الفردي المستند إلى SAML:
    - افتح مدخل [Azure،](https://portal.azure.com/) ثم سجل الدخول كمسؤول **عام** أو **Coadmin.**
    - افتح **"ملحق Azure Active Directory"** عن طريق تحديد **"كل** الخدمات" في أعلى قائمة التنقل الرئيسية على الجانب الأيمن.
    - اكتب "Azure Active Directory" في مربع البحث في عامل التصفية وحدد عنصر **Azure Active Directory.**
    - حدد **"تطبيقات المؤسسة"** من قائمة التنقل في الجانب الأيسر من Azure Active Directory.
    - حدد **"كافة** التطبيقات" لعرض قائمة بكل التطبيقات. إذا لم يظهر التطبيق الذي تريده هنا،  فاستخدم عنصر تحكم  عامل التصفية في  أعلى قائمة "كل التطبيقات" ثم قم بتعيين الخيار "إظهار" إلى **"كافة التطبيقات".**
    - حدد التطبيق الذي تريد تكوينه من أجل تسجيل الدخول الفردي.
    - بعد تحميل التطبيق، حدد تسجيل **الدخول المفرد** من قائمة التنقل الموجودة على الجانب الأيسر للتطبيق.
    - حدد **SSO قائم على SAML.**
5. استنادا إلى الخطأ، لمعرفة المزيد حول الخطوات المستحسنة التي يجب اتباعها، راجع مشاكل تسجيل الدخول إلى تطبيقات تسجيل الدخول الفردية المستندة إلى SAML التي [تم تكوينها.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. لا استكشاف مشاكل تسجيل الدخول الأخرى للمستخدم وإصلاحها، راجع الإرشادات التالية:
    - [بروتوكول Sign-On SAML مفرد](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [كيفية استكشاف أخطاء تسجيل الدخول وإصلاحها باستخدام تقارير Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [مطالبة موافقة غير متوقعة](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [خطأ في موافقة المستخدم](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [مشاكل في تسجيل الدخول من "تطبيقاتي"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [خطأ على صفحة تسجيل الدخول إلى التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [مشكلة في تسجيل الدخول إلى تطبيق Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
