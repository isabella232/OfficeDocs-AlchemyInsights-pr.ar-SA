---
title: مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741531"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="3b696-102">مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث</span><span class="sxs-lookup"><span data-stu-id="3b696-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="3b696-103">إذا تم إعداد البيئة الخاصة بك قبل أبريل 2019، يمكنك تغيير موقع الجذر الخاص بك إلى موقع حديث باستخدام Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3b696-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="3b696-104">إذا كان لديك موقع مختلف تريد استخدامه كموقع الجذر الخاص بك، يمكنك استبدال [(مبادلة) موقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) معه.</span><span class="sxs-lookup"><span data-stu-id="3b696-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="3b696-105">استخدم [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="3b696-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="3b696-106">متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="3b696-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="3b696-107">سيتم تقديم قدرات إضافية قريبًا تسمح لك بمواصلة استخدام المحتوى على الموقع ، ولكن تحويل الموقع الحالي إلى موقع اتصال.</span><span class="sxs-lookup"><span data-stu-id="3b696-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="3b696-108">وسيتم نشر هذه القدرات تدريجيا.</span><span class="sxs-lookup"><span data-stu-id="3b696-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="3b696-109">متابعة التحقق من مركز الرسائل للحصول على التحديثات.</span><span class="sxs-lookup"><span data-stu-id="3b696-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="3b696-110">المشكلات المعروفة مع مواقع المبادلة</span><span class="sxs-lookup"><span data-stu-id="3b696-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="3b696-111">قد يرجع الموقع المستهدف خطأ "لم يتم العثور عليه" (HTTP 404) لفترة قصيرة من الزمن.</span><span class="sxs-lookup"><span data-stu-id="3b696-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="3b696-112">يجب إعادة كتابة المحتوى لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="3b696-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="3b696-113">لا توجد خطوة يدوية مطلوبة - سيتم ذلك تلقائيًا.</span><span class="sxs-lookup"><span data-stu-id="3b696-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="3b696-114">أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملفات وملفات OneNote) سيحتاج إلى تصحيح يدويًا.</span><span class="sxs-lookup"><span data-stu-id="3b696-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="3b696-115">إذا كان موقع المصدر موقعًا إخباريًا تنظيميًا، فقم بتحديث عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="3b696-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="3b696-116">احصل على قائمة بجميع المواقع الإخبارية التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="3b696-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="3b696-117">قد تحتاج مواقع Project Server إلى التحقق من صحتها للتأكد من أنها لا تزال مقترنة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="3b696-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
