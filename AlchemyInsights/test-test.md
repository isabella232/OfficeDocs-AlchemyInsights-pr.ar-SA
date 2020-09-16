---
title: الشروط المفقودة من مخزن مصطلحات SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750438"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="78dfc-102">تمكين تشفير Bitlocker باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="78dfc-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="78dfc-103">يمكن استخدام نهج حماية النقاط النهائية في Intune لتكوين إعدادات تشفير بويتلوكير للاجهزه التي تعمل بنظام التشغيل Windows كما هو موضح في: Windows10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="78dfc-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="78dfc-104">يجب ان تكون علي علم بان العديد من الاجهزه الجديدة التي تقوم بتشغيل Windows 10 تدعم تشفير bitlocker التلقائي الذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="78dfc-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="78dfc-105">قد يؤثر هذا علي تطبيق النهج إذا لم يتم تكوين الإعدادات الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="78dfc-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="78dfc-106">راجع الاسئله المتداولة لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="78dfc-106">See FAQ for more detail.</span></span>


<span data-ttu-id="78dfc-107"> الاسئله المتداولة Q: ما هي إصدارات تشفير جهاز دعم Windows التي تستخدم نهج حماية نقطه النهاية ؟</span><span class="sxs-lookup"><span data-stu-id="78dfc-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="78dfc-108"> ج: يتم تطبيق الإعدادات الموجودة في نهج حماية نقطه نهاية Intune باستخدام Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="78dfc-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="78dfc-109">ليست كل الإصدارات أو الإصدارات من Windows تدعم Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="78dfc-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="78dfc-110">في هذا الوقت ، إصدارات Windows: Enterprise ؛ يتم دعم التعليم والمحمول والمؤسسة المحمولة والمهنية (من النسخة 1809 فما بعد).</span><span class="sxs-lookup"><span data-stu-id="78dfc-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="78dfc-111">س: إذا تم بالفعل تشفير جهاز بواسطة Bitlocker باستخدام "الإعدادات الافتراضية لنظام التشغيل" لأسلوب التشفير وقوه التشفير (إكستس-AES-128) ، سيتم تطبيق نهج باستخدام إعدادات مختلفه تلقائيا بتشغيل الإعدادات الجديدة ؟</span><span class="sxs-lookup"><span data-stu-id="78dfc-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="78dfc-112">ج: لا.</span><span class="sxs-lookup"><span data-stu-id="78dfc-112">A: No.</span></span> <span data-ttu-id="78dfc-113">لتطبيق إعدادات التشفير الجديدة ، يجب ان يكون محرك الاقراص مشفرا أولا.</span><span class="sxs-lookup"><span data-stu-id="78dfc-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="78dfc-114">ملاحظه للاجهزه التي يتم تسجيلها باستخدام Autopilot لا يتم تشغيل التشفير التلقائي الذي سيحدث اثناء OOBE حتى يتم تقييم نهج Intune الذي يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الافتراضيات لنظام التشغيل.</span><span class="sxs-lookup"><span data-stu-id="78dfc-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="78dfc-115">س إذا تم تشفير جهاز كنتيجة لتطبيق النهج Intune سيتم فك تشفيره عند أزاله هذا النهج ؟</span><span class="sxs-lookup"><span data-stu-id="78dfc-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="78dfc-116">ج: لا تؤدي أزاله نهج التشفير المرتبط إلى فك تشفير محركات الاقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="78dfc-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="78dfc-117">س: لماذا يعرض نهج التوافق ل intune عدم وجود "تم تمكين Bitlocker" علي الجهاز ولكنه ؟</span><span class="sxs-lookup"><span data-stu-id="78dfc-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="78dfc-118">ج: يستخدم الاعداد "تم تمكين Bitlocker" في نهج التوافق ل intune لعميل مصادقه الحماية الخاصة بجهاز Windows (دها).</span><span class="sxs-lookup"><span data-stu-id="78dfc-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="78dfc-119">يقيس هذا العميل حاله الجهاز فقط في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="78dfc-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="78dfc-120">إذا لم يتم أعاده تشغيل الجهاز منذ إكمال تشفير bitlocker ، فلن تقوم خدمه عميل دا بالإبلاغ عن bitlocker كما هي نشطه.</span><span class="sxs-lookup"><span data-stu-id="78dfc-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>