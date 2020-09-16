---
title: إنشاء موقع في SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732198"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="f99bb-102">إنشاء مواقع SharePoint باستخدام القوالب</span><span class="sxs-lookup"><span data-stu-id="f99bb-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="f99bb-103">القدرة علي حفظ موقع كقالب غير معتمده مع الاتصال الحديث أو مواقع الفريق.</span><span class="sxs-lookup"><span data-stu-id="f99bb-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="f99bb-104">للحصول علي مزيد من المعلومات حول استخدام القوالب [، راجع حفظ موقع SharePoint وتنزيله وتحميله كقالب](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="f99bb-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="f99bb-105">اليك بعض المشاكل الشائعة/الحلول المتعلقة بحفظ موقع أو قائمه كقالب في Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="f99bb-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="f99bb-106">**الزر "حفظ قالب الموقع/القائمة" غير متوفر أو مفقود**</span><span class="sxs-lookup"><span data-stu-id="f99bb-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="f99bb-107">سيحتاج المسؤولون إلى السماح لبرنامج نصي مخصص بتمكين ميزات القالب.</span><span class="sxs-lookup"><span data-stu-id="f99bb-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="f99bb-108">للاطلاع علي الخطوات التفصيلية والامثله والاعتبارات</span><span class="sxs-lookup"><span data-stu-id="f99bb-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="f99bb-109">السماح بالبرامج النصية المخصصة أو منعها</span><span class="sxs-lookup"><span data-stu-id="f99bb-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="f99bb-110">الأمر "حفظ الموقع كقالب" غير معتمد وقد يؤدي إلى حدوث مشاكل في المواقع التي تستخدم البنية الاساسيه لنشر SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="f99bb-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="f99bb-111">**لا يمكن إنشاء قالب الموقع أو انه لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="f99bb-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="f99bb-112">قد لا يحتوي القالب علي [ميزه](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطها.</span><span class="sxs-lookup"><span data-stu-id="f99bb-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="f99bb-113">إذا لم تكن الميزة متوفرة للتنشيط في مجموعه المواقع المشتركة الحالية ، فلا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="f99bb-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="f99bb-114">التحقق لمعرفه ما إذا كانت هناك اي قوائم أو مكتبات تتجاوز [عتبه حدود طريقه عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) لعناصر 5000 بما انه بإمكانه حظر إنشاء قالب الموقع.</span><span class="sxs-lookup"><span data-stu-id="f99bb-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="f99bb-115">قد يستخدم الموقع عددا كبيرا جدا من الموارد ، التالي فان قالب الموقع يتجاوز الحد الأقصى ل50.</span><span class="sxs-lookup"><span data-stu-id="f99bb-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="f99bb-116">هناك مشاكل تعرض البيانات من قائمه تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="f99bb-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="f99bb-117">لمزيد من المعلومات ، راجع [القائمة التي تم إنشاؤها بالقوالب لا تعرض البيانات من قائمه البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="f99bb-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="f99bb-118">للحصول علي مزيد من المعلومات حول المشاكل والحلول الشائعة ، يرجى التحقق من [إنشاء قوالب الموقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="f99bb-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



