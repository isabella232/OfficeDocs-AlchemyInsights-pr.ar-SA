---
title: المشكلات المتعلقة بوزارة الخارجية
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250152"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="a9a89-102">المشكلات المتعلقة بوزارة الخارجية</span><span class="sxs-lookup"><span data-stu-id="a9a89-102">Issues with MFA</span></span>
<span data-ttu-id="a9a89-103">وهناك بضعة أشياء للتحقق من حالة المستخدمين لا يمكن تسجيل الدخول باستخدام مصادقة متعددة العوامل (وزارة الخارجية)</span><span class="sxs-lookup"><span data-stu-id="a9a89-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="a9a89-104">قد يتم حظر المستخدم المتأثر في موقع الدليل النشط Azure.</span><span class="sxs-lookup"><span data-stu-id="a9a89-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="a9a89-105">إذا كان الأمر كذلك، محاولات المصادقة لمستخدم معين سيتم تلقائياً رفض.</span><span class="sxs-lookup"><span data-stu-id="a9a89-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="a9a89-106">الرجاء اتباع الخطوات الموجودة في هذه المقالة لإلغاء حظر هذه الملفات.</span><span class="sxs-lookup"><span data-stu-id="a9a89-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="a9a89-107">إذا لم يساعد إلغاء منع المستخدم أو المستخدم غير محظور يمكنك محاولة إعادة تعيين ترتيب المنسوجات المتعددة الألياف للمستخدم وسوف تخرج من خلال عملية التسجيل مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="a9a89-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="a9a89-108">الرجاء اتباع الخطوات الموجودة في هذه المقالة.</span><span class="sxs-lookup"><span data-stu-id="a9a89-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="a9a89-109">إذا كانت هذه هي المرة الأولى وزارة الخارجية الممكنة والمستخدمين غير قادر على تسجيل الدخول إلى عملاء غير مستعرضات مثل Outlook، Skype، وغيرها، ربما إنبات (مكتبة مصادقة الدليل النشط) غير ممكنة على الاشتراك O365.</span><span class="sxs-lookup"><span data-stu-id="a9a89-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="a9a89-110">في هذه الحالة، ستحتاج إلى الاتصال Powershell Exchange عبر إنترنت وتشغيل الأمر cmdlet:  *مجموعة أورجانيزاتيونكونفيج-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="a9a89-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>