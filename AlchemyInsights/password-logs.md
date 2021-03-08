---
title: سجلات كلمات المرور
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523354"
---
# <a name="password-logs"></a>سجلات كلمات المرور

**أواجه مشاكل في الوصول إلى سجلات تدقيق إعادة تعيين كلمة المرور**

استكشاف المشاكل المتعلقة بالوصول إلى سجلات تدقيق إعادة تعيين كلمة المرور وإصلاحها، قم بتنفيذ الخطوة التالية:

تأكد من أنك مفوض لعرض سجلات التدقيق. 

الأدوار التالية هي فقط المعتمدة:
 - المسؤول العام
 - مسؤول الأمان
 - قارئ الأمان

**أريد رؤية كل أحداث إعادة تعيين كلمة المرور للتدقيق من وقت نشر كلمة المرور**

يتم تخزين ما يصل إلى 120000 من أحداث إعادة تعيين/تسجيل كلمات المرور في تقارير آخر 30 يوما. ينطبق هذا الحد الأقصى على واجهة المستخدم عند تنزيل CSV. يتوفر 1 مليون حدث من خلال PowerShell.
لمزيد من المعلومات، راجع الارتباطات أدناه:

- [إعادة تعيين أحداث كلمة المرور للخدمة الذاتية من Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [كيفية تنزيل أحداث إعادة تعيين تسجيل كلمات المرور بسرعة باستخدام PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**أريد فهم المزيد حول قدرات إعادة تعيين التقارير بكلمة مرور**

تحقق من الأشخاص الذين يسجلون كلمات المرور أو يعيدون تعيينها باستخدام Azure AD كلمة مرور إعادة تعيين سجلات التدقيق في مدخل Azure ضمن المستخدمين **والمجموعات.**
لمزيد من المعلومات، راجع الارتباطات التالية:

- [نظرة عامة حول إعادة تعيين كلمة المرور للتقارير](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [كيفية عرض تقارير إعادة تعيين كلمة المرور في مدخل Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [إعادة تعيين أحداث كلمة المرور للخدمة الذاتية من Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [كيفية تنزيل أحداث إعادة تعيين تسجيل كلمات المرور بسرعة باستخدام PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


