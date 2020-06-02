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
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508903"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="5eb1f-102">تحديد عنوان IP والعميل في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="5eb1f-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="5eb1f-103">يتم عرض عنوان IP الذي يتوافق مع نشاط من قبل مستخدم Microsoft 365 أو مسؤول في سجلات التدقيق.</span><span class="sxs-lookup"><span data-stu-id="5eb1f-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="5eb1f-104">يتم تسجيل معلومات العميل أيضاً.</span><span class="sxs-lookup"><span data-stu-id="5eb1f-104">The client information is also logged.</span></span> <span data-ttu-id="5eb1f-105">فيما يلي الخطوات اللازمة لتحديد هذه المعلومات</span><span class="sxs-lookup"><span data-stu-id="5eb1f-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="5eb1f-106">تسجيل الدخول إلى [مركز التوافق & الأمان Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="5eb1f-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="5eb1f-107">انتقل إلى **Search**صفحة البحث في  >  **سجل تدقيق** البحث.</span><span class="sxs-lookup"><span data-stu-id="5eb1f-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="5eb1f-108">إذا كنت مهتمًا بنشاط معين، فحدده من قائمة **الأنشطة.**</span><span class="sxs-lookup"><span data-stu-id="5eb1f-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="5eb1f-109">إذا لم يكن كذلك، سيتم إرجاع كافة الأنشطة للمستخدم المحدد (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="5eb1f-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="5eb1f-110">**ملاحظة:** قد لا تتوفر بعض الأنشطة في قائمة **الأنشطة؛** ومع ذلك، سيتم إرجاع عناصر التدقيق هذه إذا تم تحديد **إظهار النتائج لكافة الأنشطة** (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="5eb1f-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="5eb1f-111">حدد اسم المستخدم في حقل **المستخدمين،** وحدد النطاق الزمني المناسب للنشاط، ثم انقر فوق **البحث**.</span><span class="sxs-lookup"><span data-stu-id="5eb1f-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="5eb1f-112">في النتائج، يمكنك مشاهدة عنوان IP لهذا النشاط في جزء النتائج.</span><span class="sxs-lookup"><span data-stu-id="5eb1f-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="5eb1f-113">حدد سجل التدقيق للاطلاع على معلومات تفصيلية في **قائمة التفاصيل** (على سبيل المثال، العميل والمستخدم الذي قام بإجراء وما إلى ذلك).</span><span class="sxs-lookup"><span data-stu-id="5eb1f-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="5eb1f-114">لمزيد من المعلومات، راجع [العثور على عنوان IP للكمبيوتر المستخدم للوصول إلى حساب تم اختراقه.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)</span><span class="sxs-lookup"><span data-stu-id="5eb1f-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
