---
title: إنشاء موقع في SharePoint عبر إنترنت
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753694"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="56bd1-102">إنشاء مواقع SharePoint باستخدام القوالب</span><span class="sxs-lookup"><span data-stu-id="56bd1-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="56bd1-103">قوالب موقع SharePoint يتم التعريفات التي تم إنشاؤها مسبقاً مصممة على أساس حاجة عمل معينة.</span><span class="sxs-lookup"><span data-stu-id="56bd1-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="56bd1-104">لمزيد من المعلومات، راجع [استخدام قوالب لإنشاء أنواع مختلفة من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="56bd1-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="56bd1-105">فيما يلي بعض المشاكل/الحلول المشتركة فيما يتعلق بحفظ الموقع أو القائمة كقالب في Sharepoint على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="56bd1-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="56bd1-106">**زر قالب القائمة/موقع الحفظ غير متوفرة أو مفقودة**</span><span class="sxs-lookup"><span data-stu-id="56bd1-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="56bd1-107">ستحتاج إلى "نصي مخصص السماح" المسؤولين لتمكين ميزات قالب.</span><span class="sxs-lookup"><span data-stu-id="56bd1-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="56bd1-108">راجع للحصول على خطوات تفصيلية أمثلة واعتبارات</span><span class="sxs-lookup"><span data-stu-id="56bd1-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="56bd1-109">تسمح أو تمنع البرامج النصية المخصصة</span><span class="sxs-lookup"><span data-stu-id="56bd1-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="56bd1-110">حفظ الموقع كقالب أمر غير معتمد وقد يسبب مشاكل في المواقع التي تستخدم SharePoint Server نشر البنية التحتية.</span><span class="sxs-lookup"><span data-stu-id="56bd1-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="56bd1-111">لا يمكن إنشاء قالب موقع أو لا يعمل بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="56bd1-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="56bd1-112">قد يفتقد [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) القالب وسوف يتم تنشيط.</span><span class="sxs-lookup"><span data-stu-id="56bd1-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="56bd1-113">الميزة غير متوفرة لتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="56bd1-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="56bd1-114">تحقق مما إذا كان أية قوائم أو مكتبات يتجاوز [عتبة حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) عناصر 5000 بذلك حظر إنشاء قالب موقع.</span><span class="sxs-lookup"><span data-stu-id="56bd1-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="56bd1-115">قد يكون الموقع يستخدم الكثير من الموارد وذلك قالب موقع يتجاوز حد 50 ميغا بايت.</span><span class="sxs-lookup"><span data-stu-id="56bd1-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="56bd1-116">توجد مشاكل في عرض بيانات من قائمة تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="56bd1-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="56bd1-117">لمزيد من المعلومات، راجع [إنشاء قالب قائمة إلى عرض بيانات من قائمة البحث الصحيحة في SharePoint على الإنترنت](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="56bd1-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="56bd1-118">للحصول على معلومات أكثر تفصيلاً عن المشكلات والحلول الشائعة، الرجاء التحقق من [إنشاء واستخدام قوالب الموقع](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="56bd1-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



