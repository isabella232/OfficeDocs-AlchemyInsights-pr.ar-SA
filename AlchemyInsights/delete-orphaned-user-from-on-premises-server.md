---
title: حذف المستخدم المعزول من الخادم المحلي
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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680122"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>حذف المستخدم المعزول من الخادم المحلي

لأزاله مستخدم معزول ، اتبع الخطوات التالية:

1. فرض مزامنة الدليل باتباع الإرشادات [الموجودة في الهوية المختلطة باستخدام Azure Active directory ؟](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. للتحقق من مزامنة الدليل ، راجع [ما المقصود بالهوية المختلطة باستخدام Azure Active directory ؟](https://technet.microsoft.com/library/jj151797.aspx).

3. إذا كانت الدالة متزامنة بشكل صحيح ولكن حذف كائن Active directory لا يقوم بالنشر في Azure AD ، فقم بازاله الكائن المعزول يدويا باستخدام أحد الوحدة النمطية التالية ل Azure Active directory ل Windows PowerShell:

    أزاله-مسولكونتاكت  
    أزاله-مسولجروب  
    أزاله-مسولوسير

    علي سبيل المثال ، لأزاله معرف المستخدم المعزول john.smith@contoso.com ، الذي تم إنشاؤه في الأصل باستخدام مزامنة الدليل ، قم بتشغيل أمر cmdlet:

    أزاله-مسولوسير-John.Smith@Contoso.com