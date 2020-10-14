---
title: نشر تطبيق Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461725"
---
# <a name="intune-win32-app-deployment"></a>نشر تطبيق Intune Win32

يسمح Microsoft Intune لتطبيقات Win32 ، بما في ذلك لكن لا تقتصر علي MSI و. سيتم نشره في الاجهزه التي تعمل بنظام Windows 10. تتطلب اليه النشر المستخدمة توفر ملحق الاداره ل Intune (IME) علي الجهاز الهدف. سيتم تثبيت محرر أسلوب الإدخال (IME) تلقائيا كنتيجة لاستهداف برنامج powershell نصي أو نشر تطبيق win32 إلى مستخدم/جهاز.

هناك أيضا مجموعه من المتطلبات المسبقة التي يجب تحقيقها من أجل نشر تطبيقات Win32 التي تتضمن:

- الانظمه الاساسيه المعتمدة: الإصدار 1607 أو الأحدث من Windows 10 (الإصدارات Enterprise و Pro والتعليمية).
- البنية المعتمدة: x86 و x64.
- أداره الاجهزه: انضم إلى AAD وتم تسجيله تلقائيا (بما في ذلك المجال المختلط المرتبط بنهج المجموعة والتسجيل التلقائي).
- تنسيق حزمه التطبيق:. **إينتونيوين**  الملفات التي تم تحضيرها بواسطة [أداه تحضير المحتوي Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- تحديد
    - الحد الأقصى للحجم: 8 غيغابايت.
    - الهندسة غير المعتمدة: الأذرع.

راجع المستند "[أضافه تطبيق Win32 وتعيينه ومراقبته في Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" للحصول علي معلومات ذات صله بتلك الخطوات.

تفاصيل حول استكشاف أخطاء نشر التطبيقات علي Windows التي تتضمن تطبيقات Win32 يمكن مراجعتها في المستندات التالية

- [استكشاف مشاكل تثبيت التطبيق وإصلاحها](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [استكشاف أخطاء تطبيقات Win32 وإصلاحها](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)