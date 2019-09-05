---
title: الموقع الحديث كموقع الجذر
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
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753891"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="e5b48-102">الموقع الحديث كموقع جذر</span><span class="sxs-lookup"><span data-stu-id="e5b48-102">Modern site as root site</span></span>

<span data-ttu-id="e5b48-103">لقد بدأنا في طرح ميزة جديدة من شأنها أن تسمح لك [لمبادلة موقعك الجذر الكلاسيكية مع موقع حديث.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="e5b48-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="e5b48-104">استخدم [استدعاء SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لمبادلة موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="e5b48-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e5b48-105">متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="e5b48-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="e5b48-106">لا تقم بحذف موقع الجذر الكلاسيكي لإنشاء موقع اتصال حديث.</span><span class="sxs-lookup"><span data-stu-id="e5b48-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="e5b48-107">هذا غير معتمد من قبل Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e5b48-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="e5b48-108">سيؤدي حذف الموقع الجذر إلى جعل كافة مواقع SharePoint في مؤسستك غير قابلة للوصول إلى كافة المستخدمين، حتى تقوم باستعادة الموقع أو إنشاء موقع جديد في نفس محدد موقع المعلومات .(</span><span class="sxs-lookup"><span data-stu-id="e5b48-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="e5b48-109">سنقوم بتوصيل هذه الميزة عبر مركز الرسائل.</span><span class="sxs-lookup"><span data-stu-id="e5b48-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="e5b48-110">يجب أن تتوقع الميزة ليتم تشغيلها في المستأجر الخاص بك قريباً.</span><span class="sxs-lookup"><span data-stu-id="e5b48-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e5b48-111">المشكلات المعروفة مع مواقع المبادلة</span><span class="sxs-lookup"><span data-stu-id="e5b48-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="e5b48-112">قد يرجع الموقع الهدف خطأ "لم يتم العثور عليها" (HTTP 404) لفترة قصيرة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="e5b48-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e5b48-113">يجب إعادة تتبع ارتباطات المحتوى لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="e5b48-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e5b48-114">لا توجد خطوة يدوية مطلوبة هنا، وسيتم ذلك تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="e5b48-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="e5b48-115">يجب تصحيح أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملف وملفات OneNote) يدويًا.</span><span class="sxs-lookup"><span data-stu-id="e5b48-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e5b48-116">قد تحتاج مواقع خادم Project إلى التحقق من صحة للتأكد من أنها لا تزال مقترنة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="e5b48-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
