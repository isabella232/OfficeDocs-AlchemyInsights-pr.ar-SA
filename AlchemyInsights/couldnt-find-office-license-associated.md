---
title: إصلاح تطبيقات Microsoft 365 لا يمكن العثور على الرسالة المقترنة بتراخيص Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816475"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="0ad4f-102">إصلاح الرسالة "لم تتمكن من العثور على تراخيص Office المقترنة" في تطبيقات Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0ad4f-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="0ad4f-103">إذا تلقيت هذه الرسالة، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="0ad4f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0ad4f-104">تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="0ad4f-105">راجع [عناوين URL 365 في Microsoft 365 نطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="0ad4f-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="0ad4f-106">قم [بإزالة ترخيص Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) للمستخدم المتأثر ثم إعادة تعيينه.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="0ad4f-107">افتح تطبيق Office و [سجل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) من أي حسابات مستخدمين موجودة.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="0ad4f-108">انتقل إلى إعدادات Windows > **حسابات** البريد الإلكتروني & الحسابات ، وأزل كل حسابات العمل باستثناء  >  الحساب المتأثر.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="0ad4f-109">انتقل إلى إعدادات Windows > **حسابات** Access للعمل أو المدرسة ، واقطع اتصال كل حسابات العمل  >  باستثناء الحساب المتأثر.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="0ad4f-110">إعادة تعيين حالة تنشيط Office.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-110">Reset the Office activation state.</span></span> <span data-ttu-id="0ad4f-111">[تعرف على كيفية](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="0ad4f-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="0ad4f-112">[سجل الدخول](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="0ad4f-113">للحصول على حلول إضافية حول استكشاف الأخطاء وإصلاحها، راجع أخطاء التنشيط والمنتج غير مرخص [في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="0ad4f-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>