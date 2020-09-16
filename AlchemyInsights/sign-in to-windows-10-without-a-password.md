---
title: تسجيل الدخول إلى Windows 10 دون استخدام كلمه مرور
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719940"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="d7100-102">تسجيل الدخول إلى Windows 10 دون استخدام كلمه مرور</span><span class="sxs-lookup"><span data-stu-id="d7100-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="d7100-103">لتجنب الحاجة إلى كتابه كلمه مرور في "بدء تشغيل Windows" ، نوصيك باستخدام أحد خيارات تسجيل الدخول الامنه في Windows Hello ، مثل رمز PIN أو التعرف علي الوجه أو بصمه الاصبع ، إذا كانت متوفرة.</span><span class="sxs-lookup"><span data-stu-id="d7100-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="d7100-104">إذا كنت ترغب حقا في تعطيل تسجيل الدخول الأمن ، فراجع الإرشادات "تسجيل الدخول تلقائيا إلى Windows 10" أدناه.</span><span class="sxs-lookup"><span data-stu-id="d7100-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="d7100-105">**حماية البدائل في Windows Hello إلى كلمه مرور الحساب**</span><span class="sxs-lookup"><span data-stu-id="d7100-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="d7100-106">انتقل إلى **إعدادات > حسابات > خيارات تسجيل الدخول** (أو انقر [هنا](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="d7100-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d7100-107">سيتم ادراج خيارات تسجيل الدخول المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="d7100-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="d7100-108">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="d7100-108">For example:</span></span>

![خيارات تسجيل الدخول.](media/sign-in-options.png)

<span data-ttu-id="d7100-110">انقر فوق أحد الخيارات أو اضغط عليه لتكوينه.</span><span class="sxs-lookup"><span data-stu-id="d7100-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="d7100-111">في المرة التالية التي تقوم فيها بتشغيل Windows أو إلغاء تامينه ، ستتمكن من استخدام الخيار جديد بدلا من كلمه المرور.</span><span class="sxs-lookup"><span data-stu-id="d7100-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="d7100-112">**تسجيل الدخول تلقائيا إلى Windows 10**</span><span class="sxs-lookup"><span data-stu-id="d7100-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="d7100-113">**ملاحظه**: ان تسجيل الدخول التلقائي مناسب ، ولكنه يقدم خطورة علي الأمان ، خاصه إذا كان الأشخاص الذين يمكنهم الوصول إلى الكمبيوتر الشخصي.</span><span class="sxs-lookup"><span data-stu-id="d7100-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="d7100-114">انقر فوق زر **البدء** أو اضغط عليه في شريط المهام.</span><span class="sxs-lookup"><span data-stu-id="d7100-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="d7100-115">اكتب **نيتبلويز** واضغط علي المفتاح Enter لفتح نافذه حسابات المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="d7100-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="d7100-116">في **حسابات المستخدمين**، انقر فوق الحساب الذي تريد تسجيل الدخول اليه تلقائيا عند بدء تشغيل Windows.</span><span class="sxs-lookup"><span data-stu-id="d7100-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="d7100-117">قم بإلغاء تحديد خانه الاختيار "يجب علي المستخدمين إدخال اسم المستخدم وكلمه المرور لاستخدام هذا الكمبيوتر".</span><span class="sxs-lookup"><span data-stu-id="d7100-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![يجب ان يدخل المستخدمون خيار اسم المستخدم وكلمه المرور.](media/users-must-enter-username.png)

5. <span data-ttu-id="d7100-119">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d7100-119">Click **OK**.</span></span> <span data-ttu-id="d7100-120">ستتم مطالبتك بإدخال كلمه المرور الخاصة بالحساب الذي حددته وتاكيدها.</span><span class="sxs-lookup"><span data-stu-id="d7100-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="d7100-121">انقر فوق **موافق** للانتهاء.</span><span class="sxs-lookup"><span data-stu-id="d7100-121">Click **OK** to finish.</span></span> <span data-ttu-id="d7100-122">في المرة التالية التي يتم فيها بدء تشغيل Windows 10 ، سيقوم تلقائيا بتسجيل الدخول إلى الحساب الذي حددته.</span><span class="sxs-lookup"><span data-stu-id="d7100-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
