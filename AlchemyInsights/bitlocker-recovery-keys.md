---
title: مفاتيح استرداد Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820273"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="59fb8-102">الوصول إلى مفاتيح استرداد Bitlocker</span><span class="sxs-lookup"><span data-stu-id="59fb8-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="59fb8-103">عند تكوين إعدادات Bitlocker نهج حماية نقطة نهاية Intune، من الممكن تحديد ما إذا كان يجب تخزين معلومات استرداد Bitlocker في Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59fb8-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="59fb8-104">إذا تم تكوين هذا الإعداد، يجب أن تكون بيانات الاسترداد المخزنة مرئية لمسؤول Intune كجزء من بيانات سجل الجهاز في شفرة أجهزة Intune باستخدام طريقتين:</span><span class="sxs-lookup"><span data-stu-id="59fb8-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="59fb8-105">الأجهزة - أجهزة Azure AD -> "الجهاز" أو الأجهزة -> جميع الأجهزة -> "الجهاز" -> الاسترداد</span><span class="sxs-lookup"><span data-stu-id="59fb8-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="59fb8-106">بدلا من ذلك، إذا كان هناك وصول إداري إلى الجهاز نفسه، يمكن رؤية مفتاح الاسترداد (كلمة المرور) عن طريق تشغيل الأمر التالي من موجه أوامر مرتفع:</span><span class="sxs-lookup"><span data-stu-id="59fb8-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="59fb8-107">إذا كان الجهاز مشفرا قبل التسجيل في Intune، فقد يكون مفتاح الاسترداد مقترن ب "حساب Microsoft" (MSA) المستخدم في تسجيل الدخول إلى الجهاز أثناء عملية OOBE.</span><span class="sxs-lookup"><span data-stu-id="59fb8-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="59fb8-108">إذا كان الأمر كذلك، يجب أن يظهر الوصول إلى MSA ثم تسجيل الدخول باستخدامه الأجهزة التي تم تخزين مفاتيح  https://onedrive.live.com/recoverykey الاسترداد لها.</span><span class="sxs-lookup"><span data-stu-id="59fb8-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="59fb8-109">إذا تم تشفير الجهاز نتيجة التكوين من خلال نهج المجموعة المستند إلى المجال، فقد يتم تخزين معلومات الاسترداد في Active Directory المحلية.</span><span class="sxs-lookup"><span data-stu-id="59fb8-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="59fb8-110">إذا قمت بتكوين نهج حماية نقطة النهاية لتخزين مفتاح الاسترداد في Azure Active Directory ولكن لم يتم تحميل مفتاح جهاز معين، يمكنك تشغيل التحميل عن طريق تدوير مفتاح الاسترداد لهذا الجهاز من وحدة تحكم MEM.</span><span class="sxs-lookup"><span data-stu-id="59fb8-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="59fb8-111">للحصول على التفاصيل، راجع [تدوير مفاتيح استرداد BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="59fb8-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

