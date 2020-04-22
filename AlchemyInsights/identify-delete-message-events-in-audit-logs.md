---
title: تحديد أحداث حذف الرسائل في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716483"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="905dd-102">سجلات التدقيق لرسائل البريد الإلكتروني المحذوفة</span><span class="sxs-lookup"><span data-stu-id="905dd-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="905dd-103">بدءًا من يناير 2019، تقوم Microsoft بتشغيل تسجيل تدقيق علبة البريد بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="905dd-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="905dd-104">وإلا، لمراجعة أحداث حذف الرسائل لمستخدم معين، تحتاج إلى تمكين إجراءات الحذف للتدقيق يدويًا.</span><span class="sxs-lookup"><span data-stu-id="905dd-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="905dd-105">إذا تم بالفعل تمكين تسجيل تدقيق علبة البريد لمؤسستك أو للمستخدم المحدد، فاتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="905dd-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="905dd-106">تسجيل الدخول إلى [مركز التوافق & الأمان Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="905dd-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="905dd-107">انقر فوق **البحث والتحقيق** وحدد بحث **سجل التدقيق**.</span><span class="sxs-lookup"><span data-stu-id="905dd-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="905dd-108">حدد نطاق التاريخ في **حقول تاريخ البدء** وتاريخ **الانتهاء.**</span><span class="sxs-lookup"><span data-stu-id="905dd-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="905dd-109">حدد اسم المستخدم للمستخدم الذي تريد التحقيق (المستخدم الذي حذف العناصر).</span><span class="sxs-lookup"><span data-stu-id="905dd-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="905dd-110">في حقل **الأنشطة،** حدد **الرسائل المحذوفة من مجلد العناصر المحذوفة** **والرسائل التي تم نقلها إلى مجلد العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="905dd-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="905dd-111">انقر فوق **البحث**.</span><span class="sxs-lookup"><span data-stu-id="905dd-111">Click **Search**.</span></span>

<span data-ttu-id="905dd-112">في النتائج، حدد سجل تدقيق.</span><span class="sxs-lookup"><span data-stu-id="905dd-112">In the results, select an audit record.</span></span> <span data-ttu-id="905dd-113">في التفاصيل المنبثقة، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="905dd-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="905dd-114">يتم عرض معلومات إضافية حول العنصر المحذوف (على سبيل المثال، سطر الموضوع وموقع العنصر عند حذفه) في حقل **العناصر المتأثرة.**</span><span class="sxs-lookup"><span data-stu-id="905dd-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="905dd-115">ستظهر خاصية **ClientInfoString** إذا حدث الحذف في Outlook أو Outlook على الويب (المعروف سابقًا باسم Outlook Web App) أو أي جهاز آخر.</span><span class="sxs-lookup"><span data-stu-id="905dd-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="905dd-116">لمزيد من المعلومات، راجع [تحديد من قام بإعداد إعادة توجيه البريد الإلكتروني لعلبة بريد](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="905dd-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="905dd-117">**ملاحظة:** لا يمكنك استرداد العناصر المحذوفة باستخدام ميزة سجل التدقيق.</span><span class="sxs-lookup"><span data-stu-id="905dd-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="905dd-118">لاسترداد الرسائل المحذوفة في Outlook على الويب، راجع [استرداد العناصر المحذوفة في Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="905dd-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
