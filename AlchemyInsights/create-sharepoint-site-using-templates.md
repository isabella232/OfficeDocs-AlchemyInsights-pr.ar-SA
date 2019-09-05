---
title: إنشاء موقع في SharePoint على الإنترنت
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755295"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="1ba82-102">إنشاء مواقع SharePoint باستخدام القوالب</span><span class="sxs-lookup"><span data-stu-id="1ba82-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="1ba82-103">قوالب موقع SharePoint هي تعريفات مصممة مسبقًا حول حاجة عمل معينة.</span><span class="sxs-lookup"><span data-stu-id="1ba82-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="1ba82-104">لمزيد من المعلومات، راجع [استخدام القوالب لإنشاء أنواع مختلفة من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="1ba82-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="1ba82-105">فيما يلي بعض المشكلات/الحلول الشائعة فيما يتعلق بحفظ موقع أو قائمة كقالب في Sharepoint عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="1ba82-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="1ba82-106">**زر حفظ قالب الموقع/القائمة غير متوفر أو مفقود**</span><span class="sxs-lookup"><span data-stu-id="1ba82-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="1ba82-107">سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب.</span><span class="sxs-lookup"><span data-stu-id="1ba82-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="1ba82-108">للاطلاع على الخطوات التفصيلية والأمثلة والاعتبارات، انظر</span><span class="sxs-lookup"><span data-stu-id="1ba82-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="1ba82-109">السماح بالبرنامج النصي المخصص أو منعه</span><span class="sxs-lookup"><span data-stu-id="1ba82-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="1ba82-110">الأمر حفظ الموقع كقالب غير معتمد ويمكن أن يسبب مشاكل على المواقع التي تستخدم بنية نشر خادم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1ba82-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="1ba82-111">**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="1ba82-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="1ba82-112">قد يفتقد القالب [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="1ba82-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="1ba82-113">إذا كانت الميزة غير متوفرة للتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="1ba82-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="1ba82-114">تحقق لمعرفة ما إذا كانت أية قوائم أو مكتبات تتجاوز [عتبة حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) للعناصر 5000 حيث أن هذا يمكن حظر إنشاء قالب موقع.</span><span class="sxs-lookup"><span data-stu-id="1ba82-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="1ba82-115">قد يستخدم الموقع موارد كثيرة جداً وبالتالي يتجاوز قالب الموقع حد 50 ميغا بايت.</span><span class="sxs-lookup"><span data-stu-id="1ba82-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="1ba82-116">توجد مشاكل في عرض البيانات من قائمة تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="1ba82-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="1ba82-117">لمزيد من المعلومات، راجع [القائمة التي تم إنشاؤها بواسطة القالب لا تعرض البيانات من قائمة البحث الصحيحة في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="1ba82-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="1ba82-118">لمزيد من المعلومات التفصيلية حول المشاكل والحلول الشائعة، الرجاء مراجعة [إنشاء قوالب المواقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="1ba82-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



