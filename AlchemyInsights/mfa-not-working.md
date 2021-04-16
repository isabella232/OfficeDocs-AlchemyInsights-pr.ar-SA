---
title: مشاكل في MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810471"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="3f2cf-102">مشاكل في Azure MFA</span><span class="sxs-lookup"><span data-stu-id="3f2cf-102">Issues with Azure MFA</span></span>
<span data-ttu-id="3f2cf-103">هناك بعض الأمور التي يجب التحقق مما إذا كان المستخدمون لا يمكنهم تسجيل الدخول باستخدام المصادقة متعددة العوامل (MFA)</span><span class="sxs-lookup"><span data-stu-id="3f2cf-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="3f2cf-104">قد يتم حظر المستخدم المتأثر في مدخل Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3f2cf-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="3f2cf-105">إذا كان الأمر كذلك، سيتم رفض محاولات المصادقة لهذا المستخدم المحدد تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="3f2cf-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="3f2cf-106">الرجاء اتباع الخطوات في هذه المقالة إلغاء حظرها.</span><span class="sxs-lookup"><span data-stu-id="3f2cf-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="3f2cf-107">إذا لم يساعد إلغاء حظر المستخدم أو لم يتم حظر المستخدم، يمكنك محاولة إعادة تعيين MFA للمستخدم وسيخوض عملية التسجيل مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="3f2cf-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="3f2cf-108">الرجاء اتباع الخطوات في هذه المقالة.</span><span class="sxs-lookup"><span data-stu-id="3f2cf-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="3f2cf-109">إذا كانت هذه هي المرة الأولى التي تقوم فيها بتمكين المصادقة متعددة العوامل (MFA) ويتمكن المستخدمون من تسجيل الدخول إلى عملاء لا تستخدم المستعرضات مثل Outlook وسكايب وغير ذلك، ربما لم يتم تمكين ADAL (مكتبة مصادقة Active Directory) في اشتراك O365.</span><span class="sxs-lookup"><span data-stu-id="3f2cf-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="3f2cf-110">في هذه الحالة، ستحتاج إلى الاتصال ب Exchange Online Powershell وتشغيل الأمر cmdlet هذا:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="3f2cf-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>