---
title: مشكلة التنشيط - يتعذر علينا الاتصال الآن
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806429"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b55dc-102">إصلاح رسالة تطبيقات Microsoft 365 "تعذر الاتصال الآن"</span><span class="sxs-lookup"><span data-stu-id="b55dc-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b55dc-103">إذا تلقيت هذه الرسالة، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="b55dc-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b55dc-104">تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b55dc-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b55dc-105">راجع [عناوين URL ونطاقات عناوين IP ل Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b55dc-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b55dc-106">انتقل إلى **بدء**  >  **تشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="b55dc-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b55dc-107">تأكد من تشغيل جميع الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="b55dc-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b55dc-108">الإعداد التلقائي للأجهزة المتصلة بالشبكة</span><span class="sxs-lookup"><span data-stu-id="b55dc-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b55dc-109">خدمة قائمة الشبكة</span><span class="sxs-lookup"><span data-stu-id="b55dc-109">Network List Service</span></span>
    - <span data-ttu-id="b55dc-110">الوعي بموقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="b55dc-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b55dc-111">سجل أحداث Windows</span><span class="sxs-lookup"><span data-stu-id="b55dc-111">Windows Event Log</span></span>

<span data-ttu-id="b55dc-112">إذا لم تكن إحدى هذه الخدمات قيد التشغيل، فحاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="b55dc-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b55dc-113">إذا كانت لديك مشكلة في بدء تشغيل الخدمة، فدير الأمر التالي بفتح موجه أوامر بأذونات مرتفعة:</span><span class="sxs-lookup"><span data-stu-id="b55dc-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b55dc-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="b55dc-114">**sfc /scannow**</span></span>

<span data-ttu-id="b55dc-115">بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="b55dc-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b55dc-116">للحصول على معلومات مفصلة، راجع ["عذرا، لا يمكننا الاتصال حسابك. يرجى المحاولة مرة أخرى لاحقا" عند تنشيط Office من Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b55dc-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>