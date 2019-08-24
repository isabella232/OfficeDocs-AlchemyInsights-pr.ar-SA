---
title: حديث الموقع الجذر
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620746"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="9fe6e-102">موقع الحديثة كالموقع الجذر</span><span class="sxs-lookup"><span data-stu-id="9fe6e-102">Modern site as root site</span></span>

<span data-ttu-id="9fe6e-103">وقد بدأنا للتمهيد ميزة جديدة تسمح لك لتبديل موقع جذر الموقع التقليدي بموقع حديثة.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="9fe6e-104">استخدام [استدعاء سبوسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موضع موقع بموقع آخر أثناء الأرشفة الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="9fe6e-105">يتوفر لكل موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="9fe6e-106">لا تقم بحذف الموقع الجذر الكلاسيكية لإنشاء "موقع الاتصالات" الحديثة.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="9fe6e-107">وهذا غير معتمد من قبل Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="9fe6e-108">حذف الموقع الجذر سيجعل كافة مواقع SharePoint في المؤسسة الخاصة بك غير متاحة لكافة المستخدمين، حتى يمكنك استعادة الموقع أو إنشاء موقع جديد على نفس العنوان.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="9fe6e-109">أننا سوف يمكن الاتصال هذه الميزة عبر مركز الرسائل.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="9fe6e-110">يجب أن تتوقع ميزة تشغيل في جهاز المستأجر بعد قليل.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="9fe6e-111">المشكلات المعروفة المتعلقة بتبادل المواقع</span><span class="sxs-lookup"><span data-stu-id="9fe6e-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="9fe6e-112">موقع الهدف قد بإرجاع خطأ (HTTP 404) "لم يتم العثور على" لفترة قصيرة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="9fe6e-113">أن محتوى تتبع الارتباطات من جديد لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="9fe6e-114">خطوة اليدوية ليست مطلوبة هنا، هذا يتم إنجازه تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="9fe6e-115">أي شيء يعتمد على روابط "ثابتة" (مثل ملفات OneNote ومزامنة الملفات) ستحتاج إلى تصحيحه يدوياً.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="9fe6e-116">قد تحتاج مواقع المشروع على الخادم التحقق من صحة للتأكد من أنها لا يزال مرتبطاً بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="9fe6e-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
