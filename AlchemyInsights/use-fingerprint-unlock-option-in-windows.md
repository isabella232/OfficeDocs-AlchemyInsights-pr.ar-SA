---
title: استخدام خيار إلغاء قفل بصمة الإصبع في Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588303"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="be7b3-102">استخدام خيار إلغاء قفل بصمة الإصبع في Windows 10</span><span class="sxs-lookup"><span data-stu-id="be7b3-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="be7b3-103">**تمكين بصمة Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="be7b3-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="be7b3-104">لإلغاء تأمين Windows 10 باستخدام بصمة إصبعك، تحتاج إلى إعداد بصمة Windows Hello عن طريق إضافة (السماح لـ Windows بالتعرف على) إصبع واحد على الأقل.</span><span class="sxs-lookup"><span data-stu-id="be7b3-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="be7b3-105">انتقل إلى **إعدادات > الحسابات > خيارات تسجيل الدخول** (أو انقر [هنا).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="be7b3-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="be7b3-106">سيتم سرد خيارات تسجيل الدخول المتاحة.</span><span class="sxs-lookup"><span data-stu-id="be7b3-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="be7b3-107">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="be7b3-107">For example:</span></span>

    ![خيارات تسجيل الدخول.](media/sign-in-options.png)

2. <span data-ttu-id="be7b3-109">انقر فوق أو اضغط على **Windows Hello Fingerprint**، ثم انقر فوق **إعداد**.</span><span class="sxs-lookup"><span data-stu-id="be7b3-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="be7b3-110">في نافذة إعداد Windows Hello، انقر فوق **البدء**.</span><span class="sxs-lookup"><span data-stu-id="be7b3-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="be7b3-111">سيتم تنشيط مستشعر بصمة الإصبع، وسيُطلب منك وضع إصبعك على المستشعر:</span><span class="sxs-lookup"><span data-stu-id="be7b3-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![مستشعر بصمات الأصابع.](media/fingerprint-sensor.png)

3. <span data-ttu-id="be7b3-113">اتبع التعليمات، والتي سوف يطلب منك مسح إصبعك مرارا وتكرارا.</span><span class="sxs-lookup"><span data-stu-id="be7b3-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="be7b3-114">عند الانتهاء من ذلك، سيكون لديك خيار إضافة أصابع أخرى قد ترغب في استخدامها لتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="be7b3-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="be7b3-115">في المرة القادمة التي تقوم فيها بتسجيل الدخول إلى Windows 10، سيكون لديك خيار استخدام بصمة إصبعك للقيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="be7b3-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="be7b3-116">**بصمة Windows Hello غير متوفرة كخيار تسجيل الدخول**</span><span class="sxs-lookup"><span data-stu-id="be7b3-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="be7b3-117">إذا لم يتم عرض Windows Hello Fingerprint كخيار في **خيارات تسجيل الدخول**، فهذا يعني أن Windows ليس على علم بأي قارئ بصمات الأصابع / الماسح الضوئي المرفق بالكمبيوتر ، أو أن نهج النظام يمنع استخدامه (على سبيل المثال إذا كان الكمبيوتر الخاص بك مدارًا من قبل مكان عملك).</span><span class="sxs-lookup"><span data-stu-id="be7b3-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="be7b3-118">لاستكشاف الأخطاء وإصلاحها:</span><span class="sxs-lookup"><span data-stu-id="be7b3-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="be7b3-119">حدد زر **البدء** في شريط المهام وابحث عن **إدارة الأجهزة**.</span><span class="sxs-lookup"><span data-stu-id="be7b3-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="be7b3-120">انقر أو اضغط لفتح **إدارة الأجهزة**.</span><span class="sxs-lookup"><span data-stu-id="be7b3-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="be7b3-121">في إدارة الأجهزة، قم بتوسيع الأجهزة البيومترية بالنقر فوق شيفرون.</span><span class="sxs-lookup"><span data-stu-id="be7b3-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![الأجهزة البيومترية.](media/biometric-devices.png)

4. <span data-ttu-id="be7b3-123">يجب إدراج ماسح بصمات الأصابع كجهاز بيومتري، مثل ماسح متشابك WBDI:</span><span class="sxs-lookup"><span data-stu-id="be7b3-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![الأجهزة البيومترية.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="be7b3-125">إذا لم يتم عرض ماسح بصمات الأصابع، وتم دمج الماسح الضوئي في الكمبيوتر، فانتقل إلى موقع ويب الشركة المصنعة للكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="be7b3-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="be7b3-126">في قسم الدعم الفني لطراز الكمبيوتر، ابحث عن برنامج تشغيل Windows 10 للماسح الضوئي الذي يمكنك تثبيته.</span><span class="sxs-lookup"><span data-stu-id="be7b3-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="be7b3-127">إذا كان الماسح الضوئي منفصلًا عن الكمبيوتر الشخصي (مرفق عبر USB)، فانتقل إلى موقع ويب الشركة المصنعة للماسحة الضوئية للعثور على برنامج برنامج تشغيل جهاز Windows 10 وتثبيته لطراز الماسح الضوئي لديك.</span><span class="sxs-lookup"><span data-stu-id="be7b3-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
