---
title: تحديد احداث الرسائل التي تم حذفها في سجلات التدقيق
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696500"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="0b784-102">سجلات التدقيق لرسائل البريد الكتروني المحذوفة</span><span class="sxs-lookup"><span data-stu-id="0b784-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="0b784-103">بدءا من يناير 2019 ، فان Microsoft سيقوم بتشغيل تسجيل تدقيق علبه البريد بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="0b784-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="0b784-104">وبخلاف ذلك ، لمراجعه احداث الرسائل التي تم حذفها لمستخدم معين ، تحتاج إلى تمكين إجراءات الحذف يدويا.</span><span class="sxs-lookup"><span data-stu-id="0b784-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="0b784-105">إذا كان تسجيل تدقيق علبه البريد ممكنا لمؤسسك أو لمستخدم معين ، فاتبع الخطوات أدناه.</span><span class="sxs-lookup"><span data-stu-id="0b784-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="0b784-106">تسجيل الدخول إلى [مركز توافق & أمان Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="0b784-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="0b784-107">انقر فوق **البحث والاستقصاء** وحدد **البحث في سجل التدقيق**.</span><span class="sxs-lookup"><span data-stu-id="0b784-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="0b784-108">حدد نطاق التاريخ في الحقلين **"تاريخ البدء** " و " **تاريخ الانتهاء** ".</span><span class="sxs-lookup"><span data-stu-id="0b784-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="0b784-109">حدد اسم المستخدم للمستخدم الذي تريد التحقق منه (المستخدم الذي حذف العناصر).</span><span class="sxs-lookup"><span data-stu-id="0b784-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="0b784-110">في حقل **الانشطه** ، حدد **الرسائل المحذوفة من مجلد العناصر المحذوفة** **ونقل الرسائل إلى مجلد العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="0b784-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="0b784-111">انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="0b784-111">Click **Search**.</span></span>

<span data-ttu-id="0b784-112">في النتائج ، حدد سجل تدقيق.</span><span class="sxs-lookup"><span data-stu-id="0b784-112">In the results, select an audit record.</span></span> <span data-ttu-id="0b784-113">في القائمة المنبثقة التفاصيل ، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="0b784-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="0b784-114">يتم عرض معلومات اضافيه حول العنصر المحذوف (علي سبيل المثال ، سطر الموضوع وموقع العنصر عند حذفه) في الحقل **أفيكتيديتيمس** .</span><span class="sxs-lookup"><span data-stu-id="0b784-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="0b784-115">ستظهر الخاصية **كلينتينفوسترينج** إذا حدث الحذف في Outlook أو outlook علي الويب (المعروف سابقا ب Outlook web App) أو اي جهاز آخر.</span><span class="sxs-lookup"><span data-stu-id="0b784-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="0b784-116">لمزيد من المعلومات ، راجع [تحديد الأشخاص الذين قاموا باعداد أعاده توجيه البريد الكتروني لعلبه البريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="0b784-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="0b784-117">**ملاحظه**: لا يمكنك استرداد العناصر المحذوفة باستخدام ميزه سجل التدقيق.</span><span class="sxs-lookup"><span data-stu-id="0b784-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="0b784-118">لاسترداد الرسائل المحذوفة في Outlook علي الويب ، راجع [استرداد العناصر المحذوفة في Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="0b784-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
