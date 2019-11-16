---
title: ديناميات 365-يظهر لوحه التحكم الخطا في Dynamics 365 الموحدة واجهه
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528538"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="f2177-102">تظهر لوحه معلومات غير صحيحه في الواجهة الموحدة Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f2177-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="f2177-103">هناك عده أسباب لماذا قد تري لوحه معلومات مختلفه عن تلك التي تتوقعها:</span><span class="sxs-lookup"><span data-stu-id="f2177-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="f2177-104">قام المستخدم بتعيين لوحه معلومات افتراضيه للمستخدم</span><span class="sxs-lookup"><span data-stu-id="f2177-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="f2177-105">عاده يمكنك تحديد لوحه معلومات افتراضيه للمستخدم يتم تعيينها إذا لم يتم إظهار الزر **تعيين كافتراضي** في شريط الأوامر لوحه التحكم.</span><span class="sxs-lookup"><span data-stu-id="f2177-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="f2177-106">ستتجاوز لوحه معلومات المستخدم الافتراضية كافة لوحات التحكم الافتراضية الأخرى ، حتى إذا لم تكن لوحه التحكم الافتراضية للمستخدم في التطبيق الحالي.</span><span class="sxs-lookup"><span data-stu-id="f2177-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="f2177-107">استخدم الحل التالي للغاء تعيين لوحه التحكم الافتراضية الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="f2177-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="f2177-108">إنشاء لوحه معلومات شخصيه جديده.</span><span class="sxs-lookup"><span data-stu-id="f2177-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="f2177-109">تعيين لوحه التحكم الجديدة كافتراضي المستخدم.</span><span class="sxs-lookup"><span data-stu-id="f2177-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="f2177-110">حذف لوحه التحكم هذه.</span><span class="sxs-lookup"><span data-stu-id="f2177-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="f2177-111">يتم تعيين لوحه التحكم في ملف sitemap</span><span class="sxs-lookup"><span data-stu-id="f2177-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="f2177-112">قد تكون قد قمت بتعيين لوحه معلومات افتراضيه للمؤسسة عن طريق تحديد لوحه معلومات واختيار ' تعيين كافتراضي ' ضمن ' تخصيص النظام '.</span><span class="sxs-lookup"><span data-stu-id="f2177-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="f2177-113">ولكن لوحه التحكم المحددة في مصمم sitemap ستاخذ الاسبقيه علي لوحه التحكم هذه ، إذا كان المستخدم لديه حق الوصول اليها.</span><span class="sxs-lookup"><span data-stu-id="f2177-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="f2177-114">لكي يتمكن المستخدمون من رؤية لوحه التحكم التي قمت بتعيينها كافتراضي للمؤسسة ، يمكنك اما:</span><span class="sxs-lookup"><span data-stu-id="f2177-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="f2177-115">تعيين لوحه التحكم هذه في ملف sitemap</span><span class="sxs-lookup"><span data-stu-id="f2177-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="f2177-116">أزاله الوصول إلى لوحه معلومات محدده لملف sitemap لهؤلاء المستخدمين</span><span class="sxs-lookup"><span data-stu-id="f2177-116">Remove access to the sitemap defined dashboard for those users</span></span>
