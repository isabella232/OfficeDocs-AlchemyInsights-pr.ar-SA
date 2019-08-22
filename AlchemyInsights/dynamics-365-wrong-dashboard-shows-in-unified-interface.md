---
title: لوحة معلومات خاطئة Dynamics 365-يظهر في واجهة موحدة Dynamics 365
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528538"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c5f69-102">يعرض لوحة معلومات خاطئة في الواجهة الموحدة ل Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c5f69-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c5f69-103">هناك عدة أسباب لماذا قد تشاهد لوحة معلومات مختلفة عن تلك التي تتوقعها:</span><span class="sxs-lookup"><span data-stu-id="c5f69-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c5f69-104">قام المستخدم بتعيين لوحة معلومات مستخدم الافتراضي</span><span class="sxs-lookup"><span data-stu-id="c5f69-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c5f69-105">عادة يمكنك تعريف مستخدم تم تعيين لوحة معلومات افتراضية في حالة عدم ظهور الزر **تعيين كافتراضي** في شريط أوامر لوحة المعلومات.</span><span class="sxs-lookup"><span data-stu-id="c5f69-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c5f69-106">لوحة معلومات المستخدم الافتراضية ستتجاوز كافة لوحات المعلومات الافتراضية الأخرى، حتى لو لم يكن لوحة المعلومات الافتراضية للمستخدم في التطبيق الحالي.</span><span class="sxs-lookup"><span data-stu-id="c5f69-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c5f69-107">استخدم الحل البديل التالي لإلغاء تعيين لوحة المعلومات الافتراضية الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="c5f69-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c5f69-108">إنشاء لوحة معلومات شخصية جديدة.</span><span class="sxs-lookup"><span data-stu-id="c5f69-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c5f69-109">تعيين لوحة المعلومات الجديدة هذه كمستخدم افتراضي.</span><span class="sxs-lookup"><span data-stu-id="c5f69-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c5f69-110">حذف لوحة المعلومات هذه.</span><span class="sxs-lookup"><span data-stu-id="c5f69-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c5f69-111">تعيين لوحة المعلومات في خريطة الموقع</span><span class="sxs-lookup"><span data-stu-id="c5f69-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c5f69-112">قد تم تعيين تعد لوحة معلومات افتراضية مؤسسة بتحديد لوحة معلومات واختيار '"تعيين كافتراضي"' ضمن '"تخصيص النظام"'.</span><span class="sxs-lookup"><span data-stu-id="c5f69-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c5f69-113">ولكن المعرفة في خريطة الموقع مصمم لوحة المعلومات أسبقية على لوحة المعلومات هذه، إذا كان لدى المستخدم حق الوصول إليه.</span><span class="sxs-lookup"><span data-stu-id="c5f69-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c5f69-114">لجعل مستخدمي رؤية لوحة قمت بتعيين كافتراضي المؤسسة، يمكنك أما:</span><span class="sxs-lookup"><span data-stu-id="c5f69-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c5f69-115">تعيين لوحة المعلومات هذه في مخطط الموقع</span><span class="sxs-lookup"><span data-stu-id="c5f69-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c5f69-116">إزالة الوصول إلى لوحة معلومات الموقع التي تم تعريفها لهؤلاء المستخدمين</span><span class="sxs-lookup"><span data-stu-id="c5f69-116">Remove access to the sitemap defined dashboard for those users</span></span>
