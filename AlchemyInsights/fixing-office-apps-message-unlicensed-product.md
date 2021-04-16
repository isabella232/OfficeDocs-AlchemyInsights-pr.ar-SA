---
title: تعذر تنشيط Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812559"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="f35c9-102">تعذر تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="f35c9-102">Unable to activate Office</span></span>

- <span data-ttu-id="f35c9-103">تحقق مما إذا كانت حالة الاشتراك منتهية الصلاحية.</span><span class="sxs-lookup"><span data-stu-id="f35c9-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="f35c9-104">تأكد من أن لديك اشتراكا يسمح بتراخيص العميل، مثل Office 365 Business أو Business Premium، وتأكد من تعيين [ترخيص للمستخدم](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f35c9-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="f35c9-105">تأكد من أن المستخدم يقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين ترخيص له.</span><span class="sxs-lookup"><span data-stu-id="f35c9-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="f35c9-106">تحقق من [صفحه حماية خدمة Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك أي مشكلات معروفة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="f35c9-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="f35c9-107">تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع وصول تطبيقات Microsoft 365 إلى الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="f35c9-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="f35c9-108">الرجاء الاطلاع على [نطاقات عناوين IP وعناوين URL في Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "نطاقات عناوين IP وعناوين URL في Office 365").</span><span class="sxs-lookup"><span data-stu-id="f35c9-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="f35c9-109">**تلميح** على أجهزة Windows، يمكننا تشخيص العديد من مشاكل تسجيل الدخول الشائعة في Office وإصلاحها تلقائيا من أجلك.</span><span class="sxs-lookup"><span data-stu-id="f35c9-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="f35c9-110">قم  **[بتنزيل مساعد الاسترداد والدعم من Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** وتشغيله لاستخدام الأداة التلقائية.</span><span class="sxs-lookup"><span data-stu-id="f35c9-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="f35c9-111">استخدم إجراءات استكشاف الأخطاء وإصلاحها التالية:</span><span class="sxs-lookup"><span data-stu-id="f35c9-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="f35c9-112">افتح أحد تطبيقات Office، ثم [قم بتسجيل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)من أي حسابات مستخدم حالية.</span><span class="sxs-lookup"><span data-stu-id="f35c9-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="f35c9-113">[قم بإزالة](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) و[إعادة تعيين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ترخيص Office، ثم [سجّل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="f35c9-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="f35c9-114">تشغيل ["مستكشف أخطاء التنشيط ومصلحها"](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="f35c9-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="f35c9-115">إعادة تعيين حالة تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="f35c9-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "إعادة تعيين حالة تنشيط Office")
- [<span data-ttu-id="f35c9-116">قم بإجراء إصلاح Office عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="f35c9-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="f35c9-117">للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="f35c9-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="f35c9-118">المنتج غير المرخص وأخطاء التنشيط في Office</span><span class="sxs-lookup"><span data-stu-id="f35c9-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="f35c9-119">"عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="f35c9-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)