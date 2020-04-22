---
title: تحديد نشاط قاعدة البريد الوارد في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716411"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="ffd44-102">تحديد نشاط قاعدة البريد الوارد في سجلات التدقيق</span><span class="sxs-lookup"><span data-stu-id="ffd44-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="ffd44-103">يمكنك استخدام بحث سجل التدقيق في مركز توافق & الأمان من Microsoft 365 لعرض أحداث قاعدة البريد الوارد (إنشاء قواعد البريد الوارد وتعديلها وحذفها).</span><span class="sxs-lookup"><span data-stu-id="ffd44-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="ffd44-104">تسجيل الدخول إلى [مركز التوافق & الأمان Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ffd44-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ffd44-105">انتقل إلى صفحة البحث في**سجل تدقيق** **البحث.** > </span><span class="sxs-lookup"><span data-stu-id="ffd44-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="ffd44-106">حدد نطاق التاريخ في **حقول تاريخ البدء** وتاريخ **الانتهاء.**</span><span class="sxs-lookup"><span data-stu-id="ffd44-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="ffd44-107">ضمن **أنشطة علبة البريد Exchange،** تحقق من تعيين حقل **الأنشطة** إلى **قاعدة علبة الوارد الجديدة إنشاء/تعديل/تمكين/تعطيل علبة الوارد.**</span><span class="sxs-lookup"><span data-stu-id="ffd44-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="ffd44-108">انقر فوق **البحث**.</span><span class="sxs-lookup"><span data-stu-id="ffd44-108">Click **Search**.</span></span>

<span data-ttu-id="ffd44-109">في النتائج، حدد سجل تدقيق.</span><span class="sxs-lookup"><span data-stu-id="ffd44-109">In the results, select an audit record.</span></span> <span data-ttu-id="ffd44-110">في التفاصيل المنبثقة، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="ffd44-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="ffd44-111">يتم عرض معلومات حول إعدادات قاعدة البريد الوارد في حقل **المعلمات.**</span><span class="sxs-lookup"><span data-stu-id="ffd44-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="ffd44-112">لمزيد من المعلومات، راجع [تحديد ما إذا كان المستخدم قد أنشأ قاعدة علبة الوارد](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="ffd44-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
