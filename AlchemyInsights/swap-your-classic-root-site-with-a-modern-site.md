---
title: مبادله موقع الجذر الكلاسيكي الخاص بك مع موقع حديث
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042914"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="9a2ff-102">مبادله موقع الجذر الكلاسيكي الخاص بك مع موقع حديث</span><span class="sxs-lookup"><span data-stu-id="9a2ff-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="9a2ff-103">إذا تم اعداد البيئة الخاصة بك قبل 2019 ابريل ، يمكنك تغيير موقع الجذر إلى موقع حديث باستخدام Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9a2ff-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="9a2ff-104">إذا كان لديك موقع آخر تريد استخدامه كموقع الجذر الخاص بك ، يمكنك استبدال [(مبادله) موقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) معها.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="9a2ff-105">استخدام [استدعاء-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لمبادله موقع موقع مع موقع آخر اثناء أرشفه الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="9a2ff-106">متوفر لكل من موقع الفريق (غير متصل بمجموعه) وموقع الاتصالات.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="9a2ff-107">سيتم تقديم قدرات اضافيه قريبا من شانها ان تسمح لك للحفاظ علي استخدام المحتوي علي الموقع ، ولكن تحويل الموقع الحالي إلى موقع الاتصالات.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="9a2ff-108">سيتم نشر هذه القدرات تدريجيا.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="9a2ff-109">متابعه التحقق من مركز الرسائل 365 Office للحصول علي التحديثات.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="9a2ff-110">المشكلات المعروفة مع تبادل المواقع</span><span class="sxs-lookup"><span data-stu-id="9a2ff-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="9a2ff-111">قد يرجع الموقع الهدف خطا "لم يتم العثور علي" (HTTP 404) لفتره قصيرة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="9a2ff-112">سيحتاج المحتوي إلى أعاده التصنيف لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="9a2ff-113">لا توجد خطوه يدوية مطلوبه-سيتم ذلك تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="9a2ff-114">اي شيء يعتمد علي الارتباطات "الثابتة" (مثل مزامنة الملفات وملفات OneNote) سوف تحتاج إلى تصحيح يدويا.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="9a2ff-115">إذا كان موقع المصدر موقعا إخباريا تنظيميا ، فقم بتحديث عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="9a2ff-116">الحصول علي قائمه بجميع المواقع الاخباريه التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="9a2ff-117">قد تحتاج مواقع خادم Project إلى التحقق من صحتها للتاكد من انها لا تزال مقترنة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="9a2ff-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





