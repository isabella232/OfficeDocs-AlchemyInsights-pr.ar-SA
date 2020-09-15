---
title: Dynamics 365-تعرض لوحه معلومات غير صحيحه في الواجهة الموحدة في Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711262"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="5d8c3-102">تعرض لوحه معلومات غير صحيحه في الواجهة الموحدة في Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="5d8c3-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="5d8c3-103">ثمة أسباب عديده وراء ظهور لوحه معلومات مختلفه عن تلك التي تتوقعها:</span><span class="sxs-lookup"><span data-stu-id="5d8c3-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="5d8c3-104">قام المستخدم بتعيين لوحه معلومات افتراضيه للمستخدم</span><span class="sxs-lookup"><span data-stu-id="5d8c3-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="5d8c3-105">يمكنك عاده تحديد لوحه معلومات افتراضيه للمستخدمين إذا لم يظهر الزر **تعيين كافتراضي** في شريط أوامر لوحه الاداات.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="5d8c3-106">ستتجاوز لوحه المعلومات الافتراضية للمستخدم كل لوحات معلوماتك الافتراضية ، حتى لو لم تكن لوحه المعلومات الافتراضية للمستخدم في التطبيق الحالي.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="5d8c3-107">استخدم الحل البديل التالي للغاء تعيين لوحه الاجهزه الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="5d8c3-108">إنشاء لوحه معلومات شخصيه جديده.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="5d8c3-109">تعيين لوحه المعلومات الجديدة كمستخدم افتراضي.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="5d8c3-110">احذف لوحه المعلومات هذه.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="5d8c3-111">تعيين لوحه المعلومات في خريطة الموقع</span><span class="sxs-lookup"><span data-stu-id="5d8c3-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="5d8c3-112">ربما قمت بتعيين لوحه معلومات المؤسسة الافتراضية عن طريق تحديد لوحه معلومات واختيار ' تعيين كافتراضي ' ضمن ' تخصيص النظام '.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="5d8c3-113">لكن لوحه الاداات المعرفة في مصمم خريطة الموقع ستاخذ الاسبقيه علي لوحه التحكم هذه ، إذا كان المستخدم يملك حق الوصول اليه.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="5d8c3-114">لكي يتمكن المستخدمون من رؤية لوحه المعلومات التي قمت بتعيينها كالمؤسسة الافتراضية ، يمكنك اما:</span><span class="sxs-lookup"><span data-stu-id="5d8c3-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="5d8c3-115">تعيين لوحه المعلومات هذه في خريطة الموقع</span><span class="sxs-lookup"><span data-stu-id="5d8c3-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="5d8c3-116">أزاله امكانيه الوصول إلى لوحه خريطة الموقع المحددة لهؤلاء المستخدمين</span><span class="sxs-lookup"><span data-stu-id="5d8c3-116">Remove access to the sitemap defined dashboard for those users</span></span>
