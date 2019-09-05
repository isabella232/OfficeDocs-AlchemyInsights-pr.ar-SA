---
title: استكشاف الأخطاء وإصلاحها - لم يتم العثور على المستخدم في الدليل
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754179"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="19bdd-102">استكشاف الأخطاء وإصلاحها - لم يتم العثور على المستخدم في الدليل</span><span class="sxs-lookup"><span data-stu-id="19bdd-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="19bdd-103">إذا كان المستخدمون يتلقون رسالة خطأ "لا يمكن العثور على المستخدم" في الدليل.</span><span class="sxs-lookup"><span data-stu-id="19bdd-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="19bdd-104">الرجاء المحاولة مرة أخرى حيث يكون "نوع المشكلة" المستخدم غير موجود في الدليل.</span><span class="sxs-lookup"><span data-stu-id="19bdd-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="19bdd-105">يمكن إكمال الخطوات التالية لاستكشاف المشكلة وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="19bdd-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="19bdd-106">تأكد من أن الحساب الذي قبل دعوة البريد الإلكتروني هو نفس الحساب الذي يتم استخدامه لتسجيل الدخول لاحقًا.</span><span class="sxs-lookup"><span data-stu-id="19bdd-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="19bdd-107">تأكد من أن المستخدم يستخدم نفس الحساب لقبول الدعوة والتسجيل في الموقع.</span><span class="sxs-lookup"><span data-stu-id="19bdd-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="19bdd-108">لمزيد من المعلومات، راجع [كيفية إدارة</a> الأسماء المستعارة لحساب Microsoft الخاص بك لإدارة تسجيل دخول Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="19bdd-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="19bdd-109">استعرض للوصول إلى كل موقع (مواقع) يتلقى المستخدم الخطأ.</span><span class="sxs-lookup"><span data-stu-id="19bdd-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="19bdd-110">إضافة "/_layouts/15/people.aspx/membershipgroupid =0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية URL الموقع.</span><span class="sxs-lookup"><span data-stu-id="19bdd-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="19bdd-111">على سبيل المثال: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="19bdd-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="19bdd-112">حدد المستخدم من القائمة.</span><span class="sxs-lookup"><span data-stu-id="19bdd-112">Select the user from the list.</span></span>

- <span data-ttu-id="19bdd-113">انقر فوق **إزالة أذونات المستخدم** من الشريط.</span><span class="sxs-lookup"><span data-stu-id="19bdd-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="19bdd-114">إضافة المستخدم مرة أخرى وإعادة إرسال الدعوة إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="19bdd-114">Add back the User and Resend the invite to the user.</span></span>

