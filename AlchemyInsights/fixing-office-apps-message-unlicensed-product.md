---
title: يتعذر تنشيط Office
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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798667"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="b0295-102">يتعذر تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="b0295-102">Unable to activate Office</span></span>

<span data-ttu-id="b0295-103">**ملاحظة:** إذا كنت تستخدم إصدارا قديما من Windows (على سبيل المثال، Windows 7)، فتأكد من تمكين TLS 1.2 كافتراضي.</span><span class="sxs-lookup"><span data-stu-id="b0295-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="b0295-104">لمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)كبروتوكولات آمنة افتراضية في WinHTTP في Windows .</span><span class="sxs-lookup"><span data-stu-id="b0295-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="b0295-105">تحقق مما إذا كانت حالة الاشتراك منتهية الصلاحية.</span><span class="sxs-lookup"><span data-stu-id="b0295-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="b0295-106">تأكد من أن لديك اشتراكا يسمح بتراخيص العميل، مثل Office 365 Business أو ترخيص Premium، وتأكد من تعيين [ترخيص للمستخدم.](/microsoft-365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="b0295-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="b0295-107">تأكد من أن المستخدم يقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين ترخيص له.</span><span class="sxs-lookup"><span data-stu-id="b0295-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="b0295-108">تحقق من [صفحه حماية خدمة Office 365](/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك أي مشكلات معروفة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="b0295-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="b0295-109">تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع Microsoft 365 الوصول إلى الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="b0295-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="b0295-110">الرجاء الاطلاع على [نطاقات عناوين IP وعناوين URL في Office 365](/office365/enterprise/urls-and-ip-address-ranges "نطاقات عناوين IP وعناوين URL في Office 365").</span><span class="sxs-lookup"><span data-stu-id="b0295-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="b0295-111">**تلميح** على Windows الأجهزة، يمكننا تشخيص العديد من مشاكل تسجيل الدخول الشائعة Office تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="b0295-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="b0295-112">قم بتنزيل **[Microsoft مساعد الإصلاح والدعم](https://aka.ms/SaRA-OfficeSignInScenario)** لاستخدام الأداة التلقائية.</span><span class="sxs-lookup"><span data-stu-id="b0295-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="b0295-113">استخدم إجراءات استكشاف الأخطاء وإصلاحها التالية:</span><span class="sxs-lookup"><span data-stu-id="b0295-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="b0295-114">افتح أحد تطبيقات Office، ثم [قم بتسجيل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)من أي حسابات مستخدم حالية.</span><span class="sxs-lookup"><span data-stu-id="b0295-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="b0295-115">[قم بإزالة](/microsoft-365/admin/manage/remove-licenses-from-users) و[إعادة تعيين](/microsoft-365/admin/manage/assign-licenses-to-users) ترخيص Office، ثم [سجّل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="b0295-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="b0295-116">تشغيل ["مستكشف أخطاء التنشيط ومصلحها"](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="b0295-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="b0295-117">إعادة تعيين حالة تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="b0295-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "إعادة Office التنشيط")
- [<span data-ttu-id="b0295-118">قم بإجراء إصلاح Office عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="b0295-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="b0295-119">للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="b0295-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="b0295-120">المنتج غير المرخص وأخطاء التنشيط في Office</span><span class="sxs-lookup"><span data-stu-id="b0295-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="b0295-121">"عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="b0295-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)