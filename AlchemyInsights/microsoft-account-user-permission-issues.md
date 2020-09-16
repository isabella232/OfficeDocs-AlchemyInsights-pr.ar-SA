---
title: مشكله استكشاف الأخطاء وإصلاحها-تعذر العثور علي المستخدم في الدليل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725394"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="9241e-102">مشكله استكشاف الأخطاء وإصلاحها-تعذر العثور علي المستخدم في الدليل</span><span class="sxs-lookup"><span data-stu-id="9241e-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="9241e-103">إذا قام المستخدمون بتلقي رسالة خطا "تعذر العثور علي المستخدم" في الدليل ، يرجى المحاولة مره أخرى حيث يكون نوع المشكلة مستخدما ليس في الدليل.</span><span class="sxs-lookup"><span data-stu-id="9241e-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="9241e-104">يمكن إكمال الخطوات التالية لاستكشاف المشكلة وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="9241e-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="9241e-105">تاكد من ان الحساب الذي وافق علي دعوه البريد الكتروني هي نفس الحساب الذي يتم استخدامه لتسجيل الدخول لاحقا.</span><span class="sxs-lookup"><span data-stu-id="9241e-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="9241e-106">تاكد من ان المستخدم يستخدم الحساب نفسه لقبول الدعوة وتسجيل الدخول إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="9241e-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="9241e-107">لمزيد من المعلومات ، راجع [كيفيه أداره الأسماء المستعارة لحساب microsoft الخاص بك </a> لأداره تسجيل الدخول إلى microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="9241e-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="9241e-108">استعرض وصولا إلى الموقع (المواقع) الذي يتلقى فيه المستخدم الخطا.</span><span class="sxs-lookup"><span data-stu-id="9241e-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="9241e-109">أضف "/_layouts/15/people.aspx/membershipgroupid = 0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية عنوان URL الخاص بالموقع.</span><span class="sxs-lookup"><span data-stu-id="9241e-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="9241e-110">مثال: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="9241e-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="9241e-111">حدد المستخدم من القائمة.</span><span class="sxs-lookup"><span data-stu-id="9241e-111">Select the user from the list.</span></span>

- <span data-ttu-id="9241e-112">انقر فوق **أزاله أذونات المستخدمين** من الشريط.</span><span class="sxs-lookup"><span data-stu-id="9241e-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="9241e-113">أضف المستخدم وأرسل الدعوة إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="9241e-113">Add back the User and Resend the invite to the user.</span></span>

