---
title: تعريف نشاط القاعدة الوارد في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383012"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2a03e-102">تعريف نشاط القاعدة الوارد في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="2a03e-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2a03e-103">يمكنك استخدام البحث في سجل التدقيق في & أمان مركز التوافق لعرض أحداث قاعدة علبة الوارد (إنشاء وتعديل وحذف قواعد علبة الوارد).</span><span class="sxs-lookup"><span data-stu-id="2a03e-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2a03e-104">تسجيل الدخول إلى [مركز التوافق ل Office الأمن 365 &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="2a03e-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="2a03e-105">انقر فوق **البحث والتحقيق** ، وحدد **البحث في سجل التدقيق**.</span><span class="sxs-lookup"><span data-stu-id="2a03e-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="2a03e-106">حدد نطاق التواريخ في حقول **تاريخ البدء** **وتاريخ الانتهاء** .</span><span class="sxs-lookup"><span data-stu-id="2a03e-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2a03e-107">ضمن **أنشطة صندوق بريد Exchange**، تأكد من تعيين حقل **الأنشطة** **إينبوكسرولي جديد إنشاء/تعديل/تمكين/تعطيل قاعدة الوارد**.</span><span class="sxs-lookup"><span data-stu-id="2a03e-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2a03e-108">انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="2a03e-108">Click **Search**.</span></span>

<span data-ttu-id="2a03e-109">في النتائج، حدد سجل تدقيق.</span><span class="sxs-lookup"><span data-stu-id="2a03e-109">In the results, select an audit record.</span></span> <span data-ttu-id="2a03e-110">في القائمة الفرعية "تفاصيل"، انقر فوق " **معلومات إضافية**".</span><span class="sxs-lookup"><span data-stu-id="2a03e-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2a03e-111">يتم عرض معلومات حول إعدادات قواعد علبة الوارد في الحقل **المعلمات** .</span><span class="sxs-lookup"><span data-stu-id="2a03e-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2a03e-112">لمزيد من المعلومات، راجع [تحديد إذا كان هناك مستخدم إنشاء قاعدة علبة الوارد](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="2a03e-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
