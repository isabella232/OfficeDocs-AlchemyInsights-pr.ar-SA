---
title: تحديد مواقع أجهزة iOS المفقودة باستخدام Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438788"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="a9326-102">تحديد مواقع أجهزة iOS المفقودة باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="a9326-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="a9326-103">تمكين وضع المفقودة على جهاز دائرة الرقابة الداخلية يسمح للمسؤول أن يكون رسالة ورقم هاتف جهة الاتصال المعروضة على شاشة القفل.</span><span class="sxs-lookup"><span data-stu-id="a9326-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="a9326-104">بعد تمكين وضع المفقودة يمكن للمسؤول استخدام الإجراء تحديد موقع الجهاز لتحديد الموقع الفعلي للجهاز.</span><span class="sxs-lookup"><span data-stu-id="a9326-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="a9326-105">يعمل إجراء تحديد موقع الجهاز في Intune مع أجهزة iOS لعرض موقع جهاز معين على الخريطة.</span><span class="sxs-lookup"><span data-stu-id="a9326-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="a9326-106">يتطلب استخدام هذا الإجراء أن يكون جهاز iOS في:</span><span class="sxs-lookup"><span data-stu-id="a9326-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="a9326-107">الوضع الخاضع للإشراف</span><span class="sxs-lookup"><span data-stu-id="a9326-107">Supervised mode</span></span>
- <span data-ttu-id="a9326-108">وضع المفقود</span><span class="sxs-lookup"><span data-stu-id="a9326-108">Lost mode</span></span>

<span data-ttu-id="a9326-109">لمزيد من المعلومات، راجع [تمكين وضع المفقودة على أجهزة iOS/iPadOS مع Intune](https://docs.microsoft.com/intune/device-lost-mode) وتحديد [موقع أجهزة iOS/iPadOS المفقودة أو المسروقة مع Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="a9326-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="a9326-110">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="a9326-110">**FAQ**</span></span>

<span data-ttu-id="a9326-111">س: أصدرت إجراءً عن بعد لإزالة بيانات الشركة من جهاز، والآن هو عالق في حالة معلقة.</span><span class="sxs-lookup"><span data-stu-id="a9326-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="a9326-112">A: لكي يتم إكمال إجراء عن بعد بنجاح، يجب أن يكون الجهاز المستهدف متصلاً و سليمًا.</span><span class="sxs-lookup"><span data-stu-id="a9326-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="a9326-113">في الحالات التالية، يبقى الإجراء البعيد في حالة معلقة لمدة 30 يوماً أو حتى الجهاز يعترف الأمر:</span><span class="sxs-lookup"><span data-stu-id="a9326-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="a9326-114">عندما لا يكون الجهاز الاتصال</span><span class="sxs-lookup"><span data-stu-id="a9326-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="a9326-115">عندما يفقد الجهاز حالته الإدارية مع Intune</span><span class="sxs-lookup"><span data-stu-id="a9326-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="a9326-116">إذا كنت تعتقد أن أحد الأجهزة لم يعد يقوم بتسجيل الدخول، وأنه لن يتمكن من إزالة بيانات الشركة، فحدد حذف.</span><span class="sxs-lookup"><span data-stu-id="a9326-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="a9326-117">يؤدي الحذف إلى إزالة سجل الجهاز بحيث لا يظهر في قائمة الأجهزة Intune.</span><span class="sxs-lookup"><span data-stu-id="a9326-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="a9326-118">إذا أصبح الجهاز نشطًا مرة أخرى، فسيضطر المستخدم إلى إعادة تسجيله.</span><span class="sxs-lookup"><span data-stu-id="a9326-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="a9326-119">س: لماذا لا تتوفر بعض الإجراءات عن بعد لاستخدامها؟</span><span class="sxs-lookup"><span data-stu-id="a9326-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="a9326-120">A: ليست كل الأنظمة الأساسية تدعم كافة إجراءات الجهاز البعيد.</span><span class="sxs-lookup"><span data-stu-id="a9326-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="a9326-121">الإجراءات التالية عن بعد هي النظام الأساسي الخاصة، حيث أنها متوفرة فقط للأنظمة الملاحظة.</span><span class="sxs-lookup"><span data-stu-id="a9326-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="a9326-122">تجاوز قفل التنشيط (iOS فقط)</span><span class="sxs-lookup"><span data-stu-id="a9326-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="a9326-123">بداية جديدة (ويندوز فقط)</span><span class="sxs-lookup"><span data-stu-id="a9326-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="a9326-124">وضع المفقودة (دائرة الرقابة الداخلية فقط)</span><span class="sxs-lookup"><span data-stu-id="a9326-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="a9326-125">تحديد موقع الجهاز (iOS فقط)</span><span class="sxs-lookup"><span data-stu-id="a9326-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="a9326-126">إعادة التشغيل (ويندوز فقط)</span><span class="sxs-lookup"><span data-stu-id="a9326-126">Restart (Windows only)</span></span>

<span data-ttu-id="a9326-127">لمزيد من التفاصيل حول كل إجراء، راجع [الإجراءات المتوفرة للجهاز](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="a9326-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>