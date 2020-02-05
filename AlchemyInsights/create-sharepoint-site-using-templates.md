---
title: إنشاء موقع في SharePoint Online
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
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770410"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="44c21-102">إنشاء مواقع SharePoint باستخدام القوالب</span><span class="sxs-lookup"><span data-stu-id="44c21-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="44c21-103">لا يتم دعم القدرة على حفظ موقع كقالب مع مواقع الاتصال أو الفريق الحديثة.</span><span class="sxs-lookup"><span data-stu-id="44c21-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="44c21-104">لمزيد من المعلومات حول استخدام القوالب راجع [حفظ موقع SharePoint وتنزيله وتحميله كقالب](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="44c21-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="44c21-105">فيما يلي بعض المشكلات/الحلول الشائعة فيما يتعلق بحفظ موقع أو قائمة كقالب في Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="44c21-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="44c21-106">**حفظ زر قالب الموقع/القائمة غير متوفر أو مفقود**</span><span class="sxs-lookup"><span data-stu-id="44c21-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="44c21-107">سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب.</span><span class="sxs-lookup"><span data-stu-id="44c21-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="44c21-108">للحصول على خطوات مفصلة، أمثلة واعتبارات انظر</span><span class="sxs-lookup"><span data-stu-id="44c21-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="44c21-109">السماح بالبرنامج النصي المخصص أو منعه</span><span class="sxs-lookup"><span data-stu-id="44c21-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="44c21-110">موقع الحفظ كأمر قالب غير معتمد ويمكن أن يسبب مشاكل على المواقع التي تستخدم البنية التحتية لنشر خادم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="44c21-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="44c21-111">**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="44c21-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="44c21-112">قد يفتقد القالب [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="44c21-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="44c21-113">إذا لم تكن الميزة متوفرة للتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="44c21-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="44c21-114">تحقق لمعرفة ما إذا كانت أي قوائم أو مكتبات تتجاوز [حد عرض القائمة الحد الأدنى](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) من 5000 عنصر حيث يمكن حظر إنشاء قالب موقع.</span><span class="sxs-lookup"><span data-stu-id="44c21-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="44c21-115">قد يستخدم الموقع موارد كثيرة جداً وبالتالي يتجاوز قالب الموقع حد 50 ميغابايت.</span><span class="sxs-lookup"><span data-stu-id="44c21-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="44c21-116">هناك مشاكل في عرض البيانات من قائمة تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="44c21-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="44c21-117">لمزيد من المعلومات، راجع [القائمة التي تم إنشاؤها بواسطة القالب لا تعرض البيانات من قائمة البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="44c21-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="44c21-118">لمزيد من المعلومات التفصيلية حول المشاكل والحلول الشائعة، يرجى التحقق من [إنشاء واستخدام قوالب الموقع.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="44c21-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



