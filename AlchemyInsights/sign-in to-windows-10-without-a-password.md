---
title: تسجيل الدخول إلى Windows 10 دون استخدام كلمة مرور
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588268"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="f0276-102">تسجيل الدخول إلى Windows 10 دون استخدام كلمة مرور</span><span class="sxs-lookup"><span data-stu-id="f0276-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="f0276-103">لتجنب الحاجة إلى كتابة كلمة مرور عند بدء تشغيل Windows، نوصي باستخدام أحد خيارات تسجيل الدخول الآمنة في Windows Hello، مثل رقم التعريف الشخصي أو التعرف على الوجه أو بصمة الإصبع، إذا كانت متوفرة.</span><span class="sxs-lookup"><span data-stu-id="f0276-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="f0276-104">إذا كنت تريد حقًا تعطيل تسجيل الدخول الآمن، فراجع إرشادات "تسجيل الدخول تلقائيًا إلى Windows 10" أدناه.</span><span class="sxs-lookup"><span data-stu-id="f0276-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="f0276-105">**تأمين بدائل Windows Hello لكلمة مرور الحساب**</span><span class="sxs-lookup"><span data-stu-id="f0276-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="f0276-106">انتقل إلى **إعدادات > الحسابات > خيارات تسجيل الدخول** (أو انقر [هنا).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="f0276-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="f0276-107">سيتم سرد خيارات تسجيل الدخول المتاحة.</span><span class="sxs-lookup"><span data-stu-id="f0276-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="f0276-108">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="f0276-108">For example:</span></span>

![خيارات تسجيل الدخول.](media/sign-in-options.png)

<span data-ttu-id="f0276-110">انقر فوق أحد الخيارات لتكوينه أو اضغط عليه.</span><span class="sxs-lookup"><span data-stu-id="f0276-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="f0276-111">في المرة القادمة التي تبدأ فيها تشغيل Windows أو إلغاء قفله، ستتمكن من استخدام الخيار الجديد بدلاً من كلمة مرور.</span><span class="sxs-lookup"><span data-stu-id="f0276-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="f0276-112">**تسجيل الدخول تلقائيًا إلى Windows 10**</span><span class="sxs-lookup"><span data-stu-id="f0276-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="f0276-113">**ملاحظة:** تسجيل الدخول التلقائي مناسب، ولكنه يقدم خطرًا أمنيًا، خاصة إذا كان الكمبيوتر الخاص بك يمكن الوصول إليه من قبل عدة أشخاص.</span><span class="sxs-lookup"><span data-stu-id="f0276-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="f0276-114">انقر أو اضغط على زر **البدء** في شريط المهام.</span><span class="sxs-lookup"><span data-stu-id="f0276-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="f0276-115">اكتب **netplwiz** وضرب مفتاح إدخال لفتح نافذة حسابات المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="f0276-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="f0276-116">في **حسابات المستخدمين،** انقر فوق الحساب الذي تريد تسجيل الدخول إليه تلقائيًا عند بدء تشغيل Windows.</span><span class="sxs-lookup"><span data-stu-id="f0276-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="f0276-117">إلغاء تحديد خانة الاختيار "يجب على المستخدمين إدخال اسم مستخدم وكلمة مرور لاستخدام هذا الكمبيوتر".</span><span class="sxs-lookup"><span data-stu-id="f0276-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![يجب على المستخدمين إدخال خيار اسم المستخدم وكلمة المرور.](media/users-must-enter-username.png)

5. <span data-ttu-id="f0276-119">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="f0276-119">Click **OK**.</span></span> <span data-ttu-id="f0276-120">سيُطلب منك إدخال كلمة المرور الخاصة بالحساب الذي حددته وتأكيدها.</span><span class="sxs-lookup"><span data-stu-id="f0276-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="f0276-121">انقر فوق **موافق** للانتهاء.</span><span class="sxs-lookup"><span data-stu-id="f0276-121">Click **OK** to finish.</span></span> <span data-ttu-id="f0276-122">في المرة القادمة التي يبدأ فيها Windows 10، سيقوم بتسجيل الدخول تلقائيًا إلى الحساب الذي حددته.</span><span class="sxs-lookup"><span data-stu-id="f0276-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
