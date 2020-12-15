---
title: الجهاز في الحالة "معلق"
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/11/2020
ms.locfileid: "49676805"
---
# <a name="device-in-pending-state"></a>الجهاز في الحالة "معلق"

**متطلب**

1. إذا كنت تقوم باعداد تسجيلات الاجهزه للمرة الاولي ، فالرجاء التاكد من انك قمت بمراجعه [مقدمه حول أداره الاجهزه في Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) التي سترشدك علي كيفيه الحصول علي الاجهزه ضمن عنصر التحكم في azure AD.
2. إذا كنت تقوم بتسجيل الاجهزه في Azure AD مباشره وقامت بانتسابها في Intune ، ستحتاج إلى التاكد من انك قمت [بتكوين Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ولديك [الترخيص](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) في المكان أولا.
3. تاكد من انك مخول بتنفيذ العمليات في Azure AD والإعلان المحلي. يمكن للمسؤول العام فقط في Azure AD أداره إعدادات تسجيلات الاجهزه. بالاضافه إلى ذلك ، إذا كنت تقوم باعداد التسجيلات التلقائية في Active Directory المحلي ، ستحتاج إلى ان تكون مسؤولا ل Active directory و AD FS (إذا كان ذلك ممكنا).

تحتاج عمليه التسجيل المختلط في Azure AD join إلى الاجهزه التي يجب ان تكون علي شبكه الشركة. كما يعمل أيضا عبر الشبكات الظاهرية ، ولكن هناك بعض الكافيتس. لقد سمعنا العملاء الذين يحتاجون إلى مساعده في استكشاف الأخطاء المختلطة لعمليه التسجيل في Azure AD join ضمن ظروف العمل البعيدة.

**بيئة المصادقة السحابية (باستخدام المزامنة الخاصة بتجزئه كلمه مرور Azure AD أو المصادقة التمريري)**

يعرف تدفق التسجيل هذا أيضا "الصلة بالمزامنة".

فيما يلي تصنيف تفصيلي لما يحدث اثناء عمليه التسجيل:

1. سجل نقطه اتصال خدمه اكتشاف Windows 10 (سكب) عندما يقوم المستخدم بتسجيل الدخول إلى الجهاز.

    1. يحاول الجهاز أولا استرداد معلومات المستاجر من جانب العميل سكب في التسجيل [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. لمزيد من المعلومات ، راجع [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. إذا فشلت هذه العملية ، سيتصل الجهاز بخدمه Active Directory المحلية للحصول علي معلومات المستاجر من سكب. للتحقق من السكب ، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > نوصي بتمكين سكب في Active Directory واستخدام سكب من جانب العميل للتحقق من صحة مبدئي.

2. يحاول نظام التشغيل Windows 10 التواصل مع Azure AD تحت سياق النظام للمصادقة علي نفسه مقابل Azure AD.

    يمكنك التحقق مما إذا كان بإمكان الجهاز الوصول إلى موارد Microsoft ضمن حساب النظام باستخدام [البرنامج النصي لاتصال تسجيل جهاز الاختبار](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. يقوم Windows 10 بإنشاء شهادة موقعه ذاتيا وتخزينها ضمن كائن الكمبيوتر في Active Directory المحلي. يتطلب ذلك ان يتم الاطلاع علي الخطوط الخاصة بالمجال.

4. كائن الجهاز الذي تمت مزامنة الشهادة معه في Azure AD عبر Azure AD Connect. دوره المزامنة كل 30 دقيقه بشكل افتراضي ، ولكنها تعتمد علي تكوين Azure AD Connect. لمزيد من المعلومات ، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. في هذه المرحلة ، يجب ان تكون قادرا علي رؤية جهاز الموضوع في الحالة "**معلق**" ضمن "الجهاز النصليه في Azure Portal".

6. عند تسجيل دخول المستخدم التالي إلى Windows 10 ، سيتم إكمال التسجيل.

    > [!NOTE]
    > إذا كنت تستخدم VPN وقامت بتسجيل الدخول ، سيؤدي ذلك إلى إنهاء اتصال المجال ، يمكنك تشغيل التسجيل يدويا. لتنفيذ الإجراءات التالية:
    >
    > `dsregcmd /join`الإصدار المحلي لمطالبه المسؤول أو عن بعد عبر بسيكسيك إلى الكمبيوتر الشخصي.
    >
    > على سبيل المثال: `PsExec -s \\win10client01 cmd, dsregcmd /join`

للاطلاع علي المشاكل الشائعة في تسجيل جهاز Azure Active directory ، راجع [الاسئله المتداولة حول الاجهزه](https://docs.microsoft.com/azure/active-directory/devices/faq).
