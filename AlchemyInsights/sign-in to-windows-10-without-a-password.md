---
title: تسجيل الدخول إلى Windows 10 بدون استخدام كلمة مرور
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830533"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="2712d-102">تسجيل الدخول إلى Windows 10 بدون استخدام كلمة مرور</span><span class="sxs-lookup"><span data-stu-id="2712d-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="2712d-103">لتجنب الحاجة إلى كتابة كلمة مرور عند بدء تشغيل Windows، نوصي باستخدام أحد خيارات تسجيل الدخول الآمنة في Windows Hello، مثل رقم التعريف الشخصي (PIN) أو التعرف على الوجه أو بصمات الأصابع، إذا كان متوفرا.</span><span class="sxs-lookup"><span data-stu-id="2712d-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="2712d-104">إذا كنت تريد حقا تعطيل تسجيل الدخول الآمن، فشاهد إرشادات "تسجيل الدخول تلقائيا إلى Windows 10" أدناه.</span><span class="sxs-lookup"><span data-stu-id="2712d-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="2712d-105">**تأمين بدائل Windows Hello لكلمة مرور الحساب**</span><span class="sxs-lookup"><span data-stu-id="2712d-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="2712d-106">انتقل إلى **إعدادات > الحسابات > خيارات تسجيل الدخول** (أو انقر [هنا).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="2712d-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2712d-107">سيتم إدراج خيارات تسجيل الدخول المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="2712d-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="2712d-108">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="2712d-108">For example:</span></span>

![خيارات تسجيل الدخول.](media/sign-in-options.png)

<span data-ttu-id="2712d-110">انقر فوق أحد الخيارات لتكوينه أو اضغط عليه.</span><span class="sxs-lookup"><span data-stu-id="2712d-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="2712d-111">في المرة التالية التي تبدأ فيها تشغيل Windows أو إلغاء تأمينه، ستكون قادرا على استخدام الخيار الجديد بدلا من كلمة مرور.</span><span class="sxs-lookup"><span data-stu-id="2712d-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="2712d-112">**تسجيل الدخول تلقائيا إلى Windows 10**</span><span class="sxs-lookup"><span data-stu-id="2712d-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="2712d-113">**ملاحظة:** إن تسجيل الدخول التلقائي ملائم، ولكنه يقدم خطرا على الأمان، خاصة إذا كان يمكن الوصول إلى جهاز الكمبيوتر الخاص بك من قبل عدة أشخاص.</span><span class="sxs-lookup"><span data-stu-id="2712d-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="2712d-114">انقر فوق الزر **بدء** في شريط المهام أو اضغط عليه.</span><span class="sxs-lookup"><span data-stu-id="2712d-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="2712d-115">اكتب **netplwiz وادخل** المفتاح Enter لفتح نافذة حسابات المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="2712d-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="2712d-116">في **حسابات المستخدمين،** انقر فوق الحساب الذي تريد تسجيل الدخول تلقائيا إلى عند بدء تشغيل Windows.</span><span class="sxs-lookup"><span data-stu-id="2712d-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="2712d-117">قم ب إلغاء تحديد خانة الاختيار "يجب على المستخدمين إدخال اسم المستخدم وكلمة المرور لاستخدام هذا الكمبيوتر".</span><span class="sxs-lookup"><span data-stu-id="2712d-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![يجب على المستخدمين إدخال خيار اسم المستخدم وكلمة المرور.](media/users-must-enter-username.png)

5. <span data-ttu-id="2712d-119">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2712d-119">Click **OK**.</span></span> <span data-ttu-id="2712d-120">سيطلب منك إدخال كلمة المرور للحساب الذي حددته وتأكيدها.</span><span class="sxs-lookup"><span data-stu-id="2712d-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="2712d-121">انقر **فوق موافق** للانتهاء.</span><span class="sxs-lookup"><span data-stu-id="2712d-121">Click **OK** to finish.</span></span> <span data-ttu-id="2712d-122">في المرة التالية التي يبدأ فيها تشغيل Windows 10، سيتم تسجيل الدخول تلقائيا إلى الحساب الذي حددته.</span><span class="sxs-lookup"><span data-stu-id="2712d-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
