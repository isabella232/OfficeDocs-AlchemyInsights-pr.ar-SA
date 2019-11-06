---
title: 2609-الاحتفاظ-أو-ediscovery-عقد
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994040"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="0e133-102">غير قادر علي حذف العناصر في SharePoint علي الإنترنت أو اندريف للعمل</span><span class="sxs-lookup"><span data-stu-id="0e133-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="0e133-103">قد تكون أنت أو المستخدمين غير قادر علي حذف العناصر في SharePoint علي الإنترنت أو اندريف للعمل لأنه يتم تطبيق نهج استبقاء أو تسميه استبقاء أو احتجاز eDiscovery إلى موقع SharePoint من اندريف أو إلى عنصر معين.</span><span class="sxs-lookup"><span data-stu-id="0e133-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="0e133-104">ويشمل ذلك عدم القدرة علي حذف مستند أو إصدار مستند أو مجلد أو مكتبه مستندات أو قائمه أو تطبيق أو موقع أو مجموعه مواقع...</span><span class="sxs-lookup"><span data-stu-id="0e133-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="0e133-105">فيما يلي بعض الامثله علي رسائل الخطا التي قد تتلقاها عند محاولة حذف أحد العناصر التي يتم الاحتفاظ بها:</span><span class="sxs-lookup"><span data-stu-id="0e133-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="0e133-106">"لا يمكن حذف هذا الموقع لأنه مضمن في نهج احتجاز أو استبقاء eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="0e133-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="0e133-107">"يحتوي هذا الموقع علي نهج التوافق الذي تم تعيينه لحظر الحذف"</span><span class="sxs-lookup"><span data-stu-id="0e133-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="0e133-108">"نهج التوافق حاليا حظر حذف هذا الموقع"</span><span class="sxs-lookup"><span data-stu-id="0e133-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="0e133-109">"لا يمكن حذف مجموعه المواقع هذه لأنها تحتوي علي المواقع التي تم تضمينها في الاحتفاظ eDiscovery أو نهج الاستبقاء"</span><span class="sxs-lookup"><span data-stu-id="0e133-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="0e133-110">"لديك لحذف كافة العناصر الموجودة في هذا المجلد قبل حذف المجلد"</span><span class="sxs-lookup"><span data-stu-id="0e133-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="0e133-111">"لا يمكن حذف إصدارات هذا العنصر لأنه علي نهج الاحتجاز أو الاستبقاء"</span><span class="sxs-lookup"><span data-stu-id="0e133-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="0e133-112">"لا يمكن حذف العنصر اثناء الاحتجاز"</span><span class="sxs-lookup"><span data-stu-id="0e133-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="0e133-113">"التسمية التي يتم تطبيقها علي هذا العنصر يمنع تحريرها أو حذفها"</span><span class="sxs-lookup"><span data-stu-id="0e133-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="0e133-114">"لا يمكن حذف القائمة اثناء الاحتجاز أو نهج الاستبقاء"</span><span class="sxs-lookup"><span data-stu-id="0e133-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="0e133-115">"لا يمكن حذف القائمة إذا تم حظره أو إذا تم تطبيق نهج استبقاء عليه"</span><span class="sxs-lookup"><span data-stu-id="0e133-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="0e133-116">لحذف العناصر في أحد هذه السيناريوهات ، يجب أزاله نهج الاستبقاء أو تسميه الاستبقاء أو احتجاز eDiscovery (أو يجب استبعاد موقع من نهج الاستبقاء).</span><span class="sxs-lookup"><span data-stu-id="0e133-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="0e133-117">تحتاج إلى اما تعطيل أو استبعاد الاحتجاز الخاصة التي تسبب هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="0e133-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="0e133-118">بعد أزاله نهج الاستبقاء أو الاحتجاز ، قد يستغرق التغيير ما يصل إلى 24 ساعة حتى يتم تنفيذه.</span><span class="sxs-lookup"><span data-stu-id="0e133-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="0e133-119">للحصول علي معلومات حول ميزات الاستبقاء والاحتجاز المختلفة التي يمكن تطبيقها علي مواقع SharePoint وحسابات OneDrive ، راجع أحد المواضيع التالية.</span><span class="sxs-lookup"><span data-stu-id="0e133-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="0e133-120">نظره عامه علي سياسات الاستبقاء</span><span class="sxs-lookup"><span data-stu-id="0e133-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="0e133-121">نظره عامه حول تسميات الاستبقاء</span><span class="sxs-lookup"><span data-stu-id="0e133-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="0e133-122">أداره التعليقات في eDiscovery المتقدم</span><span class="sxs-lookup"><span data-stu-id="0e133-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="0e133-123">eDiscovery يحمل</span><span class="sxs-lookup"><span data-stu-id="0e133-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="0e133-124">سياسات الإغلاق والحذف للمواقع القديمة</span><span class="sxs-lookup"><span data-stu-id="0e133-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
