---
title: تصدير نتائج البحث في المحتوى/eDiscovery
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429245"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="d5353-102">تصدير نتائج البحث في المحتوى/eDiscovery</span><span class="sxs-lookup"><span data-stu-id="d5353-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="d5353-103">قد تحتاج إلى تصدير نتائج البحث إلى ملف PST (من البريد الإلكتروني) أو إلى مستندات Office الأصلية (من مواقع SharePoint و OneDrive for Business).</span><span class="sxs-lookup"><span data-stu-id="d5353-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="d5353-104">إذا كان الأمر كذلك، فتابع ما يلي:</span><span class="sxs-lookup"><span data-stu-id="d5353-104">If so, do the following:</span></span>

- <span data-ttu-id="d5353-105">تأكد من تعيين الأذونات الصحيحة للتصدير لحسابك.</span><span class="sxs-lookup"><span data-stu-id="d5353-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="d5353-106">لمزيد من المعلومات، راجع [الإذن "تعيين eDiscovery".](https://go.microsoft.com/fwlink/?linkid=2102406)</span><span class="sxs-lookup"><span data-stu-id="d5353-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="d5353-107">تأكد من أن الكمبيوتر الخاص بك قد تم فيه تحقيق [جميع المتطلبات الأساسية.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="d5353-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="d5353-108">لا يتم دعم كل المستعرضات، مثل Chrome.</span><span class="sxs-lookup"><span data-stu-id="d5353-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="d5353-109">للتصدير من البحث في المحتوى: أ.</span><span class="sxs-lookup"><span data-stu-id="d5353-109">To export from a Content Search: a.</span></span> <span data-ttu-id="d5353-110">انتقل إلى [مركز & الأمان وانقر](https://protection.office.com/contentsearch) فوق **"بحث"،** ثم حدد "البحث في **المحتوى".**</span><span class="sxs-lookup"><span data-stu-id="d5353-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="d5353-111">في صفحة **البحث في** المحتوى، حدد عملية بحث محفوظة.</span><span class="sxs-lookup"><span data-stu-id="d5353-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="d5353-112">ب.</span><span class="sxs-lookup"><span data-stu-id="d5353-112">b.</span></span> <span data-ttu-id="d5353-113">في الجزء "تفاصيل"، ضمن "تصدير **النتائج إلى جهاز كمبيوتر"،** حدد **"بدء التصدير".**</span><span class="sxs-lookup"><span data-stu-id="d5353-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="d5353-114">إذا كنت تقوم بتصدير أكثر من 100 علبة بريد، ستحتاج إلى استخدام PowerShell لتنزيل نتائج التصدير.</span><span class="sxs-lookup"><span data-stu-id="d5353-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="d5353-115">لمزيد من المعلومات، راجع تصدير النتائج من أكثر من [100 ألف علبة بريد.](https://go.microsoft.com/fwlink/?linkid=2143861)</span><span class="sxs-lookup"><span data-stu-id="d5353-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="d5353-116">لمعرفة المزيد، راجع ["تصدير نتائج البحث في المحتوى".](https://go.microsoft.com/fwlink/?linkid=2102118)</span><span class="sxs-lookup"><span data-stu-id="d5353-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>