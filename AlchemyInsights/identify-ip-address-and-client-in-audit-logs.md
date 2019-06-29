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
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382940"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="c6618-102">تحديد عنوان IP وعميل في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="c6618-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="c6618-103">يتم عرض عنوان IP المتوافق مع نشاط المستخدم أو المسؤول في "سجلات التدقيق".</span><span class="sxs-lookup"><span data-stu-id="c6618-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="c6618-104">كما يتم تسجيل معلومات العميل.</span><span class="sxs-lookup"><span data-stu-id="c6618-104">The client information is also logged.</span></span> <span data-ttu-id="c6618-105">فيما يلي الخطوات اللازمة لتحديد هذه المعلومات</span><span class="sxs-lookup"><span data-stu-id="c6618-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="c6618-106">تسجيل الدخول إلى [مركز التوافق ل Office الأمن 365 &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c6618-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c6618-107">انقر فوق **البحث والتحقيق** ، وحدد **البحث في سجل التدقيق**.</span><span class="sxs-lookup"><span data-stu-id="c6618-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="c6618-108">إذا كنت ترغب في نشاط معين، حدد من قائمة **الأنشطة** .</span><span class="sxs-lookup"><span data-stu-id="c6618-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="c6618-109">وإلا، سيتم إرجاع كافة الأنشطة الخاصة بالمستخدم المحدد (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="c6618-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="c6618-110">**ملاحظة**: بعض الأنشطة قد لا يكون متوفراً في قائمة **الأنشطة** ؛ غير أن تلك تدوين العناصر سوف يتم إرجاعها إذا كان **إظهار النتائج لكافة الأنشطة** المحددة (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="c6618-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="c6618-111">حدد اسم المستخدم في الحقل **المستخدمين** وحدد نطاق التاريخ المناسب للنشاط ثم انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="c6618-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="c6618-112">في النتائج، يمكنك مشاهدة عنوان IP لهذا النشاط في جزء النتائج.</span><span class="sxs-lookup"><span data-stu-id="c6618-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="c6618-113">حدد سجل التدقيق لمشاهدة المعلومات التفصيلية في القائمة الفرعية **تفاصيل** (على سبيل المثال، عميل، المستخدم الذي قام بتنفيذ الإجراء، إلخ.).</span><span class="sxs-lookup"><span data-stu-id="c6618-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="c6618-114">لمزيد من المعلومات، راجع [البحث عن عنوان IP للكمبيوتر المستخدم للوصول إلى حساب المكسور](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="c6618-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
