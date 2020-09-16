---
title: إصلاح تطبيقات Microsoft 365 تعذر العثور علي الرسالة المقترنة بتراخيص office
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747682"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="48412-102">إصلاح الرسالة Microsoft 365 تعذر العثور علي تراخيص office المقترنة</span><span class="sxs-lookup"><span data-stu-id="48412-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="48412-103">إذا تلقيت هذه الرسالة ، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="48412-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="48412-104">تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر الوصول إلى تطبيقات Microsoft 365 علي الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="48412-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="48412-105">راجع [نطاقات عناوين IP و Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="48412-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="48412-106">أزاله [ترخيص Office وأعاده تعيينه](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) للمستخدم المتاثر.</span><span class="sxs-lookup"><span data-stu-id="48412-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="48412-107">افتح تطبيق Office [وسجل خروجك](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) من اي حسابات مستخدمين موجودة.</span><span class="sxs-lookup"><span data-stu-id="48412-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="48412-108">انتقل إلى إعدادات Windows > البريد الكتروني **للحسابات**  >  **& الحسابات**، وقم بازاله كل حسابات العمل باستثناء الحساب المتاثر.</span><span class="sxs-lookup"><span data-stu-id="48412-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="48412-109">انتقل إلى إعدادات Windows > **الحسابات**  >  الخاصة**بالعمل أو المؤسسة التعليمية**، وقم بقطع اتصال كل حسابات العمل باستثناء الحساب المتاثر.</span><span class="sxs-lookup"><span data-stu-id="48412-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="48412-110">أعاده تعيين حاله تنشيط Office.</span><span class="sxs-lookup"><span data-stu-id="48412-110">Reset the Office activation state.</span></span> <span data-ttu-id="48412-111">[تعرف علي كيفيه القيام](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)بذلك.</span><span class="sxs-lookup"><span data-stu-id="48412-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="48412-112">[سجل الدخول](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتاثر.</span><span class="sxs-lookup"><span data-stu-id="48412-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="48412-113">للحصول علي حلول اضافيه لاستكشاف الأخطاء وإصلاحها ، راجع [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="48412-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>