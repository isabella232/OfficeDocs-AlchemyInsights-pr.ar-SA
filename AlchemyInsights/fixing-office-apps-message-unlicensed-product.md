---
title: غير قادر على تنشيط Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: ee4618bd288e3e8be75dc969af58f921a14f48b0
ms.sourcegitcommit: bf87d91fa60bd961bc6c887c4a4be7a3c7665b38
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/01/2020
ms.locfileid: "44474484"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="c4225-102">غير قادر على تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="c4225-102">Unable to activate Office</span></span>

- <span data-ttu-id="c4225-103">تحقق مما إذا كانت حالة الاشتراك منتهية الصلاحية.</span><span class="sxs-lookup"><span data-stu-id="c4225-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="c4225-104">تأكد من وجود اشتراك يسمح بتراخيص العميل، مثل Office 365 Business أو Business Premium، [وتأكد من أن المستخدم لديه ترخيص معين](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="c4225-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="c4225-105">تأكد من أن المستخدم يقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين ترخيص له.</span><span class="sxs-lookup"><span data-stu-id="c4225-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="c4225-106">تحقق من [صفحه حماية خدمة Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك أي مشكلات معروفة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="c4225-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="c4225-107">تحقق من جدار الحماية وإعدادات برنامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من عدم حظر وصول تطبيقات Office إلى الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="c4225-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Office apps access to the internet.</span></span> <span data-ttu-id="c4225-108">الرجاء الاطلاع على [نطاقات عناوين IP وعناوين URL في Office 365](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "نطاقات عناوين IP وعناوين URL في Office 365").</span><span class="sxs-lookup"><span data-stu-id="c4225-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="c4225-109">استخدم إجراءات استكشاف الأخطاء وإصلاحها التالية:</span><span class="sxs-lookup"><span data-stu-id="c4225-109">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="c4225-110">افتح أحد تطبيقات Office، ثم [قم بتسجيل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)من أي حسابات مستخدم حالية.</span><span class="sxs-lookup"><span data-stu-id="c4225-110">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="c4225-111">[قم بإزالة](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "ازاله") و[إعادة تعيين](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "إعادة التعيين") ترخيص Office، ثم [سجّل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "تسجيل الدخول إلى Office") باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="c4225-111">[Remove](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Remove") and [re-assign](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "re-assign") Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "sign into Office") using the affected user account.</span></span>
- <span data-ttu-id="c4225-112">تشغيل ["مستكشف أخطاء التنشيط ومصلحها"](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="c4225-112">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="c4225-113">إعادة تعيين حالة تنشيط Office</span><span class="sxs-lookup"><span data-stu-id="c4225-113">Reset Office activation state</span></span>](https://docs.microsoft.com/en-us/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "إعادة تعيين حالة تنشيط Office")
- [<span data-ttu-id="c4225-114">قم بإجراء إصلاح Office عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="c4225-114">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="c4225-115">للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="c4225-115">For additional troubleshooting solutions, see:</span></span>  
[<span data-ttu-id="c4225-116">المنتج غير المرخص وأخطاء التنشيط في Office</span><span class="sxs-lookup"><span data-stu-id="c4225-116">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
<span data-ttu-id="c4225-117">["آسف، لا يمكننا الاتصال بحسابك.</span><span class="sxs-lookup"><span data-stu-id="c4225-117">["Sorry, we can't connect to your account.</span></span> <span data-ttu-id="c4225-118">الرجاء المحاولة مرة أخرى لاحقًا" خطأ عند تنشيط Office]( https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 "عذراً، لا يمكننا الاتصال بحسابك.</span><span class="sxs-lookup"><span data-stu-id="c4225-118">Please try again later" error when you activate Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 ""Sorry, we can't connect to your account.</span></span> <span data-ttu-id="c4225-119">الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط Office")</span><span class="sxs-lookup"><span data-stu-id="c4225-119">Please try again later" error when you activate Office")</span></span>