---
title: تحديد أعاده توجيه البريد الكتروني الخارجي علي علب البريد في سجلات التدقيق
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696284"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="4afd2-102">تحديد وقت تكوين أعاده توجيه البريد الكتروني الخارجي علي علب البريد</span><span class="sxs-lookup"><span data-stu-id="4afd2-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="4afd2-103">عند قيام مستخدم Microsoft 365 بتكوين أعاده توجيه البريد الكتروني الخارجي علي علبه البريد ، يتم تدقيق النشاط كجزء من الأمر cmdlet **علبه البريد** .</span><span class="sxs-lookup"><span data-stu-id="4afd2-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="4afd2-104">يمكنك رؤية النشاط باستخدام البحث في سجل التدقيق في مركز توافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="4afd2-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="4afd2-105">سجل الدخول إلى [مركز توافق & أمان Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="4afd2-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="4afd2-106">انتقل إلى صفحه **Search**  >  **البحث في سجل تدقيق** البحث.</span><span class="sxs-lookup"><span data-stu-id="4afd2-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="4afd2-107">حدد نطاق التاريخ في الحقلين **"تاريخ البدء** " و " **تاريخ الانتهاء** ".</span><span class="sxs-lookup"><span data-stu-id="4afd2-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="4afd2-108">لا تحتاج إلى تحديد اسم المستخدم.</span><span class="sxs-lookup"><span data-stu-id="4afd2-108">You don't need to specify a username.</span></span> <span data-ttu-id="4afd2-109">تاكد من تعيين الحقل " **الانشطه** " **لعرض النتائج لكل الانشطه**.</span><span class="sxs-lookup"><span data-stu-id="4afd2-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="4afd2-110">انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="4afd2-110">Click **Search**.</span></span>

<span data-ttu-id="4afd2-111">في النتائج ، انقر فوق **تصفيه النتائج** واكتب **Set-علبه البريد** في المربع عامل تصفيه النشاط.</span><span class="sxs-lookup"><span data-stu-id="4afd2-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="4afd2-112">حدد سجل تدقيق في النتائج.</span><span class="sxs-lookup"><span data-stu-id="4afd2-112">Select an audit record in the results.</span></span> <span data-ttu-id="4afd2-113">في القائمة المنبثقة **التفاصيل** ، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="4afd2-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="4afd2-114">يجب عليك إلقاء نظره علي تفاصيل كل سجل تدقيق لتحديد ما إذا كان النشاط مرتبطا باعاده توجيه البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="4afd2-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="4afd2-115">**ObjectId**: القيمة المستعارة لعلبه البريد التي تم تعديلها.</span><span class="sxs-lookup"><span data-stu-id="4afd2-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="4afd2-116">**المعلمات**: _فورواردينجسمتبادريس_ تشير إلى عنوان البريد الكتروني الهدف.</span><span class="sxs-lookup"><span data-stu-id="4afd2-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="4afd2-117">**UserId**: المستخدم الذي قام بتكوين أعاده توجيه البريد الكتروني علي علبه البريد في الحقل **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="4afd2-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="4afd2-118">لمزيد من المعلومات ، راجع [تحديد الأشخاص الذين قاموا باعداد أعاده توجيه البريد الكتروني لعلبه البريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="4afd2-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
