---
title: مشكلة في مستخدم واحد
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429283"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="ccced-102">مشكلة في مستخدم واحد</span><span class="sxs-lookup"><span data-stu-id="ccced-102">Problem with single user</span></span>

- <span data-ttu-id="ccced-103">ربما لم يتم توفير الخدمة للمستخدم نظرا لعدم فرصة تقييم المستخدم بعد.</span><span class="sxs-lookup"><span data-stu-id="ccced-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="ccced-104">راجع الإرشادات المتعلقة بمدى الوقت الذي تستغرقه عملية التكوين بالإضافة إلى شريط التقدم على صفحة تكوين الإعداد.</span><span class="sxs-lookup"><span data-stu-id="ccced-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="ccced-105">إذا كانت الحالة الثابت المحددة في قسم التفاصيل الإضافية قبل تاريخ إنشاء/تحديث/حذف المستخدم، فهذا يعني أننا لم نقيم المستخدم بعد.</span><span class="sxs-lookup"><span data-stu-id="ccced-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="ccced-106">في هذا السيناريو، أفضل شيء يجب فعله هو انتظار انتهاء توفير الخدمة.</span><span class="sxs-lookup"><span data-stu-id="ccced-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="ccced-107">لاحظ أن خدمتنا على علم فقط بتغييرات المستخدم في النظام المصدر (الموارد البشرية في السحابة).</span><span class="sxs-lookup"><span data-stu-id="ccced-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="ccced-108">يجب أن يكون هناك تغيير صالح في نظام المصدر ل Azure AD للكشف عن التغيير وتدفقه إلى Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ccced-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="ccced-109">تم تقييم توفير الخدمة للمستخدم وحدد ضرورة عدم توفيرها:</span><span class="sxs-lookup"><span data-stu-id="ccced-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="ccced-110">إذا قمت بتعيين عامل تصفية تحديد عدد استنادا إلى سمة، فتأكد من أن المستخدم يلبي المعايير التي حددتها.</span><span class="sxs-lookup"><span data-stu-id="ccced-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="ccced-111">إذا كان المستخدمون موجودين بالفعل في النظام الهدف وكانت حالة المستخدم في تطابق المصدر والهدف، فلن نتخذ أي إجراء آخر.</span><span class="sxs-lookup"><span data-stu-id="ccced-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="ccced-112">حاول توفير الخدمة توفير المستخدم وفشل ذلك.</span><span class="sxs-lookup"><span data-stu-id="ccced-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="ccced-113">بالنسبة إلى هذه السيناريوهات، راجع علامة التبويب "استكشاف الأخطاء وإصلاحها" و"التوصيات" لسجلات توفير:</span><span class="sxs-lookup"><span data-stu-id="ccced-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="ccced-114">قد تكون السمة المطلوبة للمستخدم مفقودة في Active Directory أو Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ccced-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="ccced-115">على سبيل المثال، لا يتم إنشاء القيمة الصحيحة لقواعد الجيل userPrincipalName أو sAMAccountName.</span><span class="sxs-lookup"><span data-stu-id="ccced-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="ccced-116">لا يتم حل السمة المطابقة (عادة ما تكون employeeId) لمستخدم فريد في Active Directory المحلي أو Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ccced-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="ccced-117">على سبيل المثال، يوجد مستخدمان بنفس "الموظف" في AD وترجع الخدمة رمز خطأ يشير إلى إدخالات هدف مكررة لنفس إدخال المصدر.</span><span class="sxs-lookup"><span data-stu-id="ccced-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="ccced-118">لمراجعة السجلات لمستخدم فردي ومجموعات، راجع مراجعة سجلات توفير مشكلة مع [مستخدم معين.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="ccced-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
