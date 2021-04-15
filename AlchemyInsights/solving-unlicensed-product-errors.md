---
title: حل أخطاء "المنتج غير مرخص"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786836"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="93a08-102">اقتراحات لحل أخطاء "منتج غير مرخص"</span><span class="sxs-lookup"><span data-stu-id="93a08-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="93a08-103">لحل الأخطاء حول "منتج غير مرخص"، جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="93a08-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="93a08-104">تحقق لمعرفة ما إذا انتهت صلاحية حالة اشتراكك.</span><span class="sxs-lookup"><span data-stu-id="93a08-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="93a08-105">تأكد من أن لديك اشتراكا يسمح بتراخيص العميل، مثل Microsoft 365 Apps للأعمال أو Business Premium، وتأكد من تعيين [ترخيص للمستخدم.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="93a08-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="93a08-106">تأكد من أن المستخدم يقوم تسجيل الدخول إلى Office بنفس الحساب الذي تم تعيين الترخيص له.</span><span class="sxs-lookup"><span data-stu-id="93a08-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="93a08-107">تحقق من [صفحة حالة الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفة ما إذا كانت هناك أي مشاكل معروفة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="93a08-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="93a08-108">تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع وصول تطبيقات Microsoft 365 إلى الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="93a08-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="93a08-109">راجع [عناوين URL ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="93a08-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="93a08-110">يمكنك أيضا تجربة إجراءات استكشاف الأخطاء وإصلاحها التالية:</span><span class="sxs-lookup"><span data-stu-id="93a08-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="93a08-111">افتح تطبيق Office و [سجل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) من أي حسابات مستخدمين موجودة.</span><span class="sxs-lookup"><span data-stu-id="93a08-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="93a08-112">[قم](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [بإزالة ترخيص](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office ثم إعادة تعيينه، ثم [سجل الدخول](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) إلى Office باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="93a08-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="93a08-113">تشغيل [م استكشاف مشاكل التنشيط ومشكلاتها ومشكلاتها.](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="93a08-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="93a08-114">[إعادة تعيين حالة تنشيط Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="93a08-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="93a08-115">[إجراء إصلاح عبر الإنترنت ل Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="93a08-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="93a08-116">للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="93a08-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="93a08-117">المنتج غير المرخص وأخطاء التنشيط في Office</span><span class="sxs-lookup"><span data-stu-id="93a08-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="93a08-118">"عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="93a08-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)