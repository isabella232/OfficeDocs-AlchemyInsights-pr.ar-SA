---
title: حذف مستخدم المعزول من خادم محلي
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197762"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>حذف مستخدم المعزول من خادم محلي

لإزالة مستخدم المعزول اتبع الخطوات التالية:

1. فرض مزامنة الدليل باتباع الإرشادات في [ما هي الهوية المختلطة مع Azure Active Directory؟](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. للتحقق من مزامنة الدليل، راجع [ما هي الهوية المختلطة مع Azure Active Directory؟](https://technet.microsoft.com/library/jj151797.aspx).

3. إذا كانت مزامنة دالات بشكل صحيح ولكن لا نشر حذف كائن Active Directory إلى إعلان Azure يدوياً إزالة الكائن المعزول باستخدام أحد الوحدة النمطية "Active Directory أزور" التالية لـ Windows PowerShell cmdlets:

    إزالة-MsolContact  
    إزالة-MsolGroup  
    إزالة-MsolUser

    على سبيل المثال، لإزالة معرف المستخدم المعزول john.smith@contoso.com، تم إنشاؤها في الأصل باستخدام مزامنة الدليل، قم بتشغيل cmdlet:

    إزالة MsolUser -UserPrincipalName John.Smith@Contoso.com