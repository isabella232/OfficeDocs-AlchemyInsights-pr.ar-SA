---
title: حل أخطاء المنتج غير المرخص
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737940"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="7e16e-102">اقتراحات لحل الأخطاء "منتج غير مرخص"</span><span class="sxs-lookup"><span data-stu-id="7e16e-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="7e16e-103">لحل الأخطاء المتعلقة بمنتج غير مرخص ، جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="7e16e-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="7e16e-104">تحقق لمعرفه ما إذا كانت حاله الاشتراك قد انتهت صلاحيتها.</span><span class="sxs-lookup"><span data-stu-id="7e16e-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="7e16e-105">تاكد من ان لديك اشتراك يسمح لتراخيص العميل ، مثل تطبيقات Microsoft 365 للاعمال أو الشركات المتميزة ، [وتاكد من ان المستخدم يملك ترخيصا معينا](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="7e16e-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="7e16e-106">تاكد من ان المستخدم سيقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين الترخيص له.</span><span class="sxs-lookup"><span data-stu-id="7e16e-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="7e16e-107">تحقق من [صفحه حماية الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك اي مشاكل معروفه تتعلق بالخدمة.</span><span class="sxs-lookup"><span data-stu-id="7e16e-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="7e16e-108">تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر وصول تطبيقات Microsoft 365 إلى الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="7e16e-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="7e16e-109">راجع [نطاقات عناوين IP و url](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="7e16e-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="7e16e-110">قد تجرب أيضا إجراءات استكشاف الأخطاء وإصلاحها التالية:</span><span class="sxs-lookup"><span data-stu-id="7e16e-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="7e16e-111">افتح تطبيق Office [وسجل خروجك](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) من اي حسابات مستخدمين موجودة.</span><span class="sxs-lookup"><span data-stu-id="7e16e-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="7e16e-112">قم [بازاله](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ترخيص office [وأعاده تعيينه](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ، ثم قم [بتسجيل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتاثر.</span><span class="sxs-lookup"><span data-stu-id="7e16e-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="7e16e-113">شغل [مستكشف أخطاء التنشيط ومصلحها](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="7e16e-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="7e16e-114">[أعاده تعيين حاله تنشيط Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="7e16e-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="7e16e-115">[قم باجراء إصلاح عبر الإنترنت ل Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="7e16e-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="7e16e-116">للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="7e16e-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="7e16e-117">المنتج غير المرخص وأخطاء التنشيط في Office</span><span class="sxs-lookup"><span data-stu-id="7e16e-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="7e16e-118">"عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="7e16e-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)