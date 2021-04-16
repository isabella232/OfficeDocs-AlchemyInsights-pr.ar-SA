---
title: استخدام خيار إلغاء تأمين بصمات الأصابع في Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796664"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="7231d-102">استخدام خيار إلغاء تأمين بصمات الأصابع في Windows 10</span><span class="sxs-lookup"><span data-stu-id="7231d-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="7231d-103">**تمكين بصمة الإصبع في Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="7231d-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="7231d-104">لإلغاء تأمين Windows 10 باستخدام بصمة الإصبع، تحتاج إلى إعداد بصمة الإصبع في Windows Hello بإضافة (السماح ل Windows بالتعرف على ذلك) بإصبع واحد على الأقل.</span><span class="sxs-lookup"><span data-stu-id="7231d-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="7231d-105">انتقل إلى **إعدادات > الحسابات > خيارات تسجيل الدخول** (أو انقر [هنا).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="7231d-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="7231d-106">سيتم إدراج خيارات تسجيل الدخول المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="7231d-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="7231d-107">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="7231d-107">For example:</span></span>

    ![خيارات تسجيل الدخول.](media/sign-in-options.png)

2. <span data-ttu-id="7231d-109">انقر فوق أو اضغط **على بصمة الإصبع** في Windows Hello ، ثم انقر **فوق إعداد**.</span><span class="sxs-lookup"><span data-stu-id="7231d-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="7231d-110">في نافذة إعداد Windows Hello، انقر فوق **بدء استخدام**.</span><span class="sxs-lookup"><span data-stu-id="7231d-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="7231d-111">سيتم تنشيط مستشعر بصمات الأصابع، وستطلب منك وضع إصبعك على المستشعر:</span><span class="sxs-lookup"><span data-stu-id="7231d-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![مستشعر بصمات الأصابع.](media/fingerprint-sensor.png)

3. <span data-ttu-id="7231d-113">اتبع الإرشادات التي ستطالبك بمسح إصبعك بشكل متكرر.</span><span class="sxs-lookup"><span data-stu-id="7231d-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="7231d-114">عند الانتهاء من ذلك، سيكون لديك خيار إضافة أصابع أخرى قد ترغب في استخدامها في تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="7231d-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="7231d-115">في المرة التالية التي تقوم فيها تسجيل الدخول إلى Windows 10، سيكون لديك خيار استخدام بصمة الإصبع للقيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="7231d-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="7231d-116">**بصمة الإصبع في Windows Hello غير متوفرة كخيار تسجيل الدخول**</span><span class="sxs-lookup"><span data-stu-id="7231d-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="7231d-117">إذا لم يتم عرض بصمة الإصبع في Windows Hello كخيار في خيارات تسجيل الدخول، فهذا يعني أن Windows ليس على علم بأي قارئ بصمات أصابع/ماسح ضوئي مرفق بالكمبيوتر الشخصي، أو أن نهج النظام يمنع استخدامه (على سبيل المثال، إذا كان جهاز الكمبيوتر الخاص بك مدارا بواسطة مكان عملك). </span><span class="sxs-lookup"><span data-stu-id="7231d-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="7231d-118">لا استكشاف الأخطاء وإصلاحها:</span><span class="sxs-lookup"><span data-stu-id="7231d-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="7231d-119">حدد زر **البدء** في شريط المهام وابحث عن **إدارة الأجهزة**.</span><span class="sxs-lookup"><span data-stu-id="7231d-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="7231d-120">انقر فوق أو اضغط لفتح **إدارة الأجهزة**.</span><span class="sxs-lookup"><span data-stu-id="7231d-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="7231d-121">في "إدارة الأجهزة"، قم بتوسيع أجهزة المقاييس الحيوية بالنقر فوق الشفرة الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="7231d-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![أجهزة المقاييس الحيوية.](media/biometric-devices.png)

4. <span data-ttu-id="7231d-123">يجب إدراج الماسح الضوئي لبصمة الإصبع على أنه جهاز قياس حيوي، مثل الماسح الضوئي Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="7231d-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![أجهزة المقاييس الحيوية.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="7231d-125">إذا لم يظهر الماسح الضوئي لبصمة الإصبع، وكان الماسح الضوئي متكاملا في الكمبيوتر الشخصي، فاذهب إلى موقع الشركة المصنعة للكمبيوتر الشخصي على الويب.</span><span class="sxs-lookup"><span data-stu-id="7231d-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="7231d-126">في قسم الدعم التقني لنموذج الكمبيوتر الشخصي، ابحث عن برنامج تشغيل Windows 10 عن ماسح ضوئي يمكنك تثبيته.</span><span class="sxs-lookup"><span data-stu-id="7231d-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="7231d-127">إذا كان الماسح الضوئي منفصلا عن الكمبيوتر الشخصي (المرفق عبر USB)، فاذهب إلى موقع ويب الشركة المصنعة للماسح الضوئي للعثور على برنامج تشغيل جهاز Windows 10 وتثبيته لنموذج الماسح الضوئي لديك.</span><span class="sxs-lookup"><span data-stu-id="7231d-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
