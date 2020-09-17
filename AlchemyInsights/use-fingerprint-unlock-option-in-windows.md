---
title: استخدام خيار إلغاء تامين بصمات الأصابع في Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795231"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="5913f-102">استخدام خيار إلغاء تامين بصمات الأصابع في Windows 10</span><span class="sxs-lookup"><span data-stu-id="5913f-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="5913f-103">**تمكين بصمات Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="5913f-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="5913f-104">للغاء تامين نظام التشغيل Windows 10 باستخدام بصمات الأصابع ، يجب اعداد بصمه الاصبع في Windows Hello عبر أضافه (السماح ل Windows بالتعرف علي التعرف عليه) علي الأقل باصبع واحد.</span><span class="sxs-lookup"><span data-stu-id="5913f-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="5913f-105">انتقل إلى **إعدادات > حسابات > خيارات تسجيل الدخول** (أو انقر [هنا](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="5913f-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="5913f-106">سيتم ادراج خيارات تسجيل الدخول المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="5913f-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="5913f-107">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="5913f-107">For example:</span></span>

    ![خيارات تسجيل الدخول.](media/sign-in-options.png)

2. <span data-ttu-id="5913f-109">انقر فوق **بصمات Windows Hello**أو اضغط عليها ، ثم **انقر فوق اعداد**.</span><span class="sxs-lookup"><span data-stu-id="5913f-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="5913f-110">في نافذه اعداد Windows Hello ، انقر فوق **بدء**الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="5913f-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="5913f-111">سيتم تنشيط مجس بصمات الأصابع ، ستتم مطالبتك بوضع اصبعك علي المجس:</span><span class="sxs-lookup"><span data-stu-id="5913f-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![مجس بصمات الأصابع.](media/fingerprint-sensor.png)

3. <span data-ttu-id="5913f-113">اتبع الإرشادات التي ستسالك عن تكرار التقاط بالاصبع.</span><span class="sxs-lookup"><span data-stu-id="5913f-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="5913f-114">عند الانتهاء من ذلك ، سيتوفر لديك خيار أضافه أصابع أخرى قد ترغب في استخدامها لتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="5913f-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="5913f-115">في المرة التالية التي تسجل فيها الدخول إلى Windows 10 ، سيتوفر لديك خيار استخدام بصمه الاصبع الخاصة بك للقيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="5913f-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="5913f-116">**لا تتوفر بصمات الأصابع في Windows Hello كخيار لتسجيل الدخول**</span><span class="sxs-lookup"><span data-stu-id="5913f-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="5913f-117">إذا لم تظهر بصمات الأصابع في Windows Hello كخيار في **خيارات تسجيل الدخول**، فهذا يعني ان نظام التشغيل windows لا يدرك بأي قارئ أو ماسح ضوئي آخر متصل بالكمبيوتر الشخصي الخاص بك ، أو ان نهج النظام يمنع استخدامه (إذا كان الكمبيوتر تتم ادارته بواسطة مكان عملك).</span><span class="sxs-lookup"><span data-stu-id="5913f-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="5913f-118">لاستكشاف الأخطاء وإصلاحها:</span><span class="sxs-lookup"><span data-stu-id="5913f-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="5913f-119">حدد زر **البدء** في شريط المهام وابحث عن **أداره الاجهزه**.</span><span class="sxs-lookup"><span data-stu-id="5913f-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="5913f-120">انقر أو اضغط لفتح **أداره الاجهزه**.</span><span class="sxs-lookup"><span data-stu-id="5913f-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="5913f-121">في "أداره الاجهزه" ، قم بتوسيع أجهزه المقاييس الحيوية بالنقر فوق شارة رتبتها.</span><span class="sxs-lookup"><span data-stu-id="5913f-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![أجهزه المقاييس الحيوية.](media/biometric-devices.png)

4. <span data-ttu-id="5913f-123">يجب ان يكون ماسح بصمات الأصابع مدرجا كجهاز المقاييس الحيوية ، مثل ماسح سينابتيكس وبدي المحمول:</span><span class="sxs-lookup"><span data-stu-id="5913f-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![أجهزه المقاييس الحيوية.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="5913f-125">إذا لم يظهر الماسح الضوئي لبصمه الاصبع ، وكان الماسح الضوئي مدمجا في الكمبيوتر الشخصي ، فانتقل إلى موقع ويب الشركة المصنعة للكمبيوتر الشخصي.</span><span class="sxs-lookup"><span data-stu-id="5913f-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="5913f-126">في قسم الدعم التقني لنموذج الكمبيوتر الشخصي ، ابحث عن برنامج تشغيل Windows 10 للماسح الضوئي الذي يمكنك تثبيته.</span><span class="sxs-lookup"><span data-stu-id="5913f-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="5913f-127">إذا كان الماسح الضوئي منفصلا عن الكمبيوتر الشخصي (المرفق بواسطة USB) ، فانتقل إلى موقع ويب الشركة المصنعة للماسح الضوئي للبحث عن برنامج تشغيل الجهاز الذي يعمل بنظام Windows 10 وتثبيته لنموذج الماسح الضوئي الذي تملكه.</span><span class="sxs-lookup"><span data-stu-id="5913f-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
