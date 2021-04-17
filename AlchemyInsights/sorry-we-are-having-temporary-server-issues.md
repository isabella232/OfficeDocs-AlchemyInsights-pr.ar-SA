---
title: تصحيح تطبيقات Microsoft 365 عذرا، لدينا رسالة مشاكل مؤقتة في الخادم
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835258"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="c1ca1-102">تصحيح رسالة تطبيقات Microsoft 365 "عذرا، نحن نواجه مشاكل مؤقتة في الخادم"</span><span class="sxs-lookup"><span data-stu-id="c1ca1-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="c1ca1-103">إذا تلقيت هذه الرسالة، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="c1ca1-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="c1ca1-104">تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c1ca1-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="c1ca1-105">راجع [عناوين URL ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="c1ca1-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="c1ca1-106">انتقل إلى **بدء**  >  **تشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="c1ca1-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="c1ca1-107">تأكد من تشغيل جميع الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="c1ca1-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="c1ca1-108">الإعداد التلقائي للأجهزة المتصلة بالشبكة</span><span class="sxs-lookup"><span data-stu-id="c1ca1-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="c1ca1-109">خدمة قائمة الشبكة</span><span class="sxs-lookup"><span data-stu-id="c1ca1-109">Network List Service</span></span>
    - <span data-ttu-id="c1ca1-110">الوعي بموقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="c1ca1-110">Network Location Awareness</span></span>
    - <span data-ttu-id="c1ca1-111">سجل أحداث Windows</span><span class="sxs-lookup"><span data-stu-id="c1ca1-111">Windows Event Log</span></span>

<span data-ttu-id="c1ca1-112">إذا لم تكن إحدى هذه الخدمات قيد التشغيل، فحاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="c1ca1-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="c1ca1-113">إذا كانت لديك مشكلة في بدء تشغيل الخدمة، فدير الأمر التالي بفتح موجه أوامر بأذونات مرتفعة:</span><span class="sxs-lookup"><span data-stu-id="c1ca1-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="c1ca1-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="c1ca1-114">**sfc /scannow**</span></span>

<span data-ttu-id="c1ca1-115">بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="c1ca1-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="c1ca1-116">للحصول على معلومات مفصلة، راجع ["عذرا، لا يمكننا الاتصال حسابك. يرجى المحاولة مرة أخرى لاحقا" عند تنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="c1ca1-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>