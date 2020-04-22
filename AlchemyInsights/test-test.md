---
title: المصطلحات المفقودة من SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766840"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="1b118-102">تمكين تشفير Bitlocker مع Intune</span><span class="sxs-lookup"><span data-stu-id="1b118-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="1b118-103">يمكن استخدام نهج حماية نقطة النهاية Intune لتكوين إعدادات تشفير Boitlocker لأجهزة Windows كما هو موضح في إعدادات Windows10 (والأحدث) لحماية الأجهزة التي تستخدم Intune</span><span class="sxs-lookup"><span data-stu-id="1b118-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="1b118-104">يجب أن تدرك أن العديد من الأجهزة الأحدث التي تعمل بنظام التشغيل Windows 10 تدعم تشفير bitlocker التلقائي الذي يتم تشغيله دون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="1b118-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="1b118-105">قد يؤثر هذا على تطبيق النهج إذا تم تكوين الإعدادات غير الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="1b118-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="1b118-106">راجع الأسئلة الشائعة لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="1b118-106">See FAQ for more detail.</span></span>


<span data-ttu-id="1b118-107">الأسئلة  الشائعة س: ما هي إصدارات تشفير جهاز دعم Windows باستخدام نهج حماية نقطة النهاية؟</span><span class="sxs-lookup"><span data-stu-id="1b118-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="1b118-108"> ج: يتم تنفيذ الإعدادات في نهج حماية نقطة النهاية Intune باستخدام CSP Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="1b118-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="1b118-109">ليس كل الإصدارات ولا يبني من ويندوز دعم CSP Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="1b118-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="1b118-110">في هذا الوقت إصدارات ويندوز: المؤسسة; يتم دعم التعليم والجوال والمشاريع المتنقلة والمهنية (من بناء 1809 فصاعدا).</span><span class="sxs-lookup"><span data-stu-id="1b118-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="1b118-111">س: إذا كان الجهاز مشفرًا بالفعل باستخدام Bitlocker باستخدام إعدادات OS الافتراضية لطريقة التشفير وقوة التشفير (XTS-AES-128) فسيقوم بتطبيق نهج مع إعدادات مختلفة تلقائيًا يؤدي إلى إعادة تشفير محرك الأقراص باستخدام الإعدادات الجديدة؟</span><span class="sxs-lookup"><span data-stu-id="1b118-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="1b118-112">ج: لا.</span><span class="sxs-lookup"><span data-stu-id="1b118-112">A: No.</span></span> <span data-ttu-id="1b118-113">من أجل تطبيق إعدادات التشفير الجديدة يجب أولاً فك تشفير محرك الأقراص.</span><span class="sxs-lookup"><span data-stu-id="1b118-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="1b118-114">ملاحظة بالنسبة للأجهزة التي يتم تسجيلها مع الطيار الآلي لا يتم تشغيل التشفير التلقائي الذي سيحدث أثناء OOBE حتى يتم تقييم نهج Intune الذي يسمح باستخدام الإعدادات المستندة إلى النهج بدلاً من إعدادات OS الافتراضية</span><span class="sxs-lookup"><span data-stu-id="1b118-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="1b118-115">س: إذا تم تشفير جهاز نتيجة لتطبيق نهج Intune هل سيتم فك تشفيره عند إزالة هذا النهج؟</span><span class="sxs-lookup"><span data-stu-id="1b118-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="1b118-116">ج: إزالة نهج التشفير ذات الصلة لا يؤدي إلى فك تشفير محركات الأقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="1b118-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="1b118-117">س: لماذا تظهر سياسة التوافق في أن جهازي لا يحتوي على "Bitlocker تمكين" ولكنه كذلك؟</span><span class="sxs-lookup"><span data-stu-id="1b118-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="1b118-118">ج: يستخدم الإعداد "تمكين Bitlocker" في نهج التوافق في تناغم عميل شهادة صحة جهاز Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="1b118-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="1b118-119">يقيس هذا العميل حالة الجهاز فقط في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="1b118-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="1b118-120">حتى إذا لم يتم إعادة تمهيد جهاز منذ اكتمال تشفير bitlocker خدمة العملاء DHA لن تقرير bitlocker كما يجري نشطة.</span><span class="sxs-lookup"><span data-stu-id="1b118-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>