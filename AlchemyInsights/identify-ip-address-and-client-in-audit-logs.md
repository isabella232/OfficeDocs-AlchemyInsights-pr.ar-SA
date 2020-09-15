---
title: تحديد عنوان IP والعميل في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668297"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="7206d-102">تحديد عنوان IP والعميل في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="7206d-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="7206d-103">يظهر عنوان IP المتوافق مع نشاط بواسطة مستخدم أو مسؤول Microsoft 365 في سجلات التدقيق.</span><span class="sxs-lookup"><span data-stu-id="7206d-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="7206d-104">يتم أيضا تسجيل معلومات العميل.</span><span class="sxs-lookup"><span data-stu-id="7206d-104">The client information is also logged.</span></span> <span data-ttu-id="7206d-105">اليك الخطوات المطلوبة لتعريف هذه المعلومات</span><span class="sxs-lookup"><span data-stu-id="7206d-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="7206d-106">سجل الدخول إلى [مركز توافق & أمان Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="7206d-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="7206d-107">انتقل إلى صفحه **Search**  >  **البحث في سجل تدقيق** البحث.</span><span class="sxs-lookup"><span data-stu-id="7206d-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="7206d-108">إذا كنت مهتما بنشاط معين ، فحدده من قائمه **الانشطه** .</span><span class="sxs-lookup"><span data-stu-id="7206d-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="7206d-109">إذا لم يكن كذلك ، سيتم إرجاع كل الانشطه للمستخدم المحدد (الاعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="7206d-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="7206d-110">**ملاحظه**: قد لا تتوفر بعض الانشطه في قائمه " **الانشطه** " ؛ ومع ذلك ، سيتم إرجاع عناصر التدقيق هذه إذا تم تحديد **إظهار النتائج لكل الانشطه** (الاعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="7206d-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="7206d-111">حدد اسم المستخدم في الحقل **المستخدمون** ، وحدد نطاق التاريخ المناسب للنشاط ، ثم انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="7206d-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="7206d-112">في النتائج ، يمكنك رؤية عنوان IP لهذا النشاط في جزء النتائج.</span><span class="sxs-lookup"><span data-stu-id="7206d-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="7206d-113">حدد سجل التدقيق للاطلاع علي معلومات مفصله في القائمة المنبثقة **التفاصيل** (علي سبيل المثال ، العميل والمستخدم الذي نفذ الاجراء ، وما إلى ذلك).</span><span class="sxs-lookup"><span data-stu-id="7206d-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="7206d-114">للحصول علي مزيد من المعلومات ، راجع [البحث عن عنوان IP الخاص بالكمبيوتر المستخدم للوصول إلى حساب اختراق](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="7206d-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
