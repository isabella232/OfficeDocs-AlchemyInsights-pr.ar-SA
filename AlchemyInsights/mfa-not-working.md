---
title: المشاكل المتعلقة بالMFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755118"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="f7300-102">المشاكل المتعلقة باستخدام Azure MFA</span><span class="sxs-lookup"><span data-stu-id="f7300-102">Issues with Azure MFA</span></span>
<span data-ttu-id="f7300-103">هناك بعض الأمور التي يجب التحقق من عدم تمكن المستخدمين من تسجيل الدخول باستخدام مصادقه متعددة العوامل (MFA)</span><span class="sxs-lookup"><span data-stu-id="f7300-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="f7300-104">قد يكون المستخدم المتاثر محظورا في مدخل Azure Active directory.</span><span class="sxs-lookup"><span data-stu-id="f7300-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="f7300-105">إذا كانت هذه هي الحالة ، سيتم رفض محاولات المصادقة لهذا المستخدم المحدد تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="f7300-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="f7300-106">الرجاء اتباع الخطوات المذكورة في هذه المقالة للغاء حظرها.</span><span class="sxs-lookup"><span data-stu-id="f7300-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="f7300-107">إذا لم يساعدك إلغاء حظر المستخدم أو إذا لم يتم حظر المستخدم ، فيمكنك محاولة أعاده تعيين MFA للمستخدم سيمر علي عمليه التسجيل مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="f7300-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="f7300-108">الرجاء اتباع الخطوات الواردة في هذه المقالة.</span><span class="sxs-lookup"><span data-stu-id="f7300-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="f7300-109">إذا كانت هذه هي المرة الاولي التي تقوم فيها بتمكين MFA وكان المستخدمون غير قادرين علي تسجيل الدخول إلى العملاء الذين لا يستخدمون برنامج Outlook ، أو Skype ، وغير ذلك ، فهذا يعني انه لم يتم تمكين الأمر ADAL (مكتبه مصادقه Active directory) علي اشتراكك في O365.</span><span class="sxs-lookup"><span data-stu-id="f7300-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="f7300-110">في هذه الحالة ستحتاج إلى الاتصال ب Exchange Online Powershell وتشغيل أمر cmdlet هذا:  *Set-get-organizationconfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="f7300-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>