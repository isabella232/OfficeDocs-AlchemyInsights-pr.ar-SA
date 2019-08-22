---
title: تحديد عنوان IP وعميل في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539016"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="bd938-102">تحديد عنوان IP وعميل في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="bd938-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="bd938-103">يتم عرض عنوان IP المتوافق مع نشاط مسؤول أو مستخدم Office 365 في "سجلات التدقيق".</span><span class="sxs-lookup"><span data-stu-id="bd938-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="bd938-104">كما يتم تسجيل معلومات العميل.</span><span class="sxs-lookup"><span data-stu-id="bd938-104">The client information is also logged.</span></span> <span data-ttu-id="bd938-105">فيما يلي الخطوات اللازمة لتحديد هذه المعلومات</span><span class="sxs-lookup"><span data-stu-id="bd938-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="bd938-106">تسجيل الدخول إلى [مركز التوافق & الأمن 365 Office](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="bd938-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="bd938-107">انتقل إلى **بحث** > صفحة**البحث في سجل التدقيق** .</span><span class="sxs-lookup"><span data-stu-id="bd938-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="bd938-108">إذا كنت ترغب في نشاط معين، حدد من قائمة **الأنشطة** .</span><span class="sxs-lookup"><span data-stu-id="bd938-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="bd938-109">وإلا، سيتم إرجاع كافة الأنشطة الخاصة بالمستخدم المحدد (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="bd938-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="bd938-110">**ملاحظة**: بعض الأنشطة قد لا يكون متوفراً في قائمة **الأنشطة** ؛ غير أن تلك تدوين العناصر سوف يتم إرجاعها إذا كان **إظهار النتائج لكافة الأنشطة** المحددة (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="bd938-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="bd938-111">حدد اسم المستخدم في الحقل **المستخدمين** وحدد نطاق التاريخ المناسب للنشاط ثم انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="bd938-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="bd938-112">في النتائج، يمكنك مشاهدة عنوان IP لهذا النشاط في جزء النتائج.</span><span class="sxs-lookup"><span data-stu-id="bd938-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="bd938-113">حدد سجل التدقيق لمشاهدة المعلومات التفصيلية في القائمة الفرعية **تفاصيل** (على سبيل المثال، عميل، المستخدم الذي قام بتنفيذ الإجراء، إلخ.).</span><span class="sxs-lookup"><span data-stu-id="bd938-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="bd938-114">لمزيد من المعلومات، راجع [البحث عن عنوان IP للكمبيوتر المستخدم للوصول إلى حساب المكسور](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="bd938-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
