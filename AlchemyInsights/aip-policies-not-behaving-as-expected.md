---
title: 'AIP: لا تعمل النهج كما هو متوقع'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663176"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="49014-102">AIP: لا تعمل النهج كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="49014-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="49014-103">حماية المعلومات في Azure: لا تعمل النهج كما هو متوقع ، راجع ما يلي للإرشادات المستحسنة لمشاكل النهج المختلفة:</span><span class="sxs-lookup"><span data-stu-id="49014-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="49014-104">إذا كنت تواجه مشاكل تتعلق بالعلامات المرئية ، فيرجى المراجعة [عند تطبيق "العلامات المرئية](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)".</span><span class="sxs-lookup"><span data-stu-id="49014-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="49014-105">إذا كنت تواجه مشاكل في التسمية التلقائية ، فالرجاء مراجعه [كيفيه تكوين الشروط الخاصة بالتصنيف التلقائي والمستحسن لحماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [وما تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="49014-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="49014-106">إذا كنت تواجه مشاكل في حماية الملفات الاصليه/pfile فالرجاء مراجعه [تكوين API للملف](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="49014-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="49014-107">تحقق مما إذا كنت تستخدم نهجا في نطاق غير مكون بشكل صحيح: [كيفيه تكوين نهج حماية البيانات في Azure لمستخدمين محددين باستخدام نهج ذات نطاق](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="49014-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="49014-108">إذا لم يعمل الوضع "التسمية التلقائية" في Outlook عند إرفاق مستند مسمي ، فتحقق من ان درمينكريبتبروبيرتي غير معرف كما هو موضح هنا: [إعدادات سجل IRM للامان](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="49014-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="49014-109">إذا كنت لا تزال تواجه مشاكل ، يرجى جمع سجلات عميل حماية البيانات في Azure وإرفاق السجلات التي تم تصديرها بهذه البطاقة.</span><span class="sxs-lookup"><span data-stu-id="49014-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="49014-110">افتح مستند Office أو قم بإنشاء رسالة بريد الكتروني جديده في Outlook.</span><span class="sxs-lookup"><span data-stu-id="49014-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="49014-111">انقر **Protect/Sensitivity**فوق  >  **التعليمات الخاصة بالحماية/الحساسية والملاحظات**.</span><span class="sxs-lookup"><span data-stu-id="49014-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="49014-112">انقر فوق **تصدير السجلات**.</span><span class="sxs-lookup"><span data-stu-id="49014-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="49014-113">احفظ السجلات في اختيار الموقع ، وقم بإرفاقها بطلب الخدمة هذا.</span><span class="sxs-lookup"><span data-stu-id="49014-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="49014-114">موارد إضافية:</span><span class="sxs-lookup"><span data-stu-id="49014-114">Additional resources:</span></span>

- [<span data-ttu-id="49014-115">كيفيه تكوين تسميه لوضع العلامات المرئية لحماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="49014-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="49014-116">مراجعه وثائق حماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="49014-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="49014-117">استخدام تسميات الحساسية في تطبيقات Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="49014-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

