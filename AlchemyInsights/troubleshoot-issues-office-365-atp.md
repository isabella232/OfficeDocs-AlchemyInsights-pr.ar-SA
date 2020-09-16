---
title: استكشاف الأخطاء وإصلاحها في Office 365 الحماية من المخاطر المتقدمة (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758052"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="bf94f-102">استكشاف الأخطاء وإصلاحها في Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="bf94f-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="bf94f-103">هل **تلاحظ التاخيرات مع تسليم رسائل البريد الكتروني**؟</span><span class="sxs-lookup"><span data-stu-id="bf94f-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="bf94f-104">جرب استخدام خيار التسليم الديناميكي لنهج المرفقات الامنه ل ATP.</span><span class="sxs-lookup"><span data-stu-id="bf94f-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="bf94f-105">سيؤدي ذلك إلى تجنب حدوث تاخيرات تسليم رسائل البريد الكتروني اثناء حماية المستلمين من الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="bf94f-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="bf94f-106">**هل تريد الإبلاغ عن خطا بوسيتيفيس أو خطا في النيجاتيف**؟</span><span class="sxs-lookup"><span data-stu-id="bf94f-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="bf94f-107">استخدم هذا الارتباط لإرسال الملف لتحليل: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="bf94f-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="bf94f-108">**هل تعلم انه يمكنك تمكين حماية الارتباطات الامنه ل ATP للبريد الكتروني المرسل بين الأشخاص في مؤسستك**؟</span><span class="sxs-lookup"><span data-stu-id="bf94f-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="bf94f-109">اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="bf94f-109">Follow these steps:</span></span>
    1. <span data-ttu-id="bf94f-110">انتقل إلى https://protection.office.com ، وسجل الدخول.</span><span class="sxs-lookup"><span data-stu-id="bf94f-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="bf94f-111">انتقل إلى **Threat management**  >  **Policy**  >  **الارتباطات الامنه**لنهج أداره المخاطر.</span><span class="sxs-lookup"><span data-stu-id="bf94f-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="bf94f-112">ضمن **النهج التي تنطبق علي مستلمين محددين**أو تحرير (أو أضافه) نهج.</span><span class="sxs-lookup"><span data-stu-id="bf94f-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="bf94f-113">حدد **تطبيق الارتباطات الامنه علي الرسائل المرسلة داخل المؤسسة**.</span><span class="sxs-lookup"><span data-stu-id="bf94f-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="bf94f-114">يمكنك حفظ النهج ، والسماح لمده 30 دقيقه لتغييراتك في العمل من خلال مركز بياناتك.</span><span class="sxs-lookup"><span data-stu-id="bf94f-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="bf94f-115">للحصول علي مزيد من المساعدة في استخدام ATP ، راجع [الحماية المتقدمة من المخاطر في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="bf94f-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>