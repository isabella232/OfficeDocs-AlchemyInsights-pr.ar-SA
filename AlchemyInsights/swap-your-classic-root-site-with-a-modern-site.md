---
title: مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث
ms.author: efrene
author: efrene
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
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749247"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="2d637-102">مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث</span><span class="sxs-lookup"><span data-stu-id="2d637-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="2d637-103">إذا تم إعداد البيئة الخاصة بك قبل أبريل عام 2019، يمكنك تغيير الموقع الجذر إلى موقع حديث باستخدام Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2d637-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="2d637-104">إذا كان لديك موقع مختلف تريد استخدامه كموقع جذر، يمكنك استبدال [(مبادلة) الموقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) معه.</span><span class="sxs-lookup"><span data-stu-id="2d637-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="2d637-105">استخدم [استدعاء SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لمبادلة موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="2d637-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="2d637-106">متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="2d637-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="2d637-107">سيتم تقديم قدرات إضافية قريباً تسمح لك بالاستمرار في استخدام المحتوى على الموقع، ولكن تحويل الموقع الحالي إلى موقع اتصال.</span><span class="sxs-lookup"><span data-stu-id="2d637-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="2d637-108">وسيتم نشر هذه القدرات تدريجيا.</span><span class="sxs-lookup"><span data-stu-id="2d637-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="2d637-109">تابع التحقق من معلومات مركز رسائل Office 365 عن التحديثات.</span><span class="sxs-lookup"><span data-stu-id="2d637-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="2d637-110">المشكلات المعروفة مع مواقع المبادلة</span><span class="sxs-lookup"><span data-stu-id="2d637-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="2d637-111">قد يرجع الموقع الهدف خطأ "لم يتم العثور عليها" (HTTP 404) لفترة قصيرة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="2d637-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="2d637-112">يجب إعادة تتبع ارتباطات المحتوى لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="2d637-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="2d637-113">لا توجد خطوة يدوية مطلوبة - سيتم ذلك تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="2d637-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="2d637-114">يجب تصحيح أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملف وملفات OneNote) يدويًا.</span><span class="sxs-lookup"><span data-stu-id="2d637-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="2d637-115">إذا كان الموقع المصدر موقع أخبار تنظيمية، فحدّث عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="2d637-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="2d637-116">الحصول على قائمة بجميع مواقع الأخبار التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="2d637-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="2d637-117">قد تحتاج مواقع خادم Project إلى التحقق من صحة للتأكد من أنها لا تزال مقترنة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="2d637-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





