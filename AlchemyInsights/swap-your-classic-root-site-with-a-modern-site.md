---
title: تبديل الموقع الجذر الكلاسيكي باستخدام موقع حديث
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691166"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="d6359-102">تبديل الموقع الجذر الكلاسيكي باستخدام موقع حديث</span><span class="sxs-lookup"><span data-stu-id="d6359-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="d6359-103">إذا تم اعداد البيئة الخاصة بك قبل 2019 ابريل ، يمكنك تغيير الموقع الجذر إلى موقع حديث باستخدام Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d6359-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="d6359-104">إذا كان لديك موقع مختلف تريد استخدامه كموقع جذر ، يمكنك استبدال [(تبديل) الموقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) به.</span><span class="sxs-lookup"><span data-stu-id="d6359-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="d6359-105">استخدم [Invoke-سبوسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع الموقع مع موقع آخر اثناء أرشفه الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="d6359-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="d6359-106">متوفر لكل من موقع الفريق (غير متصل بمجموعه) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="d6359-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="d6359-107">سيتم تقديم قدرات اضافيه قريبا مما سيسمح لك بالاستمرار في استخدام المحتوي علي الموقع ، ولكن يمكنك تحويل الموقع الموجود إلى موقع اتصال.</span><span class="sxs-lookup"><span data-stu-id="d6359-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="d6359-108">سيتم عكس هذه الإمكانيات تدريجيا.</span><span class="sxs-lookup"><span data-stu-id="d6359-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="d6359-109">تابع التحقق من مركز الرسائل للحصول علي تحديثات.</span><span class="sxs-lookup"><span data-stu-id="d6359-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="d6359-110">المشاكل المعروفة في مواقع التبادل</span><span class="sxs-lookup"><span data-stu-id="d6359-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="d6359-111">قد يرجع الموقع الهدف الخطا "لم يتم العثور عليه" (HTTP 404) لفتره قصيرة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="d6359-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="d6359-112">سيحتاج المحتوي إلى ريكراوليد لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="d6359-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="d6359-113">لا توجد خطوه يدوية مطلوبه-سيتم القيام بذلك تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="d6359-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="d6359-114">يجب تصحيح اي شيء يعتمد علي ارتباطات "static" (مثل مزامنة الملفات وملفات OneNote) يدويا.</span><span class="sxs-lookup"><span data-stu-id="d6359-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="d6359-115">إذا كان الموقع المصدر عبارة عن موقع اخبار تنظيميه ، فقم بتحديث عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="d6359-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="d6359-116">احصل علي قائمه بكل مواقع الاخبار التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="d6359-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="d6359-117">قد يلزم التحقق من صحة مواقع Project Server لضمان انها لا تزال مقترنة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="d6359-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
