---
title: 'AIP: لا يتم تنفيذ النهج كما هو متوقع'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821614"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="6988b-102">AIP: لا يتم تنفيذ النهج كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="6988b-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="6988b-103">حماية معلومات Azure: لا يتم تنفيذ النهج كما هو متوقع، راجع الإرشادات الموصى بها لقضايا النهج المختلفة:</span><span class="sxs-lookup"><span data-stu-id="6988b-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="6988b-104">إذا كنت تواجه مشاكل في العلامات المرئية، فالرجاء مراجعة [عند تطبيق العلامات المرئية](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="6988b-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="6988b-105">إذا كنت تواجه مشاكل في التسمية التلقائية، فالرجاء مراجعة كيفية تكوين الشروط للتصنيف التلقائي والموصى به ل [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) وما هي أنواع المعلومات الحساسة التي [تبحث عن](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="6988b-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="6988b-106">إذا كنت تواجه مشاكل في الحماية الأصلية/Pfile، فيرجى مراجعة [تكوين API للملفات](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="6988b-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="6988b-107">تحقق مما إذا كنت تستخدم نهج النطاق التي لم يتم تكوينها بشكل صحيح: كيفية تكوين نهج [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)لمستخدمين محددين باستخدام النهج ذات النطاق .</span><span class="sxs-lookup"><span data-stu-id="6988b-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="6988b-108">إذا لم تعمل التسمية التلقائية مع Outlook عند إرفاق مستند باسم، فتحقق من أن DRMEncryptProperty غير معرف كما هو موضح هنا: إعدادات تسجيل [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)الخاصة ب الأمان .</span><span class="sxs-lookup"><span data-stu-id="6988b-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="6988b-109">إذا كنت لا تزال تواجه مشاكل، فالرجاء تجميع سجلات عميل Azure Information Protection وإرفاق السجلات المصدرة بهذه التذكرة.</span><span class="sxs-lookup"><span data-stu-id="6988b-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="6988b-110">افتح مستند Office أو أنشئ رسالة بريد إلكتروني جديدة في Outlook.</span><span class="sxs-lookup"><span data-stu-id="6988b-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="6988b-111">انقر **فوق حماية/حساسية**  >  **تعليمات وملاحظات**.</span><span class="sxs-lookup"><span data-stu-id="6988b-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="6988b-112">انقر **فوق تصدير السجلات.**</span><span class="sxs-lookup"><span data-stu-id="6988b-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="6988b-113">احفظ السجلات إلى اختيارك للموقع، وأرفقها بطلب الخدمة هذا.</span><span class="sxs-lookup"><span data-stu-id="6988b-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="6988b-114">موارد إضافية:</span><span class="sxs-lookup"><span data-stu-id="6988b-114">Additional resources:</span></span>

- [<span data-ttu-id="6988b-115">كيفية تكوين تسمية العلامات المرئية ل Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6988b-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="6988b-116">مراجعة وثائق Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6988b-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="6988b-117">استخدام تسميات الحساسية في تطبيقات Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6988b-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

