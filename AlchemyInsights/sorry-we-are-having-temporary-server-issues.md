---
title: إصلاح تطبيقات Microsoft 365 عذرا ، نواجه رسالة مشاكل مؤقته في الخادم
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758232"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="180a4-102">إصلاح تطبيقات Microsoft 365 "عذرا ، فنحن نواجه مشكلات مؤقته في الخادم"</span><span class="sxs-lookup"><span data-stu-id="180a4-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="180a4-103">إذا تلقيت هذه الرسالة ، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="180a4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="180a4-104">تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر الوصول إلى تطبيقات Microsoft 365 علي الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="180a4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="180a4-105">راجع [نطاقات عناوين IP و url](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="180a4-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="180a4-106">انتقل إلى **بدء**  >  **التشغيل**، ثم اكتب **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="180a4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="180a4-107">تاكد من تشغيل كل الخدمات التالية:</span><span class="sxs-lookup"><span data-stu-id="180a4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="180a4-108">اعداد تلقائي للاجهزه المتصلة بالشبكة</span><span class="sxs-lookup"><span data-stu-id="180a4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="180a4-109">خدمه قائمه الشبكات</span><span class="sxs-lookup"><span data-stu-id="180a4-109">Network List Service</span></span>
    - <span data-ttu-id="180a4-110">معرفه موقع الشبكة</span><span class="sxs-lookup"><span data-stu-id="180a4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="180a4-111">سجل احداث Windows</span><span class="sxs-lookup"><span data-stu-id="180a4-111">Windows Event Log</span></span>

<span data-ttu-id="180a4-112">إذا لم يتم تشغيل أحدي هذه الخدمات ، فحاول بدء تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="180a4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="180a4-113">إذا كانت لديك مشكله في بدء تشغيل الخدمة ، فقم بتشغيل الأمر التالي بفتح موجه الأوامر باستخدام أذونات مرتفعه:</span><span class="sxs-lookup"><span data-stu-id="180a4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="180a4-114">**/scannow sfc**</span><span class="sxs-lookup"><span data-stu-id="180a4-114">**sfc /scannow**</span></span>

<span data-ttu-id="180a4-115">بعد انتهاء هذا الأمر ، أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="180a4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="180a4-116">للحصول علي معلومات مفصله ، راجع ["عذرا ، يتعذر علينا الاتصال بحسابك. الرجاء المحاولة مره أخرى لاحقا "عند التنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="180a4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>