---
title: تحديد موقع أجهزه iOS المفقودة باستخدام Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675142"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="976be-102">تحديد موقع أجهزه iOS المفقودة باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="976be-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="976be-103">يسمح تمكين الوضع المفقود علي جهاز iOS للمسؤول بالحصول علي رسالة ورقم هاتف الاتصال المعروض علي شاشه التامين.</span><span class="sxs-lookup"><span data-stu-id="976be-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="976be-104">بعد تمكين الوضع المفقود ، يمكن للمسؤول استخدام اجراء تحديد الجهاز لتحديد الموقع الفعلي للجهاز.</span><span class="sxs-lookup"><span data-stu-id="976be-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="976be-105">يعمل اجراء الجهاز في Intune مع أجهزه iOS لإظهار موقع جهاز معين علي خريطة.</span><span class="sxs-lookup"><span data-stu-id="976be-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="976be-106">يتطلب استخدام هذا الاجراء ان يكون جهاز iOS في:</span><span class="sxs-lookup"><span data-stu-id="976be-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="976be-107">وضع سوبيرفيسيد</span><span class="sxs-lookup"><span data-stu-id="976be-107">Supervised mode</span></span>
- <span data-ttu-id="976be-108">وضع الفقدان</span><span class="sxs-lookup"><span data-stu-id="976be-108">Lost mode</span></span>

<span data-ttu-id="976be-109">للحصول علي مزيد من المعلومات ، راجع [تمكين الوضع الخاسر علي الاجهزه التي تعمل بنظام التشغيل ios/إيبادوس مع Intune](https://docs.microsoft.com/intune/device-lost-mode) [وتحديد موقع الاجهزه المفقودة أو التي تعمل بنظام ios/إيبادوس باستخدام intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="976be-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="976be-110">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="976be-110">**FAQ**</span></span>

<span data-ttu-id="976be-111">س: لقد قمت بإصدار اجراء عن بعد لأزاله بيانات الشركة من جهاز ، والآن عالقه بحاله معلقه.</span><span class="sxs-lookup"><span data-stu-id="976be-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="976be-112">ج: لإكمال اجراء بعيد بنجاح ، يجب ان يكون الجهاز المستهدف متصلا وسليما.</span><span class="sxs-lookup"><span data-stu-id="976be-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="976be-113">في الحالات التالية ، يبقي الاجراء البعيد في حاله معلقه لمده 30 يوما ، أو حتى يقر الجهاز بالأمر:</span><span class="sxs-lookup"><span data-stu-id="976be-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="976be-114">عندما لا يكون لدي الجهاز اتصال</span><span class="sxs-lookup"><span data-stu-id="976be-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="976be-115">عندما يفقد الجهاز حاله الاداره الخاصة به مع Intune</span><span class="sxs-lookup"><span data-stu-id="976be-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="976be-116">إذا كنت تعتقد ان الجهاز لم يعد قيد الإيداع ، ولم يتمكن من أزاله بيانات الشركة ، فحدد حذف.</span><span class="sxs-lookup"><span data-stu-id="976be-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="976be-117">يؤدي الحذف إلى أزاله سجل الجهاز بحيث لا يظهر في قائمه Intune من الاجهزه.</span><span class="sxs-lookup"><span data-stu-id="976be-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="976be-118">إذا أصبح الجهاز نشطا مره أخرى ، سيضطر المستخدم إلى أعاده تسجيله.</span><span class="sxs-lookup"><span data-stu-id="976be-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="976be-119">س: لماذا لا تتوفر إجراءات معينه عن بعد لاستخدامها ؟</span><span class="sxs-lookup"><span data-stu-id="976be-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="976be-120">ج: لا تعتمد كل الانظمه الاساسيه كل إجراءات الجهاز البعيد.</span><span class="sxs-lookup"><span data-stu-id="976be-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="976be-121">الإجراءات البعيدة التالية خاصه بالنظام الأساسي ، بحيث تكون متوفرة فقط للانظمه الاساسيه التي تمت الاشاره اليها.</span><span class="sxs-lookup"><span data-stu-id="976be-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="976be-122">تجاوز تامين التنشيط (iOS فقط)</span><span class="sxs-lookup"><span data-stu-id="976be-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="976be-123">بدء التشغيل الجديد (Windows فقط)</span><span class="sxs-lookup"><span data-stu-id="976be-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="976be-124">وضع الفقدان (iOS فقط)</span><span class="sxs-lookup"><span data-stu-id="976be-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="976be-125">تحديد موقع الجهاز (iOS فقط)</span><span class="sxs-lookup"><span data-stu-id="976be-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="976be-126">أعاده التشغيل (Windows فقط)</span><span class="sxs-lookup"><span data-stu-id="976be-126">Restart (Windows only)</span></span>

<span data-ttu-id="976be-127">للحصول علي مزيد من التفاصيل حول كل اجراء ، راجع [إجراءات الجهاز المتوفرة](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="976be-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>