---
title: يتم حظري بواسطة "الوصول الشرطي" مع جهاز انضم إلى المجال
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/20/2021
ms.locfileid: "51034869"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>يتم حظري بواسطة "الوصول الشرطي" مع جهاز انضم إلى المجال

**أدوات موصى بها بشدة**

أداة م استكشاف [الأخطاء وإصلاحها](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) لتسجيل الجهاز - الأداة التي تساعد في استكشاف مشاكل تسجيل الجهاز الأكثر شيوعا وإصلاحها.

[اختبار البرنامج النصي لاتصال](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) تسجيل الجهاز - البرنامج النصي الذي يساعد على ضمان وصول الجهاز إلى نقاط نهاية تسجيل الجهاز ضمن حساب النظام.

[برنامج نصي لتنظيف جهاز Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - البرنامج النصي الذي يمكنك من البحث عن الأجهزة التي لم يتم انتهاءها وإدارتها في بيئتك.

فيما يلي بعض الأسباب الشائعة وراء فشل الوصول الشرطي لجهاز انضم إلى مجال (Azure AD المختلط).

1. **لا يوجد Azure AD PRT** على الجهاز - يجب التأكد من أن الجهاز لديه رمز التحديث الأساسي ل Azure AD Token (PRT). لمزيد من المعلومات حول PRT، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

للتحقق مما إذا كان لديك Azure AD PRT، يمكنك تشغيل الأمر على الجهاز والتحقق مما إذا كانت `dsregcmd/status` "AzureAdPrt" تساوي "YES".

إذا كانت "AzureAdPrt" "NO"، فتحقق مما يلي:

- سواء كان لديك بيئة مضمنة مع **AD FS،** ولا يمكن الوصول إليها من الشبكات المنزلية الخاصة بالمستخدمين : في هذه الحالة، تأكد من إمكانية الوصول إلى نقاط النهاية "اسم المستخدم" من إكسترانت. إذا كان AD FS الخاص بك خلف VPN، فتأكد من اتصال المستخدمين ب VPN ثم إعادة تسجيل الدخول إلى الجهاز. لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **ما إذا كانت TPM** في الجهاز بها أخطاء وبالتالي يتعذر عليها مصادقة الجهاز : تحقق من "tpm.msc" لمعرفة ما إذا كانت حالة TPM هي "جاهز". إذا لم يكن الأمر كذلك، فدير الجهاز `dsregcmd/leave` واتركه ينضم مرة أخرى إلى Azure AD. بعد ذلك، حاول مرة أخرى. لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **أنت تستخدم موفر هوية** جهة خارجية، لا يدعم WS-Trust. كما هو موضح في مستنداتنا، لا يمكن للأجهزة المختلطة المنضمة إلى Azure AD العمل في هذه الحالة. الرجاء العمل مع موفر الهوية للحصول على الدعم.

2. يستخدم المستخدمون مستعرض Chrome بدون حسابات **Windows 10** أو ملحق Office لا يستخدم Chrome تلقائيا PRT على الأجهزة المنضمة إلى AAD أو المختلطة المنضمة إلى **AAD**: يؤدي ذلك إلى فشل أي من سياسات الوصول الشرطي المستندة إلى الجهاز، مع عرض رسالة الخطأ "جهاز غير مسجل". لاستخدام مستعرض Chrome بشكل صحيح، يجب تثبيت "حسابات Windows 10" أو "ملحق Office إلى مستعرض Chrome الخاص المستخدمين" عبر SCCM أو Intune. لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

إذا لم يكن من الممكن دفع الملحق عن بعد، قم بإعلام المستخدمين بتثبيت أحد الملحقات أعلاه يدويا للوصول إلى التطبيقات خلف الوصول الشرطي المستند إلى الجهاز. لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. كان الجهاز مختلطا بشكل صحيح انضم **Azure AD،** ولكن تم حذفه أو تعطيله عن طريق الخطأ، إما بسبب مزامنة التغييرات في Azure AD Connect أو من مدخل Azure : إذا حدث ذلك، لن يتم التعرف على كائن الجهاز على أنه جهاز منضم بالكامل على الرغم من أن حالة "AzureAdJoined" و"PRT" تظهر ك صالحة على الجهاز.

لإصلاح هذه المشكلة، يمكنك التشغيل على الأجهزة المتأثرة واتركها تنضم مجددا إلى `dsregcmd/leave` Azure AD. لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> إذا كانت أجهزتك تعمل على تحديث Windows 10، 1809، باستخدام VPN/وكيل السحابة وشاهدت مشاكل تتعلق ب "AzureAdPrt" (AzureAdPrt) أو أي تطبيق به مشكلة في SSO (outlook لا يتصل علبة البريد على الرغم من وجود PRT لديك)، فتأكد من وجود هذا التصحيح [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) أو التحديث التراكمي ل [أبريل KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) لمنع حالات فشل PRT على هذه الأجهزة.

















