---
title: إصلاح تطبيقات Office عذرا، نحن تواجه رسالة مشكلات خادم مؤقت
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764104"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="69767-102">إصلاح تطبيقات Office "عذراً، نحن نواجه مشاكل مؤقتة في الخادم"</span><span class="sxs-lookup"><span data-stu-id="69767-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="69767-103">إذا تلقيت هذه الرسالة، فجرّب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="69767-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="69767-104">تحقق من جدار الحماية وبرامج مكافحة الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="69767-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="69767-105">راجع [عناوين URL ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="69767-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="69767-106">انتقل إلى **بدء** > **تشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="69767-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="69767-107">تأكد من تشغيل كافة الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="69767-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="69767-108">الأجهزة المتصلة بالشبكة الإعداد التلقائي</span><span class="sxs-lookup"><span data-stu-id="69767-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="69767-109">خدمة قائمة الشبكة</span><span class="sxs-lookup"><span data-stu-id="69767-109">Network List Service</span></span>
    - <span data-ttu-id="69767-110">التوعية بموقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="69767-110">Network Location Awareness</span></span>
    - <span data-ttu-id="69767-111">سجل أحداث Windows</span><span class="sxs-lookup"><span data-stu-id="69767-111">Windows Event Log</span></span>

<span data-ttu-id="69767-112">إذا لم يتم تشغيل إحدى هذه الخدمات، حاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="69767-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="69767-113">إذا كان لديك مشكلة في بدء تشغيل الخدمة، قم بتشغيل الأمر التالي عن طريق فتح موجه أمر بأذونات مرتفعة:</span><span class="sxs-lookup"><span data-stu-id="69767-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="69767-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="69767-114">**sfc /scannow**</span></span>

<span data-ttu-id="69767-115">بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="69767-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="69767-116">للحصول على معلومات تفصيلية، راجع ["آسف، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="69767-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>