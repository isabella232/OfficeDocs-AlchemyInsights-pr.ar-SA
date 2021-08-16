---
title: حذف المستخدم المعزول من الخادم
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102225"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>حذف المستخدم المعزول من الخادم

لإزالة مستخدم معزول، اتبع الخطوات التالية:

1. فرض مزامنة الدليل باتباع الإرشادات الواردة في ما هي الهوية [المختلطة مع Azure Active Directory؟](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. للتحقق من مزامنة الدليل، راجع ما هي الهوية [المختلطة مع Azure Active Directory؟](https://technet.microsoft.com/library/jj151797.aspx).

3. إذا كانت المزامنة تعمل بشكل صحيح ولكن حذف الكائن Active Directory لا يتم نشره في Azure AD، فإزالة الكائن المعزول يدويا باستخدام إحدى وحدة Azure Active Directory النمطية التالية Windows PowerShell cmdlets:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    على سبيل المثال، لإزالة بيانات تعريف المستخدم المعزولة john.smith@contoso.com التي تم إنشاؤها في الأصل باستخدام مزامنة الدليل، قم بتشغيل cmdlet:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com