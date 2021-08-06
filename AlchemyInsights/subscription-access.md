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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999227"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>تعذر تسجيل الدخول إلى Azure بسبب مشاكل المستعرض (توقف المستعرض، استمر في الدوران، لا يتم تحميله، إلخ.)

قد تكون متأثّر ب انقطاع التيار الكهربائي. الرجاء التحقق لمعرفة ما إذا كان هناك انقطاع جار: [حالة صحة Azure](https://status.azure.com/status/history/).

الرجاء تسجيل الخروج من كل جلسات Azure النشطة. ابدأ وضع مستعرض الويب الخاص أو وضع التصفح المتخفي.

يمكنك أيضا محاولة تحديث المستعرض واستخدام مستعرض آخر وحذف ملفات تعريف الارتباط ذاكرة التخزين المؤقت إذا لم تعمل أعلاه.

تعرف على المزيد: استكشاف [مشاكل تسجيل الدخول وإصلاحها](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**تعذر الوصول إلى الاشتراكات**

في مدخل [Azure،](https://portal.azure.com/)تأكد من تحديد دليل Azure الصحيح من الحساب في الجزء العلوي الأيمن.

في [مركز حساب Azure ،](https://account.windowsazure.com/Subscriptions)تأكد مما إذا كان الحساب المستخدم هو مسؤول الحساب.

تعرف على المزيد: استكشاف الأخطاء وإصلاحها لم يتم [العثور على أي اشتراكات](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**تعذر الوصول إلى محفوظات الفوترة**

يجب على مسؤول الحساب التأكد من إضافة المستخدم الذي يقوم بالوصول إلى معلومات الفوترة في دليل Azure Active كمستخدم ضيف: إضافة مستخدم جديد أو [حذفه.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

بعد ذلك، يجب أن يتم منح المستخدم دور المسؤول العام: [تعيين دور للمستخدمين](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

انشر ذلك، يمكن منح المستخدم حق الوصول إلى الفوترة باستخدام سياسات RBAC: [منح حق الوصول إلى الفوترة](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**المستندات الموصى بها**

-   [لا يمكنني تسجيل الدخول لإدارة اشتراكي في Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)