---
title: تبديل الموقع الجذر التقليدية مع موقع الحديثة
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501066"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="1ff15-102">تبديل الموقع الجذر التقليدية مع موقع الحديثة</span><span class="sxs-lookup"><span data-stu-id="1ff15-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="1ff15-103">إذا تم إعداد البيئة الخاصة بك قبل نيسان/أبريل عام 2019، يمكنك تغيير الموقع الجذر الخاص بك إلى موقع حديثة باستخدام Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1ff15-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="1ff15-104">إذا كان لديك موقع آخر تريد استخدامه كالموقع الجذر الخاص بك، يمكنك استبدال (ترحيل) الجذر الموقع معها.</span><span class="sxs-lookup"><span data-stu-id="1ff15-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="1ff15-105">استخدام [استدعاء سبوسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موضع موقع بموقع آخر أثناء الأرشفة الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="1ff15-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1ff15-106">يتوفر لكل موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="1ff15-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="1ff15-107">تم توفير قدرات إضافية قريبا التي تسمح لك للاحتفاظ باستخدام المحتوى على الموقع، ولكن تحويل موقع موجود إلى موقع اتصال.</span><span class="sxs-lookup"><span data-stu-id="1ff15-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="1ff15-108">هذه القدرات سيبدأ تدريجيا.</span><span class="sxs-lookup"><span data-stu-id="1ff15-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="1ff15-109">متابعة للتحقق من مركز الرسائل Office 365 للتحديثات.</span><span class="sxs-lookup"><span data-stu-id="1ff15-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1ff15-110">المشكلات المعروفة المتعلقة بتبادل المواقع</span><span class="sxs-lookup"><span data-stu-id="1ff15-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="1ff15-111">موقع الهدف قد بإرجاع خطأ (HTTP 404) "لم يتم العثور على" لفترة قصيرة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="1ff15-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1ff15-112">أن محتوى تتبع الارتباطات من جديد لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="1ff15-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1ff15-113">خطوة ليست اليدوية المطلوبة-هذا يتم إنجازه تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="1ff15-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="1ff15-114">أي شيء يعتمد على روابط "ثابتة" (مثل ملفات OneNote ومزامنة الملفات) ستحتاج إلى تصحيحه يدوياً.</span><span class="sxs-lookup"><span data-stu-id="1ff15-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1ff15-115">إذا كان موقع المصدر موقع أخبار المؤسسة، تحديث عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="1ff15-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="1ff15-116">الحصول على قائمة بكافة مواقع أخبار المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="1ff15-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="1ff15-117">قد تحتاج مواقع المشروع على الخادم التحقق من صحة للتأكد من أنها لا يزال مرتبطاً بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="1ff15-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





