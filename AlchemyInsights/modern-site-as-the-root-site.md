---
title: الموقع الحديث كالموقع الجذر
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666857"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="485e0-102">موقع حديث كموقع جذر</span><span class="sxs-lookup"><span data-stu-id="485e0-102">Modern site as root site</span></span>

<span data-ttu-id="485e0-103">لقد بدانا في نشر ميزه جديده ستسمح لك [بتبديل الموقع الجذر للموقع التقليدي مع موقع حديث](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="485e0-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="485e0-104">استخدم [Invoke-سبوسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع الموقع مع موقع آخر اثناء أرشفه الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="485e0-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="485e0-105">متوفر لكل من موقع الفريق (غير متصل بمجموعه) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="485e0-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="485e0-106">لا تحذف الموقع الجذر الكلاسيكي لإنشاء موقع اتصالات حديثه.</span><span class="sxs-lookup"><span data-stu-id="485e0-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="485e0-107">لا يتم دعم هذا الأمر بواسطة Microsoft.</span><span class="sxs-lookup"><span data-stu-id="485e0-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="485e0-108">سيؤدي حذف الموقع الجذر إلى جعل جميع مواقع SharePoint في مؤسستك غير قابله للوصول إلى كل المستخدمين ، حتى تقوم باستعادة الموقع أو إنشاء موقع جديد في عنوان URL نفسه.</span><span class="sxs-lookup"><span data-stu-id="485e0-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="485e0-109">سنقوم بالاتصال بهذه الميزة عبر مركز الرسائل.</span><span class="sxs-lookup"><span data-stu-id="485e0-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="485e0-110">يجب ان تتوقع ان تكون الميزة قيد التشغيل في نطاق المستاجر الخاص بك قريبا.</span><span class="sxs-lookup"><span data-stu-id="485e0-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="485e0-111">المشاكل المعروفة في مواقع التبادل</span><span class="sxs-lookup"><span data-stu-id="485e0-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="485e0-112">قد يرجع الموقع الهدف الخطا "لم يتم العثور عليه" (HTTP 404) لفتره قصيرة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="485e0-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="485e0-113">سيحتاج المحتوي إلى ريكراوليد لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="485e0-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="485e0-114">لا توجد خطوه يدوية مطلوبه هنا ، سيتم تنفيذ ذلك تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="485e0-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="485e0-115">يجب تصحيح اي شيء يعتمد علي ارتباطات "static" (مثل مزامنة الملفات وملفات OneNote) يدويا.</span><span class="sxs-lookup"><span data-stu-id="485e0-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="485e0-116">قد يلزم التحقق من صحة مواقع Project Server لضمان انها لا تزال مقترنة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="485e0-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
