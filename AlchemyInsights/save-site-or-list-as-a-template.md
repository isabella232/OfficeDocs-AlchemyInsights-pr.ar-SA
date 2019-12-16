---
title: حفظ الموقع أو القائمة كقالب
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048711"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="976f0-102">حفظ الموقع أو القائمة كقالب</span><span class="sxs-lookup"><span data-stu-id="976f0-102">Save site or list as a template</span></span>

<span data-ttu-id="976f0-103">قوالب موقع SharePoint هي تعريفات تم بناؤها مسبقا مصممه حول حاجه عمل معينه.</span><span class="sxs-lookup"><span data-stu-id="976f0-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="976f0-104">لمزيد من المعلومات ، راجع [استخدام قوالب لإنشاء أنواع مختلفه من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="976f0-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="976f0-105">فيما يلي بعض المشكلات/الحلول الشائعة المتعلقة بحفظ موقع أو قائمه كقالب في SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="976f0-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="976f0-106">**زر حفظ قالب الموقع/القائمة غير متوفر أو مفقود**.</span><span class="sxs-lookup"><span data-stu-id="976f0-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="976f0-107">سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب.</span><span class="sxs-lookup"><span data-stu-id="976f0-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="976f0-108">للخطوات التفصيلية ، راجع الامثله والاعتبارات [السماح أو منع البرنامج النصي المخصص](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="976f0-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="976f0-109">الأمر حفظ الموقع كقالب غير معتمد ويمكن ان يسبب مشاكل علي المواقع التي تستخدم البنية الاساسيه للنشر خادم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="976f0-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="976f0-110">**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="976f0-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="976f0-111">قد يفتقد القالب [ميزه](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="976f0-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="976f0-112">إذا كانت الميزة غير متوفرة للتنشيط في مجموعه الموقع الحالية ، لا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="976f0-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="976f0-113">تحقق لمعرفه ما إذا كانت إيه قوائم أو مكتبات تتجاوز [عتبه حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) للعناصر 5000 لان هذا يمكن ان يمنع إنشاء قالب موقع.</span><span class="sxs-lookup"><span data-stu-id="976f0-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="976f0-114">قد يستخدم الموقع موارد كثيره جدا التالي يتجاوز قالب الموقع حد 50 ميغابايت (MB).</span><span class="sxs-lookup"><span data-stu-id="976f0-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="976f0-115">هناك مشاكل في عرض البيانات من قائمه تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="976f0-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="976f0-116">لمزيد من المعلومات ، راجع [القائمة التي تم إنشاؤها بالقالب لا تعرض البيانات من قائمه البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="976f0-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="976f0-117">للحصول علي معلومات أكثر تفصيلا حول المشاكل والحلول الشائعة ، يرجى الرجوع إلى [قوالب المواقع وإنشاءها واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="976f0-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

