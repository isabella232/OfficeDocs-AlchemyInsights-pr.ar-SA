---
title: استكشاف مشكله برت وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573291"
---
# <a name="troubleshoot-prt-issue"></a>استكشاف مشكله برت وإصلاحها

لكي تكتمل عمليه المصادقة علي اي جهاز ، يجب ان يكون مسجلا بالبالكامل وفي حاله جيده ويمكنه الحصول علي رمز تحديث أساسي (برت).

تحتاج عمليه التسجيل المختلط في Azure AD join إلى الاجهزه التي يجب ان تكون علي شبكه الشركة. كما يعمل أيضا عبر الشبكات الظاهرية ، ولكن هناك بعض الكافياتس. لقد سمعنا العملاء الذين يحتاجون إلى مساعده في استكشاف عمليه التسجيل المختلطة في Azure AD join وإصلاحها ببموجب ظروف العمل عن بعد. اليك تصنيف تفصيلي لما يحدث "ضمن غطاء" اثناء عمليه التسجيل.

**بيئة المصادقة السحابية (باستخدام المزامنة الخاصة بتجزئه كلمه مرور Azure AD أو المصادقة التمريري)**

يعرف تدفق التسجيل هذا أيضا "الصلة بالمزامنة".

1. يكتشف Windows 10 سجل سكب عند تسجيل دخول المستخدم إلى الجهاز.
    1. يحاول الجهاز أولا استرداد معلومات المستاجر من جانب العميل سكب في التسجيل [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. لمزيد من المعلومات ، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. إذا فشلت هذه العملية ، سيتصل الجهاز بخدمه Active Directory المحلية (AD) للحصول علي معلومات المستاجر من نقطه اتصال الخدمة (سكب). للتحقق من السكب ، يرجى الرجوع إلى هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> نوصي بتمكين سكب في الإعلان واستخدام سكب من جانب العميل للتحقق من صحة مبدئي.

2. يحاول نظام التشغيل Windows 10 التواصل مع Azure AD تحت سياق النظام للمصادقة علي نفسه مقابل Azure AD. يمكنك التحقق مما إذا كان بإمكان الجهاز الوصول إلى موارد Microsoft ضمن حساب النظام باستخدام البرنامج النصي لاتصال تسجيل جهاز الاختبار.

3. ينشئ Windows 10 شهادة موقعه ذاتيا ويخزنها ضمن كائن الكمبيوتر في الإعلان المحلي. يتطلب ذلك ان يتم الاطلاع علي الخطوط الخاصة بالمجال.

4. تتم مزامنة كائن الجهاز الذي تمت الشهادة معه في Azure AD عبر Azure AD Connect. دوره المزامنة كل 30 دقيقه بشكل افتراضي ، ولكنها تعتمد علي تكوين Azure AD Connect. لمزيد من المعلومات ، يرجى الرجوع إلى هذا [المستند](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. في هذه المرحلة ، يجب ان تكون قادرا علي رؤية جهاز الموضوع في الحالة "معلق" ضمن "الجهاز النصليه في Azure Portal".

6. عند تسجيل دخول المستخدم التالي إلى Windows 10 ، سيتم إكمال التسجيل. 

> [!NOTE]
> إذا كنت تستخدم VPN وكانت عمليه تسجيل الدخول إلى التسجيل الخاص بك تقوم بإنهاء اتصال المجال ، فيمكنك تشغيل التسجيل يدويا:
 1. إصدار دسريجكمد/join محليا في مطالبه المسؤول أو عن بعد عبر بسيكسيك إلى الكمبيوتر الشخصي. علي سبيل المثال ، بسيكسيك \\ win10client01 cmd ، دسريجكمد/الصلة

 2. للحصول علي مزيد من التفاصيل حول مشاكل الصلة المختلطة ، راجع [مشكله استكشاف الأخطاء وإصلاحها](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
