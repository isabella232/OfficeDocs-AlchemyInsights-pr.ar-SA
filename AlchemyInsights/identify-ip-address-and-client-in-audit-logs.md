---
title: تحديد عنوان IP والعميل في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716375"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="40de7-102">تحديد عنوان IP والعميل في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="40de7-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="40de7-103">يتم عرض عنوان IP الذي يتوافق مع نشاط من قبل مستخدم Microsoft 365 أو مسؤول في سجلات التدقيق.</span><span class="sxs-lookup"><span data-stu-id="40de7-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="40de7-104">يتم تسجيل معلومات العميل أيضاً.</span><span class="sxs-lookup"><span data-stu-id="40de7-104">The client information is also logged.</span></span> <span data-ttu-id="40de7-105">فيما يلي الخطوات اللازمة لتحديد هذه المعلومات</span><span class="sxs-lookup"><span data-stu-id="40de7-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="40de7-106">تسجيل الدخول إلى [مركز التوافق & الأمان Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="40de7-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="40de7-107">انتقل إلى صفحة البحث في**سجل تدقيق** **البحث.** > </span><span class="sxs-lookup"><span data-stu-id="40de7-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="40de7-108">إذا كنت مهتمًا بنشاط معين، فحدده من قائمة **الأنشطة.**</span><span class="sxs-lookup"><span data-stu-id="40de7-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="40de7-109">إذا لم يكن كذلك، سيتم إرجاع كافة الأنشطة للمستخدم المحدد (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="40de7-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="40de7-110">**ملاحظة:** قد لا تتوفر بعض الأنشطة في قائمة **الأنشطة؛** ومع ذلك، سيتم إرجاع عناصر التدقيق هذه إذا تم تحديد **إظهار النتائج لكافة الأنشطة** (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="40de7-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="40de7-111">حدد اسم المستخدم في حقل **المستخدمين،** وحدد النطاق الزمني المناسب للنشاط، ثم انقر فوق **البحث**.</span><span class="sxs-lookup"><span data-stu-id="40de7-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="40de7-112">في النتائج، يمكنك مشاهدة عنوان IP لهذا النشاط في جزء النتائج.</span><span class="sxs-lookup"><span data-stu-id="40de7-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="40de7-113">حدد سجل التدقيق للاطلاع على معلومات تفصيلية في **قائمة التفاصيل** (على سبيل المثال، العميل والمستخدم الذي قام بإجراء وما إلى ذلك).</span><span class="sxs-lookup"><span data-stu-id="40de7-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="40de7-114">لمزيد من المعلومات، راجع [العثور على عنوان IP للكمبيوتر المستخدم للوصول إلى حساب تم اختراقه.](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)</span><span class="sxs-lookup"><span data-stu-id="40de7-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
