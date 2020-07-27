---
title: تجاوز قفل التنشيط على أجهزة iOS الخاضعة للإشراف مع Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423307"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="3fdcb-102">تجاوز قفل التنشيط على أجهزة iOS الخاضعة للإشراف مع Intune</span><span class="sxs-lookup"><span data-stu-id="3fdcb-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="3fdcb-103">القدرة على تجاوز تأمين التنشيط على أجهزة iOS يجعل من السهل استرداد من السيناريو حيث يقوم المستخدم بتمكين تأمين التنشيط على جهاز الشركة، ثم يترك الشركة.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="3fdcb-104">المتطلبات المسبقة لتجاوز قفل التنشيط تشمل:</span><span class="sxs-lookup"><span data-stu-id="3fdcb-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="3fdcb-105">الجهاز هو أن "تحت إشراف".</span><span class="sxs-lookup"><span data-stu-id="3fdcb-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="3fdcb-106">يتم تمكين تأمين التنشيط بنجاح باستخدام سياسة تقييد جهاز iOS في Intune.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="3fdcb-107">بالإضافة إلى ذلك، عند تجاوز تأمين التنشيط، يجب عليك:</span><span class="sxs-lookup"><span data-stu-id="3fdcb-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="3fdcb-108">تمتلك فعليا الجهاز الذي يجري مسحها.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="3fdcb-109">نسخ التعليمات البرمجية قبل إصدار المسح.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="3fdcb-110">**ملاحظة:** رمز المسح غير حساس لحالة الأحرف، لذا لا تكون الأحرف "-" مطلوبة.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="3fdcb-111">للحصول على التفاصيل، راجع [تجاوز قفل التنشيط على أجهزة iOS الخاضعة للإشراف مع Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="3fdcb-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="3fdcb-112">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="3fdcb-112">**FAQ**</span></span>

<span data-ttu-id="3fdcb-113">س: **أصدرت إجراءً عن بعد لإزالة بيانات الشركة من جهاز، والآن هو عالق في حالة معلقة.**</span><span class="sxs-lookup"><span data-stu-id="3fdcb-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="3fdcb-114">A: لكي يتم إكمال إجراء عن بعد بنجاح، يجب أن يكون الجهاز المستهدف متصلاً و سليمًا.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="3fdcb-115">في الحالات التالية، يبقى الإجراء عن بعد في حالة معلقة لمدة 30 يوماً أو حتى الجهاز يعترف الأمر عند الجهاز:</span><span class="sxs-lookup"><span data-stu-id="3fdcb-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="3fdcb-116">ليس لديه اتصال.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-116">Does not have connectivity.</span></span>
- <span data-ttu-id="3fdcb-117">يفقد حالته الإدارية مع Intune.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="3fdcb-118">إذا كنت تعتقد أن الجهاز لم يعد يقوم بتسجيل الدخول، وأنه لن يزيل بيانات الشركة، فحدد حذف.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="3fdcb-119">يؤدي الحذف إلى إزالة سجل الجهاز بحيث لا يظهر في قائمة الأجهزة Intune.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="3fdcb-120">لكي يصبح الجهاز نشطًا مرة أخرى، يجب أن يعيد المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="3fdcb-121">س: **لماذا لا تتوفر بعض الإجراءات عن بعد لاستخدامها؟**</span><span class="sxs-lookup"><span data-stu-id="3fdcb-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="3fdcb-122">A: ليست كل الأنظمة الأساسية تدعم كافة إجراءات الجهاز البعيد.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="3fdcb-123">الإجراءات التالية عن بعد هي النظام الأساسي الخاصة.</span><span class="sxs-lookup"><span data-stu-id="3fdcb-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="3fdcb-124">تجاوز قفل التنشيط (iOS فقط)</span><span class="sxs-lookup"><span data-stu-id="3fdcb-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="3fdcb-125">بداية جديدة (ويندوز فقط)</span><span class="sxs-lookup"><span data-stu-id="3fdcb-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="3fdcb-126">وضع المفقودة (دائرة الرقابة الداخلية فقط)</span><span class="sxs-lookup"><span data-stu-id="3fdcb-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="3fdcb-127">تحديد موقع الجهاز (iOS فقط)</span><span class="sxs-lookup"><span data-stu-id="3fdcb-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="3fdcb-128">إعادة التشغيل (ويندوز فقط)</span><span class="sxs-lookup"><span data-stu-id="3fdcb-128">Restart (Windows only)</span></span>

<span data-ttu-id="3fdcb-129">لمزيد من التفاصيل حول كل إجراء، راجع [الإجراءات المتوفرة للجهاز](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="3fdcb-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>