---
title: الشروط المفقودة من متجر مصطلحات SharePoint عبر الإنترنت
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762035"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="38e74-102">تمكين تشفير Bitlocker مع إينتوني</span><span class="sxs-lookup"><span data-stu-id="38e74-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="38e74-103">يمكن استخدام نهج حماية نقطة النهاية إينتوني لتكوين إعدادات تشفير Boitlocker لأجهزة Windows كما هو موضح في : إعدادات Windows10 (والأحدث) لحماية الأجهزة باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="38e74-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="38e74-104">يجب أن تدرك أن العديد من الأجهزة الأحدث التي تعمل بنظام التشغيل Windows 10 تدعم تشفير bitlocker التلقائي الذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="38e74-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="38e74-105">قد يؤثر هذا على تطبيق النهج إذا تم تكوين إعدادات غير افتراضية.</span><span class="sxs-lookup"><span data-stu-id="38e74-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="38e74-106">راجع الأسئلة المتداولة لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="38e74-106">See FAQ for more detail.</span></span>


<span data-ttu-id="38e74-107">الأسئلة  المتداولة س: ما هي إصدارات تشفير جهاز دعم Windows باستخدام نهج حماية نقطة النهاية؟</span><span class="sxs-lookup"><span data-stu-id="38e74-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="38e74-108"> ج: يتم تطبيق الإعدادات في "نهج حماية نقطة النهاية إينتوني" باستخدام CSP Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="38e74-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="38e74-109">لا تدعم كافة الإصدارات ولا بنيات Windows CSP Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="38e74-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="38e74-110">في هذا الوقت إصدارات ويندوز: المؤسسة; يتم دعم التعليم، والمحمول، والمؤسسات المتنقلة والمهنية (من بناء 1809 فصاعدا).</span><span class="sxs-lookup"><span data-stu-id="38e74-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="38e74-111">س: إذا تم تشفير جهاز بالفعل باستخدام Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل لأسلوب التشفير وقوة التشفير (XTS-AES-128) سيتم تطبيق نهج مع إعدادات مختلفة تلقائيا ً بتشغيل إعادة تشفير محرك الأقراص مع الإعدادات الجديدة؟</span><span class="sxs-lookup"><span data-stu-id="38e74-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="38e74-112">أ: لا.</span><span class="sxs-lookup"><span data-stu-id="38e74-112">A: No.</span></span> <span data-ttu-id="38e74-113">لتطبيق إعدادات التشفير الجديدة يجب أولاً فك تشفير محرك الأقراص.</span><span class="sxs-lookup"><span data-stu-id="38e74-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="38e74-114">ملاحظة بالنسبة للأجهزة التي يتم تسجيلها مع الطيار الآلي لا يتم تشغيل التشفير التلقائي الذي قد يحدث أثناء OOBE حتى يتم تقييم نهج Intune الذي يسمح الإعدادات المستندة إلى النهج ليتم استخدامها بدلاً من افتراضيات نظام التشغيل</span><span class="sxs-lookup"><span data-stu-id="38e74-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="38e74-115">س إذا تم تشفير جهاز نتيجة لتطبيق نهج Intune سيتم فك تشفيره عند إزالة هذا النهج؟</span><span class="sxs-lookup"><span data-stu-id="38e74-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="38e74-116">A: إزالة النهج المتعلقة بالتشفير لا يؤدي إلى فك تشفير محركات الأقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="38e74-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="38e74-117">س: لماذا يظهر نهج التوافق في التوليف أن جهازي لا يحتوي على "تمكين Bitlocker" ولكنه كذلك؟</span><span class="sxs-lookup"><span data-stu-id="38e74-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="38e74-118">ج: يستخدم الإعداد "تمكين Bitlocker" في نهج التوافق إينتوني عميل شهادة صحة جهاز Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="38e74-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="38e74-119">يقيس هذا العميل حالة الجهاز فقط في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="38e74-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="38e74-120">حتى إذا لم يتم إعادة تمهيد جهاز منذ اكتمال تشفير bitlocker خدمة عميل DHA لن تقرير bitlocker كنشط.</span><span class="sxs-lookup"><span data-stu-id="38e74-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>