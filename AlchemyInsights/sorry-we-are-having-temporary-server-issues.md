---
title: إصلاح تطبيقات Microsoft 365 عذرا، نحن تواجه رسالة مشاكل الخادم المؤقت
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582690"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="68f4f-102">إصلاح تطبيقات Microsoft 365 "عذراً، نحن نواجه مشاكل مؤقتة في الخادم"</span><span class="sxs-lookup"><span data-stu-id="68f4f-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="68f4f-103">إذا تلقيت هذه الرسالة، فجرّب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="68f4f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="68f4f-104">تحقق من جدار الحماية وبرامج مكافحة الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="68f4f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="68f4f-105">راجع [عناوين URL ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="68f4f-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="68f4f-106">انتقل إلى **بدء**  >  **تشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="68f4f-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="68f4f-107">تأكد من تشغيل كافة الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="68f4f-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="68f4f-108">الأجهزة المتصلة بالشبكة الإعداد التلقائي</span><span class="sxs-lookup"><span data-stu-id="68f4f-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="68f4f-109">خدمة قائمة الشبكة</span><span class="sxs-lookup"><span data-stu-id="68f4f-109">Network List Service</span></span>
    - <span data-ttu-id="68f4f-110">التوعية بموقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="68f4f-110">Network Location Awareness</span></span>
    - <span data-ttu-id="68f4f-111">سجل أحداث Windows</span><span class="sxs-lookup"><span data-stu-id="68f4f-111">Windows Event Log</span></span>

<span data-ttu-id="68f4f-112">إذا لم يتم تشغيل إحدى هذه الخدمات، حاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="68f4f-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="68f4f-113">إذا كان لديك مشكلة في بدء تشغيل الخدمة، قم بتشغيل الأمر التالي عن طريق فتح موجه أمر بأذونات مرتفعة:</span><span class="sxs-lookup"><span data-stu-id="68f4f-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="68f4f-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="68f4f-114">**sfc /scannow**</span></span>

<span data-ttu-id="68f4f-115">بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="68f4f-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="68f4f-116">للحصول على معلومات تفصيلية، راجع ["آسف، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="68f4f-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>