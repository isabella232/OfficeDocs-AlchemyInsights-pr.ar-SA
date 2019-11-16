---
title: قضايا مع وزاره الخارجية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768824"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="3085a-102">قضايا مع وزاره الخارجية Azure</span><span class="sxs-lookup"><span data-stu-id="3085a-102">Issues with Azure MFA</span></span>
<span data-ttu-id="3085a-103">هناك بضعة أشياء للتحقق ما إذا كان المستخدمين لا يمكن تسجيل الدخول باستخدام المصادقة متعددة العوامل (وزاره الخارجية)</span><span class="sxs-lookup"><span data-stu-id="3085a-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="3085a-104">قد يتم حظر المستخدم المتاثر في موقع الدليل النشط Azure.</span><span class="sxs-lookup"><span data-stu-id="3085a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="3085a-105">إذا كانت هذه هي الحالة ، سيتم تلقائيا رفض محاولات المصادقة لهذا المستخدم المحدد.</span><span class="sxs-lookup"><span data-stu-id="3085a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="3085a-106">الرجاء اتباع الخطوات التالية في هذه المقالة للغاء حظرها.</span><span class="sxs-lookup"><span data-stu-id="3085a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="3085a-107">إذا كان إلغاء حظر المستخدم لم يساعد أو لم يتم حظر المستخدم يمكنك محاولة أعاده تعيين وزاره الخارجية للمستخدم وانها سوف تذهب من خلال عمليه التسجيل مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="3085a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="3085a-108">الرجاء اتباع الخطوات التالية في هذه المقالة.</span><span class="sxs-lookup"><span data-stu-id="3085a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="3085a-109">إذا كانت هذه هي المرة الاولي التي قمت بتمكين وزاره الخارجية والمستخدمين غير قادرين علي تسجيل الدخول إلى العملاء غير المستعرضات مثل Outlook ، سكايب ، وما إلى ذلك ، وربما لم يتم تمكين ال (مكتبه مصادقه الدليل النشط) علي الاشتراك O365 الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="3085a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="3085a-110">في هذه الحالة سوف تحتاج إلى الاتصال Powershell Exchange عبر الإنترنت وتشغيل هذا cmdlet:  *مجموعه-اورجانيزاتيونكونفيج-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="3085a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>