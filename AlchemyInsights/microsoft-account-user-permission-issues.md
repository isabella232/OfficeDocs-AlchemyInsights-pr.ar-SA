---
title: استكشاف أخطاء المشكلة-لم يتم العثور علي المستخدم في الدليل
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768788"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="8e62b-102">استكشاف أخطاء المشكلة-لم يتم العثور علي المستخدم في الدليل</span><span class="sxs-lookup"><span data-stu-id="8e62b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="8e62b-103">إذا كان المستخدمون يتلقون رسالة خطا "لا يمكن العثور علي المستخدم" في الدليل ، الرجاء المحاولة مره أخرى حيث "نوع المشكلة" المستخدم غير موجود في الدليل.</span><span class="sxs-lookup"><span data-stu-id="8e62b-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="8e62b-104">يمكن إكمال الخطوات التالية لاستكشاف المشكلة وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="8e62b-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="8e62b-105">تاكد من ان الحساب الذي قبل دعوه البريد الكتروني هو نفس الحساب الذي يتم استخدامه لتسجيل الدخول لاحقا.</span><span class="sxs-lookup"><span data-stu-id="8e62b-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="8e62b-106">تاكد من ان المستخدم يستخدم نفس الحساب لقبول الدعوة وتسجيل الدخول إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="8e62b-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="8e62b-107">لمزيد من المعلومات ، راجع [كيفيه أداره الأسماء المستعارة لحساب</a> Microsoft الخاص بك لأداره المكتب 365 تسجيل الدخول](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="8e62b-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="8e62b-108">استعرض لكل موقع (مواقع) حيث يتلقى المستخدم الخطا.</span><span class="sxs-lookup"><span data-stu-id="8e62b-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="8e62b-109">أضافه "/_layouts/15/sys\sscsx/mcershipgrid = 0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية URL الموقع.</span><span class="sxs-lookup"><span data-stu-id="8e62b-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="8e62b-110">علي سبيل المثال: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="8e62b-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="8e62b-111">حدد المستخدم من القائمة.</span><span class="sxs-lookup"><span data-stu-id="8e62b-111">Select the user from the list.</span></span>

- <span data-ttu-id="8e62b-112">انقر فوق **أزاله أذونات المستخدم** من "الشريط".</span><span class="sxs-lookup"><span data-stu-id="8e62b-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="8e62b-113">أضافه المستخدم وأعاده إرسال الدعوة إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="8e62b-113">Add back the User and Resend the invite to the user.</span></span>

