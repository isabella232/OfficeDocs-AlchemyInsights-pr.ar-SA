---
title: إصلاح تطبيقات Office عذرا ، لدينا رسالة مشاكل الخادم المؤقتة
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627977"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="acff5-102">إصلاح تطبيقات Office "عذرا ، لدينا مشاكل الخادم المؤقتة" رسالة</span><span class="sxs-lookup"><span data-stu-id="acff5-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="acff5-103">إذا تلقيت هذه الرسالة ، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="acff5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="acff5-104">تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="acff5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="acff5-105">راجع [عناوين url 365 Office ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="acff5-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="acff5-106">انتقل إلى **بدء** > **تشغيل**، ومن ثم اكتب **خدمات. msc**.</span><span class="sxs-lookup"><span data-stu-id="acff5-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="acff5-107">تاكد من تشغيل كافة الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="acff5-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="acff5-108">الاعداد التلقائي للاجهزه المتصلة بالشبكة</span><span class="sxs-lookup"><span data-stu-id="acff5-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="acff5-109">خدمه قائمه الشبكة</span><span class="sxs-lookup"><span data-stu-id="acff5-109">Network List Service</span></span>
    - <span data-ttu-id="acff5-110">التوعية بموقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="acff5-110">Network Location Awareness</span></span>
    - <span data-ttu-id="acff5-111">سجل احداث Windows</span><span class="sxs-lookup"><span data-stu-id="acff5-111">Windows Event Log</span></span>

<span data-ttu-id="acff5-112">إذا لم تكن أحدي هذه الخدمات قيد التشغيل ، فحاول تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="acff5-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="acff5-113">إذا كان لديك مشكله في بدء الخدمة ، قم بتشغيل الأمر التالي عن طريق فتح موجه الأوامر بأذونات مرتفعه:</span><span class="sxs-lookup"><span data-stu-id="acff5-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="acff5-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="acff5-114">**sfc /scannow**</span></span>

<span data-ttu-id="acff5-115">بعد انتهاء هذا الأمر ، قم باعاده تشغيل جهاز الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="acff5-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="acff5-116">للحصول علي معلومات مفصله ، راجع ["عذرا ، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مره أخرى لاحقا "خطا عند تنشيط Office من Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="acff5-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>