---
title: استكشاف المشاكل المتعلقة بحماية التهديدات المتقدمة من Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766732"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="e8214-102">استكشاف المشاكل وإصلاحها باستخدام Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="e8214-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="e8214-103">**هل لاحظت تأخيرات في تسليم رسالة البريد الإلكتروني؟**</span><span class="sxs-lookup"><span data-stu-id="e8214-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="e8214-104">حاول استخدام خيار التسليم الديناميكي لنُهج المرفقات الآمنة ATP.</span><span class="sxs-lookup"><span data-stu-id="e8214-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="e8214-105">سيؤدي ذلك إلى تجنب تأخير تسليم رسائل البريد الإلكتروني مع حماية المستلمين من الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="e8214-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="e8214-106">**هل تريد الإبلاغ عن إيجابيات كاذبة أو سلبيات كاذبة؟**</span><span class="sxs-lookup"><span data-stu-id="e8214-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="e8214-107">استخدم هذا الرابط لإرسال الملف للتحليل:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="e8214-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="e8214-108">**هل تعلم أنه يمكنك تمكين حماية ATP Safe Links للبريد الإلكتروني المرسل بين الأشخاص في مؤسستك؟**</span><span class="sxs-lookup"><span data-stu-id="e8214-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="e8214-109">اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="e8214-109">Follow these steps:</span></span>
    1. <span data-ttu-id="e8214-110">انتقل https://protection.office.comإلى ، وتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="e8214-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="e8214-111">انتقل إلى**روابط\*\*\*\*آمنة لسياسة** >  **إدارة** > التهديدات.</span><span class="sxs-lookup"><span data-stu-id="e8214-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="e8214-112">ضمن **السياسات التي تنطبق على مستلمين محددين،** قم بتحرير (أو إضافة) نهج.</span><span class="sxs-lookup"><span data-stu-id="e8214-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="e8214-113">حدد **تطبيق ارتباطات آمنة على الرسائل المرسلة داخل المؤسسة**.</span><span class="sxs-lookup"><span data-stu-id="e8214-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="e8214-114">احفظ سياستك، واسمح لحوالي 30 دقيقة للتغييرات الخاصة بك بالعمل في طريقها من خلال مركز البيانات الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="e8214-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="e8214-115">للحصول على مزيد من المساعدة في ATP، راجع [Office 365 الحماية المتقدمة من التهديدات.](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="e8214-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>