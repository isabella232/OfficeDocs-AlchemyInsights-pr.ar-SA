---
title: الموقع الحديث كموقع الجذر
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713778"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="37895-102">الموقع الحديث كموقع الجذر</span><span class="sxs-lookup"><span data-stu-id="37895-102">Modern site as root site</span></span>

<span data-ttu-id="37895-103">لقد بدأنا في طرح ميزة جديدة من شأنها أن تسمح لك [لمبادلة موقع جذر الموقع الكلاسيكي الخاص بك مع موقع حديث.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="37895-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="37895-104">استخدم [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي.</span><span class="sxs-lookup"><span data-stu-id="37895-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="37895-105">متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="37895-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="37895-106">لا تقم بحذف موقع الجذر الكلاسيكي الخاص بك لإنشاء موقع اتصال حديث.</span><span class="sxs-lookup"><span data-stu-id="37895-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="37895-107">هذا غير معتمد من قبل Microsoft.</span><span class="sxs-lookup"><span data-stu-id="37895-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="37895-108">سيؤدي حذف موقع الجذر إلى جعل جميع مواقع SharePoint في مؤسستك غير قابلة للوصول إلى جميع المستخدمين، حتى تقوم باستعادة الموقع أو إنشاء موقع جديد في نفس عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="37895-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="37895-109">سنقوم بتوصيل هذه الميزة عبر مركز الرسائل.</span><span class="sxs-lookup"><span data-stu-id="37895-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="37895-110">يجب أن تتوقع تشغيل الميزة في المستأجر الخاص بك قريباً.</span><span class="sxs-lookup"><span data-stu-id="37895-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="37895-111">المشكلات المعروفة مع مواقع المبادلة</span><span class="sxs-lookup"><span data-stu-id="37895-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="37895-112">قد يرجع الموقع المستهدف خطأ "لم يتم العثور عليه" (HTTP 404) لفترة قصيرة من الزمن.</span><span class="sxs-lookup"><span data-stu-id="37895-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="37895-113">يجب إعادة كتابة المحتوى لتحديث فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="37895-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="37895-114">لا توجد خطوة يدوية مطلوبة هنا ، وسيتم ذلك تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="37895-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="37895-115">أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملفات وملفات OneNote) سيحتاج إلى تصحيح يدويًا.</span><span class="sxs-lookup"><span data-stu-id="37895-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="37895-116">قد تحتاج مواقع Project Server إلى التحقق من صحتها للتأكد من أنها لا تزال مقترنة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="37895-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
