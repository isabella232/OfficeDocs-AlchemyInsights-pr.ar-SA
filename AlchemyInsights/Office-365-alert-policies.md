---
title: 1385-Office-365-سياسات التنبيه
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 05c58bded5ba45aef8ae3bc1d33491e6e0365c18
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502414"
---
# <a name="alert-policies"></a><span data-ttu-id="e0a21-102">سياسات التنبيه</span><span class="sxs-lookup"><span data-stu-id="e0a21-102">Alert policies</span></span>

<span data-ttu-id="e0a21-103">يوفر مركز التوافق & الأمان من Microsoft 365 [نُهج تنبيه افتراضية](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) تقوم بتشغيل تنبيهات للمؤسسات التي تحتوي على اشتراك Office 365 Enterprise أو Office 365 في حكومة الولايات المتحدة E1/G1 أو E3/G3 أو E5/G5.</span><span class="sxs-lookup"><span data-stu-id="e0a21-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="e0a21-104">لذلك، قد يتلقى المسؤولون إشعار تنبيه بالبريد الإلكتروني مرسل بواسطة Office365Alerts@microsoft.com مع سطر موضوع مثل "تنبيه منخفض الخطورة: *اسم سياسة التنبيه*".</span><span class="sxs-lookup"><span data-stu-id="e0a21-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="e0a21-105">يتم إرسال إشعارات التنبيه عند تشغيل التنبيهات للأنشطة الشائعة، مثل عندما يقوم المستخدمون بذلك:</span><span class="sxs-lookup"><span data-stu-id="e0a21-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="e0a21-106">إنشاء قواعد البريد الوارد التي إعادة توجيه البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="e0a21-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="e0a21-107">تعيين أذونات علبة البريد الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="e0a21-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="e0a21-108">مشاركة أو حذف عدد كبير من الملفات في مشاركة ملفات SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e0a21-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="e0a21-109">إنشاء عمليات بحث eDiscovery وتصدير نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="e0a21-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="e0a21-110">لمراجعة التنبيه والتصرف بناءً عليه:</span><span class="sxs-lookup"><span data-stu-id="e0a21-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="e0a21-111">انتقل إلى [مركز التوافق & الأمان](https://protection.office.com) وتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="e0a21-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="e0a21-112">انقر فوق **تنبيهات**  >  **عرض التنبيهات**.</span><span class="sxs-lookup"><span data-stu-id="e0a21-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="e0a21-113">انقر فوق تنبيه لعرض صفحة منبثقة تحتوي على معلومات حول التنبيه.</span><span class="sxs-lookup"><span data-stu-id="e0a21-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="e0a21-114">يمكنك اتخاذ إجراء في تنبيه، مثل [إزالة قاعدة البريد الوارد المشبوهة](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="e0a21-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="e0a21-115">أو يمكنك ببساطة إغلاق التنبيه بالنقر فوق **حل** على صفحة المنبثقة التنبيه.</span><span class="sxs-lookup"><span data-stu-id="e0a21-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="e0a21-116">لمزيد من المعلومات حول تكوين وإدارة نُهج التنبيه، راجع [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="e0a21-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="e0a21-117">**هام:** لن تطلب منك إشعارات البريد الإلكتروني التنبيه من Microsoft أبدًا القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="e0a21-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="e0a21-118">توفير كلمة مرور</span><span class="sxs-lookup"><span data-stu-id="e0a21-118">Provide a password</span></span>
- <span data-ttu-id="e0a21-119">التحقق من تفاصيل الأمان في حسابك</span><span class="sxs-lookup"><span data-stu-id="e0a21-119">Verify the security details of your account</span></span>
- <span data-ttu-id="e0a21-120">إعادة المصادقة على نفسك</span><span class="sxs-lookup"><span data-stu-id="e0a21-120">Re-authenticate yourself</span></span>

<span data-ttu-id="e0a21-121">إذا تلقيت رسالة بريد إلكتروني مثل هذه، لم يتم إرسالها من قبل Microsoft وينبغي اعتبارها عملية احتيال احتيالية.</span><span class="sxs-lookup"><span data-stu-id="e0a21-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="e0a21-122">إذا حدث ذلك، يرجى [الإبلاغ عن ذلك إلى Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="e0a21-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>