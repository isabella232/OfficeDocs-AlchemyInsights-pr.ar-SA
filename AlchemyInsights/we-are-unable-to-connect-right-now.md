---
title: مشكله التنشيط-تعذر الاتصال حاليا
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725970"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="22885-102">إصلاح تطبيقات Microsoft 365 "تعذر الاتصال الآن"</span><span class="sxs-lookup"><span data-stu-id="22885-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="22885-103">إذا تلقيت هذه الرسالة ، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="22885-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="22885-104">تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر الوصول إلى تطبيقات Microsoft 365 علي الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="22885-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="22885-105">راجع [نطاقات عناوين IP و url في Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="22885-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="22885-106">انتقل إلى **بدء**  >  **التشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="22885-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="22885-107">تاكد من تشغيل كل الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="22885-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="22885-108">اعداد تلقائي للاجهزه المتصلة بالشبكة</span><span class="sxs-lookup"><span data-stu-id="22885-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="22885-109">خدمه قائمه الشبكات</span><span class="sxs-lookup"><span data-stu-id="22885-109">Network List Service</span></span>
    - <span data-ttu-id="22885-110">معرفه موقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="22885-110">Network Location Awareness</span></span>
    - <span data-ttu-id="22885-111">سجل احداث Windows</span><span class="sxs-lookup"><span data-stu-id="22885-111">Windows Event Log</span></span>

<span data-ttu-id="22885-112">إذا لم يتم تشغيل أحدي هذه الخدمات ، فحاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="22885-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="22885-113">إذا كانت لديك مشكله في بدء تشغيل الخدمة ، فقم بتشغيل الأمر التالي بفتح موجه الأوامر باستخدام أذونات مرتفعه:</span><span class="sxs-lookup"><span data-stu-id="22885-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="22885-114">**/scannow sfc**</span><span class="sxs-lookup"><span data-stu-id="22885-114">**sfc /scannow**</span></span>

<span data-ttu-id="22885-115">بعد انتهاء هذا الأمر ، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="22885-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="22885-116">للحصول علي معلومات مفصله ، راجع ["عذرا ، يتعذر علينا الاتصال بحسابك. يرجى المحاولة مره أخرى لاحقا "عند تنشيط Office من Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="22885-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>