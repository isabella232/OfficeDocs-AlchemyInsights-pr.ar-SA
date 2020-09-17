---
title: تحديد نشاط قاعده علبه الوارد في سجلات التدقيق
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779038"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="5e8f1-102">تحديد نشاط قاعده علبه الوارد في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="5e8f1-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="5e8f1-103">يمكنك استخدام البحث في سجل التدقيق في مركز التوافق ل Microsoft 365 Security & لعرض احداث قواعد علبه الوارد (إنشاء قواعد علبه الوارد وتعديلها وحذفها).</span><span class="sxs-lookup"><span data-stu-id="5e8f1-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="5e8f1-104">سجل الدخول إلى [مركز توافق & أمان Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="5e8f1-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="5e8f1-105">انتقل إلى صفحه **Search**  >  **البحث في سجل تدقيق** البحث.</span><span class="sxs-lookup"><span data-stu-id="5e8f1-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="5e8f1-106">حدد نطاق التاريخ في الحقلين **"تاريخ البدء** " و " **تاريخ الانتهاء** ".</span><span class="sxs-lookup"><span data-stu-id="5e8f1-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="5e8f1-107">ضمن **أنشطه علبه بريد Exchange**، تحقق من انه قد تم تعيين الحقل " **الانشطه** " علي **الإينبوكسرولي إنشاء/تعديل/تمكين قاعده علبه الوارد**.</span><span class="sxs-lookup"><span data-stu-id="5e8f1-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="5e8f1-108">انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="5e8f1-108">Click **Search**.</span></span>

<span data-ttu-id="5e8f1-109">في النتائج ، حدد سجل تدقيق.</span><span class="sxs-lookup"><span data-stu-id="5e8f1-109">In the results, select an audit record.</span></span> <span data-ttu-id="5e8f1-110">في القائمة المنبثقة التفاصيل ، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="5e8f1-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="5e8f1-111">يتم عرض معلومات حول إعدادات قاعده علبه الوارد في حقل **المعلمات** .</span><span class="sxs-lookup"><span data-stu-id="5e8f1-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="5e8f1-112">لمزيد من المعلومات ، راجع [تحديد ما إذا قام المستخدم بإنشاء قاعده علبه الوارد](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="5e8f1-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
