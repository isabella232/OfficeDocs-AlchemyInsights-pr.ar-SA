---
title: حل المشكلة-المستخدم غير موجود في الدليل
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544850"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="9486c-102">حل المشكلة-المستخدم غير موجود في الدليل</span><span class="sxs-lookup"><span data-stu-id="9486c-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="9486c-103">إذا كان المستخدمون تتلقى خطأ رسالة "لا يمكن العثور على المستخدم" في الدليل.</span><span class="sxs-lookup"><span data-stu-id="9486c-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="9486c-104">الرجاء المحاولة مرة أخرى حيث "نوع المشكلة" غير المستخدم في الدليل.</span><span class="sxs-lookup"><span data-stu-id="9486c-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="9486c-105">يمكن إكمال الخطوات التالية استكشاف المشكلة وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="9486c-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="9486c-106">تأكد من الحساب الذي قبلت دعوة البريد الإلكتروني هو نفسه الحساب الذي يتم استخدامه لتسجيل الدخول لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="9486c-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="9486c-107">تأكد من أن المستخدم يستخدم نفس الحساب لقبول الدعوة وتسجيل الدخول إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="9486c-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="9486c-108">لمزيد من المعلومات، راجع [كيفية إدارة الأسماء المستعارة لحساب Microsoft</a> لإدارة تسجيل الدخول Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="9486c-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="9486c-109">استعرض للوصول إلى كل المواقع التي يتلقى المستخدم الخطأ.</span><span class="sxs-lookup"><span data-stu-id="9486c-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="9486c-110">إضافة "/_layouts/15/people.aspx/membershipgroupid=0" (داخل علامات اقتباس المزدوجة) إلى نهاية url الخاص بالموقع.</span><span class="sxs-lookup"><span data-stu-id="9486c-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="9486c-111">على سبيل المثال: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="9486c-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="9486c-112">حدد المستخدم من القائمة.</span><span class="sxs-lookup"><span data-stu-id="9486c-112">Select the user from the list.</span></span>

- <span data-ttu-id="9486c-113">انقر فوق **إزالة أذونات المستخدم** من "الشريط".</span><span class="sxs-lookup"><span data-stu-id="9486c-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="9486c-114">إضافة المستخدم مرة أخرى وإعادة إرسال الدعوة إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="9486c-114">Add back the User and Resend the invite to the user.</span></span>

