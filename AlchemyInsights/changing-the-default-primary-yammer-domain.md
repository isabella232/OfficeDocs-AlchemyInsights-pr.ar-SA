---
title: تغيير مجال Yammer الافتراضي
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817921"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="fa201-102">تغيير مجال Yammer الافتراضي/الأساسي</span><span class="sxs-lookup"><span data-stu-id="fa201-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="fa201-103">يتضمن عنوان URL الخاص بـ Yammer اسم المجال الأساسي الحالي لشبكه Yammer الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="fa201-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="fa201-104">قد لا يتطابق اسم المجال هذا مع مجموعة أسماء المجالات الأساسية في Office 365 أو Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fa201-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="fa201-105">يوجد اختلافات في الأسلوب بناءً على عدد المجالات المخصصة المضافة إلى المستأجر، وعما إذا كان Yammer يتمتع بتكوين مدعوم (مستأجر واحد: شبكة واحدة، أو 1:1).</span><span class="sxs-lookup"><span data-stu-id="fa201-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="fa201-106">تتوفر الوثائق الخاصة بمجالات Yammer [و Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).</span><span class="sxs-lookup"><span data-stu-id="fa201-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="fa201-107">السبب الأكثر شيوعا لرؤية مجال غير صحيح هو وجود العديد من شبكات Yammer والتي يجب تجميعها.</span><span class="sxs-lookup"><span data-stu-id="fa201-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="fa201-108">[إن التجميع وصولًا إلى شبكة واحدة](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) باستخدام أداة ترحيل الشبكة تعتبر خطوة أولى مهمة.</span><span class="sxs-lookup"><span data-stu-id="fa201-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="fa201-109">قم بتكملة ذلك قبل محاولة تعيين مجالك الأساسي.</span><span class="sxs-lookup"><span data-stu-id="fa201-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="fa201-110">**لا يوجد المجالات المخصصة**</span><span class="sxs-lookup"><span data-stu-id="fa201-110">**No custom domains**</span></span>

<span data-ttu-id="fa201-111">بالنسبة للمستأجرين الجدد، سيتم استخدام المجال الافتراضي (على سبيل المثال fabrikam.onmicrosoft.com) من المستأجر لـ Yammer.</span><span class="sxs-lookup"><span data-stu-id="fa201-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="fa201-112">يتم تعيين المجال الأساسي على yammer.com/fabrikam.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="fa201-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="fa201-113">**مجال مخصص واحد**</span><span class="sxs-lookup"><span data-stu-id="fa201-113">**Single custom domain**</span></span>

<span data-ttu-id="fa201-114">سيحدد Yammer المجال المخصص تلقائيًا (على سبيل المثال fabrikam.com) من المستأجر كالمجال الأساسي في Yammer.</span><span class="sxs-lookup"><span data-stu-id="fa201-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="fa201-115">يتم تعيينه على yammer.com/fabrikam.com.</span><span class="sxs-lookup"><span data-stu-id="fa201-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="fa201-116">يتم إجراء هذا التغيير عن طريق خدمة مزامنة المجال، ويمكن أن يستغرق الأمر حتى 24 ساعة حتى يكون ساري المفعول.</span><span class="sxs-lookup"><span data-stu-id="fa201-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="fa201-117">**مجالات مخصصة متعددة**</span><span class="sxs-lookup"><span data-stu-id="fa201-117">**Multiple custom domains**</span></span>

<span data-ttu-id="fa201-118">يمكن أن يتضمن Yammer مجالًا أساسيًا مختلفًا عن المجال المستأجر الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="fa201-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="fa201-119">نظرًا لوجود مجالات مخصصة متعددة، فإن Yammer لا يحاول تخمين المجال الصحيح من تلك المجالات المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="fa201-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="fa201-120">يجب فتح حالة دعم للمطالبة بتغيير اسم المجال الأساسي إلى المجال الأساسي الذي تختاره.</span><span class="sxs-lookup"><span data-stu-id="fa201-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="fa201-121">**معلومات إضافية حول استكشاف الأخطاء وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="fa201-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="fa201-122">من المحتمل في بعض الحالات حدوث تنقل للمجالات بين المستأجرين وعدم تمكن خدمة مزامنة المجال من العمل بنجاح.</span><span class="sxs-lookup"><span data-stu-id="fa201-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="fa201-123">قد تواجهك مشاكل خاصة بتسجيل الدخول أو مشاكل أخرى، بالإضافة إلى وجود مجال أساسي غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="fa201-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="fa201-124">لحل هذه المشكلة، يجب نقل المجالات إلى الشبكة الصحيحة بمساعدة من دعم Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fa201-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="fa201-125">تتطلب هذه الحالة مساعدة مباشرة وقد يُستغرق بعض الوقت لحلها، وخاصة في حالة وجود قائمة طويلة للغاية بأسماء المجالات.</span><span class="sxs-lookup"><span data-stu-id="fa201-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="fa201-126">افتح حالة دعم للحصول على مساعدة في حل تلك الأنواع من المشاكل.</span><span class="sxs-lookup"><span data-stu-id="fa201-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="fa201-127">عند العمل مع وكيل دعم، سيتأكد من التحقق من المجالات على مستأجر تحت سيطرتك.</span><span class="sxs-lookup"><span data-stu-id="fa201-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="fa201-128">قد يسألك أسئلة تحقق إضافية حول مجالاتك إذا ما تم إضافتها إلى مستأجرك ولكن لم يتم التحقق منها بواسطة DNS.</span><span class="sxs-lookup"><span data-stu-id="fa201-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="fa201-129">يرجى التأكد من أنه تم التحقق من المجالات بواسطة DNS لزيادة سرعة العملية.</span><span class="sxs-lookup"><span data-stu-id="fa201-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
