---
title: إنشاء موقع في SharePoint علي الإنترنت
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052456"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="383b4-102">إنشاء مواقع SharePoint باستخدام القوالب</span><span class="sxs-lookup"><span data-stu-id="383b4-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="383b4-103">قوالب موقع SharePoint هي تعريفات تم بناؤها مسبقا مصممه حول حاجه عمل معينه.</span><span class="sxs-lookup"><span data-stu-id="383b4-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="383b4-104">لمزيد من المعلومات ، راجع [استخدام قوالب لإنشاء أنواع مختلفه من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="383b4-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="383b4-105">فيما يلي بعض المشكلات/الحلول الشائعة المتعلقة بحفظ موقع أو قائمه كقالب في Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="383b4-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="383b4-106">**زر حفظ قالب الموقع/القائمة غير متوفر أو مفقود**</span><span class="sxs-lookup"><span data-stu-id="383b4-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="383b4-107">سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب.</span><span class="sxs-lookup"><span data-stu-id="383b4-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="383b4-108">وللاطلاع علي الخطوات التفصيلية ، انظر الامثله والاعتبارات</span><span class="sxs-lookup"><span data-stu-id="383b4-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="383b4-109">السماح بالبرنامج النصي المخصص أو منعه</span><span class="sxs-lookup"><span data-stu-id="383b4-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="383b4-110">الأمر حفظ الموقع كقالب غير معتمد ويمكن ان يسبب مشاكل علي المواقع التي تستخدم البنية الاساسيه للنشر خادم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="383b4-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="383b4-111">**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="383b4-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="383b4-112">قد يفتقد القالب [ميزه](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="383b4-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="383b4-113">إذا كانت الميزة غير متوفرة للتنشيط في مجموعه الموقع الحالية ، لا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="383b4-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="383b4-114">تحقق لمعرفه ما إذا كانت إيه قوائم أو مكتبات تتجاوز [عتبه حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) للعناصر 5000 لان هذا يمكن ان يمنع إنشاء قالب موقع.</span><span class="sxs-lookup"><span data-stu-id="383b4-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="383b4-115">قد يستخدم الموقع موارد كثيره جدا التالي يتجاوز قالب الموقع حد 50 ميغابايت.</span><span class="sxs-lookup"><span data-stu-id="383b4-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="383b4-116">هناك مشاكل في عرض البيانات من قائمه تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="383b4-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="383b4-117">لمزيد من المعلومات ، راجع [القائمة التي تم إنشاؤها بالقالب لا تعرض البيانات من قائمه البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="383b4-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="383b4-118">للحصول علي معلومات أكثر تفصيلا حول المشاكل والحلول الشائعة ، الرجاء التحقق من [إنشاء قوالب الموقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="383b4-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



