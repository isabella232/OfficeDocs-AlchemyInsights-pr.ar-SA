---
title: يتم حظري بواسطة "الوصول الشرطي" مع جهاز متوافق
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019135"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>يتم حظري بواسطة "الوصول الشرطي" مع جهاز متوافق

**أدوات موصى بها بشدة**

- أداة م استكشاف [الأخطاء وإصلاحها](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) لتسجيل الجهاز - أداة شاملة تساعد على استكشاف مشاكل تسجيل الأجهزة الأكثر شيوعا وإصلاحها.
- [اختبار البرنامج النصي لاتصال](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) تسجيل الجهاز - أداة تستخدم للتأكد من أن الجهاز يمكنه الوصول إلى نقاط نهاية تسجيل الجهاز ضمن حساب النظام.
- [برنامج نصي لتنظيف جهاز Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - أداة تستخدم للبحث عن الأجهزة التي لا تعمل بشكل جيد وإدارتها في بيئتك.

فيما يلي بعض الأسباب الشائعة لفشل الوصول الشرطي لجهاز متوافق أو  سبب تلقي المستخدمين لرسالة لا يمكنك الوصول إليها من هنا أثناء طلب تسجيل الدخول إلى مورد المؤسسة.

1. **الجهاز غير في حالة جهاز مطلوب مع MDM:**

تحقق من أن الجهاز مسجل مع موفر MDM معتمد مثل Intune وضع *علامة عليه كمتوافق.* لمزيد من المعلومات حول Intune، راجع هذا [المستند](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). للحصول على فهم أفضل لتوافق الأجهزة و Intune، راجع استخدام نهج التوافق لتعيين قواعد للأجهزة التي [تديرها باستخدام Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). إذا كنت تواجه مشاكل في تسجيل جهاز باستخدام Intune، فاعثر على تفاصيل استكشاف الأخطاء وإصلاحها في تسجيل الجهاز وإصلاحها [في Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). لمزيد من دعم Intune، قم بإنشاء طلب دعم. للقيام بذلك، تفضل بزيارة [صفحة تعليمات ودعم Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **الجهاز غير منضم إلى شبكة المؤسسات**:

للوصول إلى موارد المؤسسة، يجب أن يكون الجهاز متصلا بشبكة المؤسسة، إما من خلال اتصال مباشر أو شبكة ظاهرية خاصة (VPN)، وأن يكون متصلا أيضا ب Azure Active Directory أو المحلي. للانضمام إلى جهاز عمل إلى شبكة المؤسسة، راجع الانضمام إلى جهاز العمل إلى [شبكة مؤسستك](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). لتسجيل جهاز شخصي/BYOD، راجع تسجيل جهازك [الشخصي على شبكة مؤسستك](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- للتحقق مما إذا كان الجهاز قد انضم إلى الشبكة، [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) يمكنك اتباع الخطوات الخاصة بالأجهزة المسجلة هنا أو أجهزة العمل [هنا.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) لنطاق المشكلة إلى اتصال شبكة المؤسسة، اتبع الإرشادات أدناه:

    1. سجل الدخول Windows باستخدام حساب العمل أو المدرسة، على سبيل المثال، alain@contoso.com.
    2. الاتصال إلى شبكة مؤسستك من خلال VPN أو DirectAccesss.
    3. بعد الاتصال، اضغط على مفتاح **Windows+L** لقفل جهازك.
    4. قم بإلغاء تأمين جهازك باستخدام حساب العمل أو المدرسة، ثم حاول الوصول إلى التطبيق أو الخدمة التي تسبب مشاكل مرة أخرى.

إذا رأيت رسالة الخطأ **لا** يمكنك الوصول إلى هناك من هنا مرة أخرى، فمن المرجح أن تكون المشكلة في مكان آخر.

3. **نظام التشغيل غير معتمد:**

تأكد من تشغيل إصدار معتمد من نظام التشغيل، بما في ذلك:

- **Windows العميل**: Windows 7 أو أي وقت لاحق

- **Windows Server**: Windows Server 2008 R2 أو أي وقت لاحق

- **macOS**: macOS X أو أي وقت لاحق

- **Android و iOS**: أحدث إصدار من أنظمة تشغيل الأجهزة المحمولة التي تعمل بنظامي التشغيل Android و iOS

4. **مستعرض ويب غير معتمد:**

الرجاء العثور على المستعرضات المعتمدة أدناه. بالنسبة إلى دعم Chrome Windows الإصدار 1703 أو الإصدارات الأحدث، يلزم Windows 10 الحسابات. بالنسبة إلى Edge 85+، يحتاج المستخدم إلى تسجيل الدخول لتمرير معلومات توافق الجهاز بشكل صحيح. لمزيد من التفاصيل، راجع [هنا](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge و Internet Explorer و Chrome
- **Windows 8 / 8.1**: Internet Explorer، Chrome
- **Windows 7**: Internet Explorer، Chrome
- **iOS**: Microsoft Edge، مستعرض Intune المدار، Safari
- **Android**: **Microsoft Edge**: مستعرض Intune المدار، Chrome
- **Windows Phone**: Microsoft Edge Internet Explorer
- **Windows Server 2019**: Microsoft Edge و Internet Explorer و Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome، Safari

يمكنك العثور على مزيد من المعلومات حول **الرسالة** لا يمكنك الوصول إلى هناك والخطوات المتعلقة استكشاف الأخطاء وإصلاحها [هنا](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
