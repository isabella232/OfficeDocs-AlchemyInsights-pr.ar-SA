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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716159"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="6bffe-102">إصلاح رسالة تطبيقات Office "نحن غير قادرين على الاتصال الآن"</span><span class="sxs-lookup"><span data-stu-id="6bffe-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="6bffe-103">إذا تلقيت هذه الرسالة، فجرّب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="6bffe-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6bffe-104">تحقق من جدار الحماية وبرامج مكافحة الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="6bffe-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="6bffe-105">راجع [عناوين URL لـ Microsoft ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6bffe-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="6bffe-106">انتقل إلى **بدء** > **تشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="6bffe-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="6bffe-107">تأكد من تشغيل كافة الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="6bffe-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="6bffe-108">الأجهزة المتصلة بالشبكة الإعداد التلقائي</span><span class="sxs-lookup"><span data-stu-id="6bffe-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="6bffe-109">خدمة قائمة الشبكة</span><span class="sxs-lookup"><span data-stu-id="6bffe-109">Network List Service</span></span>
    - <span data-ttu-id="6bffe-110">التوعية بموقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="6bffe-110">Network Location Awareness</span></span>
    - <span data-ttu-id="6bffe-111">سجل أحداث Windows</span><span class="sxs-lookup"><span data-stu-id="6bffe-111">Windows Event Log</span></span>

<span data-ttu-id="6bffe-112">إذا لم يتم تشغيل إحدى هذه الخدمات، حاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="6bffe-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="6bffe-113">إذا كان لديك مشكلة في بدء تشغيل الخدمة، قم بتشغيل الأمر التالي عن طريق فتح موجه أمر بأذونات مرتفعة:</span><span class="sxs-lookup"><span data-stu-id="6bffe-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="6bffe-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="6bffe-114">**sfc /scannow**</span></span>

<span data-ttu-id="6bffe-115">بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="6bffe-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="6bffe-116">للحصول على معلومات تفصيلية، راجع ["آسف، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط Office من Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="6bffe-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>