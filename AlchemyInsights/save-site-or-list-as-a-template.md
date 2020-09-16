---
title: حفظ الموقع أو القائمة كقالب
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727518"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="986a6-102">حفظ الموقع أو القائمة كقالب</span><span class="sxs-lookup"><span data-stu-id="986a6-102">Save site or list as a template</span></span>

<span data-ttu-id="986a6-103">قوالب موقع SharePoint هي تعريفات منشاه مسبقا التي تم تصميمها حول احتياجات عمل معينه.</span><span class="sxs-lookup"><span data-stu-id="986a6-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="986a6-104">لمزيد من المعلومات ، راجع [استخدام القوالب لإنشاء أنواع مختلفه من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="986a6-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="986a6-105">اليك بعض المشاكل الشائعة/الحلول المتعلقة بحفظ موقع أو قائمه كقالب في SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="986a6-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="986a6-106">**الزر "حفظ قالب الموقع/القائمة" غير متوفر أو مفقود**.</span><span class="sxs-lookup"><span data-stu-id="986a6-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="986a6-107">سيحتاج المسؤولون إلى السماح لبرنامج نصي مخصص بتمكين ميزات القالب.</span><span class="sxs-lookup"><span data-stu-id="986a6-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="986a6-108">للاطلاع علي الخطوات التفصيلية والامثله والاعتبارات ، راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="986a6-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="986a6-109">الأمر "حفظ الموقع كقالب" غير معتمد وقد يؤدي إلى حدوث مشاكل في المواقع التي تستخدم البنية الاساسيه لنشر SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="986a6-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="986a6-110">**لا يمكن إنشاء قالب الموقع أو انه لا يعمل بشكل صحيح**</span><span class="sxs-lookup"><span data-stu-id="986a6-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="986a6-111">قد لا يحتوي القالب علي [ميزه](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطها.</span><span class="sxs-lookup"><span data-stu-id="986a6-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="986a6-112">إذا لم تكن الميزة متوفرة للتنشيط في مجموعه المواقع المشتركة الحالية ، فلا يمكنك استخدام قالب الموقع لإنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="986a6-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="986a6-113">التحقق لمعرفه ما إذا كانت هناك اي قوائم أو مكتبات تتجاوز [عتبه حدود طريقه عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) لعناصر 5000 بما انه بإمكانه حظر إنشاء قالب الموقع.</span><span class="sxs-lookup"><span data-stu-id="986a6-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="986a6-114">قد يستخدم الموقع عددا كبيرا جدا من الموارد ، التالي فان قالب الموقع يتجاوز الحد الأقصى ل50 ميغابايت.</span><span class="sxs-lookup"><span data-stu-id="986a6-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="986a6-115">هناك مشاكل تعرض البيانات من قائمه تستخدم عمود بحث.</span><span class="sxs-lookup"><span data-stu-id="986a6-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="986a6-116">لمزيد من المعلومات ، راجع [القائمة التي تم إنشاؤها بالقوالب لا تعرض البيانات من قائمه البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="986a6-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="986a6-117">للحصول علي مزيد من المعلومات حول المشاكل والحلول الشائعة ، يرجى الاشاره إلى [قوالب الموقع وإنشاءها واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="986a6-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

