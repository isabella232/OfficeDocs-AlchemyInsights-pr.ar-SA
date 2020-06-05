---
title: مشكلة التنشيط - نحن غير قادرين على الاتصال الآن
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581862"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="e0cfb-102">إصلاح رسالة تطبيقات Microsoft 365 "نحن غير قادرين على الاتصال الآن"</span><span class="sxs-lookup"><span data-stu-id="e0cfb-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="e0cfb-103">إذا تلقيت هذه الرسالة، فجرّب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="e0cfb-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e0cfb-104">تحقق من جدار الحماية وبرامج مكافحة الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e0cfb-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e0cfb-105">راجع [عناوين URL لـ Microsoft ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e0cfb-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e0cfb-106">انتقل إلى **بدء**  >  **تشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="e0cfb-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e0cfb-107">تأكد من تشغيل كافة الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="e0cfb-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e0cfb-108">الأجهزة المتصلة بالشبكة الإعداد التلقائي</span><span class="sxs-lookup"><span data-stu-id="e0cfb-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e0cfb-109">خدمة قائمة الشبكة</span><span class="sxs-lookup"><span data-stu-id="e0cfb-109">Network List Service</span></span>
    - <span data-ttu-id="e0cfb-110">التوعية بموقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="e0cfb-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e0cfb-111">سجل أحداث Windows</span><span class="sxs-lookup"><span data-stu-id="e0cfb-111">Windows Event Log</span></span>

<span data-ttu-id="e0cfb-112">إذا لم يتم تشغيل إحدى هذه الخدمات، حاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="e0cfb-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e0cfb-113">إذا كان لديك مشكلة في بدء تشغيل الخدمة، قم بتشغيل الأمر التالي عن طريق فتح موجه أمر بأذونات مرتفعة:</span><span class="sxs-lookup"><span data-stu-id="e0cfb-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e0cfb-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="e0cfb-114">**sfc /scannow**</span></span>

<span data-ttu-id="e0cfb-115">بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="e0cfb-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e0cfb-116">للحصول على معلومات تفصيلية، راجع ["آسف، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط Office من Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e0cfb-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>