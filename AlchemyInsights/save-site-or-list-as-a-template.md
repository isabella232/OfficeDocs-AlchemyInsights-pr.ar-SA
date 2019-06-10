---
title: حفظ موقع أو قائمة موجودة كقالب
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770515"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="bc674-102">حفظ موقع أو قائمة موجودة كقالب</span><span class="sxs-lookup"><span data-stu-id="bc674-102">Save site or list as a template</span></span>

<span data-ttu-id="bc674-103">قوالب موقع SharePoint يتم التعريفات التي تم إنشاؤها مسبقاً مصممة على أساس حاجة عمل معينة.</span><span class="sxs-lookup"><span data-stu-id="bc674-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="bc674-104">لمزيد من المعلومات، راجع [استخدام قوالب لإنشاء أنواع مختلفة من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="bc674-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="bc674-105">فيما يلي بعض المشاكل/الحلول المشتركة فيما يتعلق بحفظ الموقع أو القائمة كقالب في SharePoint على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="bc674-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="bc674-106">**حفظ قائمة المواقع/قالب الزر غير متوفر أو مفقودة**.</span><span class="sxs-lookup"><span data-stu-id="bc674-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="bc674-107">ستحتاج إلى "نصي مخصص السماح" المسؤولين لتمكين ميزات قالب.</span><span class="sxs-lookup"><span data-stu-id="bc674-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="bc674-108">للحصول على خطوات تفصيلية وأمثلة واعتبارات راجع [السماح أو منع البرامج النصية المخصصة](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="bc674-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="bc674-109">حفظ الموقع كقالب أمر غير معتمد وقد يسبب مشاكل في المواقع التي تستخدم SharePoint Server نشر البنية التحتية.</span><span class="sxs-lookup"><span data-stu-id="bc674-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="bc674-110">**لا يمكن إنشاء قالب موقع أو لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="bc674-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="bc674-111">قد يفتقد [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) القالب وسوف يتم تنشيط.</span><span class="sxs-lookup"><span data-stu-id="bc674-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="bc674-112">الميزة غير متوفرة لتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="bc674-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="bc674-113">تحقق مما إذا كان أية قوائم أو مكتبات يتجاوز [عتبة حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) عناصر 5000 بذلك حظر إنشاء قالب موقع.</span><span class="sxs-lookup"><span data-stu-id="bc674-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="bc674-114">قد يكون الموقع يستخدم الكثير من الموارد وذلك قالب موقع يتجاوز حد 50 ميغابايت (MB).</span><span class="sxs-lookup"><span data-stu-id="bc674-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="bc674-115">توجد مشاكل في عرض بيانات من قائمة تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="bc674-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="bc674-116">لمزيد من المعلومات، راجع [إنشاء قالب قائمة إلى عرض بيانات من قائمة البحث الصحيحة في SharePoint على الإنترنت](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="bc674-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="bc674-117">للحصول على معلومات أكثر تفصيلاً عن المشاكل المشتركة والحلول الرجاء الإشارة، [إنشاء واستخدام قوالب الموقع](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="bc674-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

