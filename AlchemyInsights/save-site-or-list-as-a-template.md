---
title: حفظ الموقع أو القائمة كقالب
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752019"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="1233b-102">حفظ الموقع أو القائمة كقالب</span><span class="sxs-lookup"><span data-stu-id="1233b-102">Save site or list as a template</span></span>

<span data-ttu-id="1233b-103">قوالب موقع SharePoint هي تعريفات مصممة مسبقًا حول حاجة عمل معينة.</span><span class="sxs-lookup"><span data-stu-id="1233b-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="1233b-104">لمزيد من المعلومات، راجع [استخدام القوالب لإنشاء أنواع مختلفة من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="1233b-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="1233b-105">فيما يلي بعض المشكلات/الحلول الشائعة فيما يتعلق بحفظ موقع أو قائمة كقالب في SharePoint على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="1233b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="1233b-106">**زر حفظ قالب الموقع/القائمة غير متوفر أو مفقود**.</span><span class="sxs-lookup"><span data-stu-id="1233b-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="1233b-107">سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب.</span><span class="sxs-lookup"><span data-stu-id="1233b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="1233b-108">للحصول على خطوات تفصيلية وأمثلة واعتبارات راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="1233b-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="1233b-109">الأمر حفظ الموقع كقالب غير معتمد ويمكن أن يسبب مشاكل على المواقع التي تستخدم بنية نشر خادم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1233b-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="1233b-110">**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="1233b-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="1233b-111">قد يفتقد القالب [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="1233b-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="1233b-112">إذا كانت الميزة غير متوفرة للتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="1233b-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="1233b-113">تحقق لمعرفة ما إذا كانت أية قوائم أو مكتبات تتجاوز [عتبة حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) للعناصر 5000 حيث أن هذا يمكن حظر إنشاء قالب موقع.</span><span class="sxs-lookup"><span data-stu-id="1233b-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="1233b-114">قد يستخدم الموقع موارد كثيرة جداً وبالتالي يتجاوز قالب الموقع حد 50 ميغابايت (MB).</span><span class="sxs-lookup"><span data-stu-id="1233b-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="1233b-115">توجد مشاكل في عرض البيانات من قائمة تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="1233b-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="1233b-116">لمزيد من المعلومات، راجع [القائمة التي تم إنشاؤها بواسطة القالب لا تعرض البيانات من قائمة البحث الصحيحة في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="1233b-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="1233b-117">لمزيد من المعلومات التفصيلية حول المشاكل والحلول الشائعة يرجى الرجوع إليها، [إنشاء واستخدام قوالب الموقع](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="1233b-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

