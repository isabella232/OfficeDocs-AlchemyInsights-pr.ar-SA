---
title: الوصول إلى الاشتراك
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807157"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>تعذر تسجيل الدخول في Azure بسبب مشاكل في المستعرض (يتوقف المستعرض ، ولكنه لا يتم تحميله ، وغير ذلك.)

قد تتاثر بالانقطاع. يرجى التحقق لمعرفه ما إذا كان هناك انقطاع مستمر: [حاله حماية Azure](https://status.azure.com/status/history/).

يرجى تسجيل الخروج من كل جلسات عمل Azure النشطة. أبدا تشغيل وضع خاص أو نافذه تصفح متخفي في مستعرض الويب.

يمكنك أيضا محاولة تحديث المستعرض ، واستخدام مستعرض آخر ، حذف ملفات تعريف الارتباط الخاصة بذاكره التخزين المؤقت إذا لم ينجح ذلك.

تعرف علي المزيد: [استكشاف مشاكل تسجيل الدخول وإصلاحها](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**تعذر الوصول إلى الاشتراكات**

في [مدخل azure](https://portal.azure.com/)، تاكد من تحديد دليل azure الصحيح من الحساب في الجزء العلوي الأيسر.

في [مركز حسابات Azure](https://account.windowsazure.com/Subscriptions)، تاكد من ان الحساب المستخدم هو مسؤول الحساب.

معرفه المزيد: [استكشاف الأخطاء وإصلاحها لم يتم العثور علي اشتراكات](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**تعذر الوصول إلى محفوظات الفوترة**

يحتاج مسؤول الحساب إلى التاكد من أضافه المستخدم الذي يقوم بالوصول إلى معلومات الفوترة في Azure Active directory كمستخدم ضيف: [أضافه مستخدم جديد أو حذفه](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

يجب ان يتم منح المستخدم الدور المسؤول العام: [تعيين الدور إلى المستخدمين](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

قم بنشر هذا المستخدم باستخدام نهج RBAC: [منح حق الوصول إلى الفوترة](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**المستندات المستحسنة**

-   [لا يمكنني تسجيل الدخول لأداره اشتراكك في Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)