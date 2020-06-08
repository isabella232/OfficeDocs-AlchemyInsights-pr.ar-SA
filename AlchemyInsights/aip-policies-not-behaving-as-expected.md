---
title: 'AIP: السياسات لا تتصرف كما هو متوقع'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580752"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="0a23d-102">AIP: السياسات لا تتصرف كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="0a23d-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="0a23d-103">حماية المعلومات Azure: السياسات لا تتصرف كما هو متوقع، راجع ما يلي للإرشادات الموصى بها لمختلف مشكلات السياسة:</span><span class="sxs-lookup"><span data-stu-id="0a23d-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="0a23d-104">إذا كنت تواجه مشكلات في العلامات البصرية، يرجى مراجعة [عند تطبيق العلامات المرئية.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="0a23d-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="0a23d-105">إذا كنت تواجه مشكلات في وضع العلامات التلقائية، يرجى مراجعة [كيفية تكوين شروط التصنيف التلقائي والموصى به لحماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) وما تبحث عنه أنواع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="0a23d-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="0a23d-106">إذا كنت تواجه مشاكل مع حماية الأصلي / Pfile، يرجى مراجعة [تكوين واجهة برمجة التطبيقات ملف](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="0a23d-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="0a23d-107">تحقق مما إذا كنت تستخدم نُهج ًا ذات نطاق لم يتم تكوينها بشكل صحيح: [كيفية تكوين نهج حماية المعلومات Azure لمستخدمين محددين باستخدام نُهج ذات نطاق](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="0a23d-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="0a23d-108">إذا لم يعمل وضع العلامات التلقائي ة مع Outlook عند إرفاق مستند مسمى، فتحقق من عدم تعريف DRMEncryptProperty كما هو موضح هنا: [إعدادات التسجيل IRM للأمان](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="0a23d-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="0a23d-109">إذا كنت لا تزال تواجه مشكلات، يرجى جمع سجلات عملاء حماية المعلومات Azure وإرفاق السجلات المصدرة بهذه التذكرة.</span><span class="sxs-lookup"><span data-stu-id="0a23d-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="0a23d-110">افتح مستند Office أو أنشئ بريدًا إلكترونيًا جديدًا في Outlook.</span><span class="sxs-lookup"><span data-stu-id="0a23d-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="0a23d-111">انقر فوق **حماية / تعليمات الحساسية**  >  **والملاحظات.**</span><span class="sxs-lookup"><span data-stu-id="0a23d-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="0a23d-112">انقر فوق **سجلات التصدير**.</span><span class="sxs-lookup"><span data-stu-id="0a23d-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="0a23d-113">احفظ السجلات على اختيارك للموقع، وإرفاقها بطلب الخدمة هذا.</span><span class="sxs-lookup"><span data-stu-id="0a23d-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="0a23d-114">موارد إضافية:</span><span class="sxs-lookup"><span data-stu-id="0a23d-114">Additional resources:</span></span>

- [<span data-ttu-id="0a23d-115">كيفية تكوين تسمية للعلامات المرئية لحماية معلومات Azure</span><span class="sxs-lookup"><span data-stu-id="0a23d-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="0a23d-116">مراجعة وثائق حماية المعلومات Azure</span><span class="sxs-lookup"><span data-stu-id="0a23d-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="0a23d-117">استخدام تسميات الحساسية في تطبيقات Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0a23d-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

