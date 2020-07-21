---
title: المستخدم يتلقى خطأ AADSTS7000112 تم تعطيل Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197718"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>المستخدم يتلقى خطأ AADSTS7000112 تم تعطيل Yammer

إذا تلقيت الخطأ "AADSTS7000112: تطبيق '00000005-0000-0ff1-ce00-000000000000000000000' (Yammer) معطلة" ، توجد مشكلة مع أساس الخدمة داخل Azure AD. ربما قام أحد المسؤولين بتعطيل أساس الخدمة لحظر الوصول إلى Yammer.

تعطيل أساس الخدمة غير مستحسن ويمكن أن يسبب مشاكل إضافية. لمزيد من المعلومات حول الأسلوب المعتمد لمنع وصول المستخدم إلى Yammer، راجع [إيقاف تشغيل وصول Yammer لمستخدمي Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

لتصحيح هذه المشكلة في البوابة الإلكترونية أزور واستعادة وصول المستخدم إلى Yammer:

1.  افتح صفحة Azure Active Directory، وحدد **تطبيقات المؤسسة** ضمن **إدارة** في جزء التنقل الأيمن.
3.  اكتب **Yammer Office 365** في مربع البحث، وحدد اسم التطبيق لفتح الإعدادات.
4.  حدد **خصائص** ضمن **إدارة** في جزء التنقل الأيمن.
5.  قم بتعيين قيمة **ممكّن للمستخدمين لتسجيل الدخول إلى** **نعم**، ثم حدد **حفظ**.
6.  تسجيل الدخول إلى Yammer مرة أخرى. قد تحتاج إلى مسح ملفات تعريف الارتباط.

بدلاً من ذلك، قم بتشغيل أوامر PowerShell لتعيين القيمة. لمزيد من المعلومات، راجع [الخطأ "عذراً، ولكن لدينا مشكلة في تسجيل الدخول" عند النقر فوق الإطار المتجانب Yammer في Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 