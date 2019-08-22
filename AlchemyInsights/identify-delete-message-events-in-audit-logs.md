---
title: تعريف الأحداث رسالة حذف سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539196"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="aeaab-102">سجلات التدقيق للحصول على رسائل البريد الإلكتروني المحذوف</span><span class="sxs-lookup"><span data-stu-id="aeaab-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="aeaab-103">ابتداء من كانون الثاني/يناير عام 2019، Microsoft يتم تشغيل تدقيق علبة البريد تسجيل بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="aeaab-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="aeaab-104">وإلا، لمراجعة أحداث رسالة حذف لمستخدم معين، تحتاج إلى تمكين تدقيق إجراءات الحذف يدوياً.</span><span class="sxs-lookup"><span data-stu-id="aeaab-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="aeaab-105">حالة التدقيق علبة البريد تم تمكين التسجيل للمؤسسة الخاصة بك أو لمستخدم معين، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="aeaab-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="aeaab-106">تسجيل الدخول إلى [مركز التوافق ل Office الأمن 365 &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="aeaab-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="aeaab-107">انقر فوق **البحث والتحقيق** ، وحدد **البحث في سجل التدقيق**.</span><span class="sxs-lookup"><span data-stu-id="aeaab-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="aeaab-108">حدد نطاق التواريخ في حقول **تاريخ البدء** **وتاريخ الانتهاء** .</span><span class="sxs-lookup"><span data-stu-id="aeaab-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="aeaab-109">تحديد اسم المستخدم للمستخدم الذي تريد التحقيق (المستخدم الذي قام بحذف العناصر).</span><span class="sxs-lookup"><span data-stu-id="aeaab-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="aeaab-110">في مجال **الأنشطة** ، حدد **الرسائل المحذوفة من مجلد "العناصر المحذوفة"** و **نقل الرسائل إلى مجلد "العناصر المحذوفة"**.</span><span class="sxs-lookup"><span data-stu-id="aeaab-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="aeaab-111">انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="aeaab-111">Click **Search**.</span></span>

<span data-ttu-id="aeaab-112">في النتائج، حدد سجل تدقيق.</span><span class="sxs-lookup"><span data-stu-id="aeaab-112">In the results, select an audit record.</span></span> <span data-ttu-id="aeaab-113">في القائمة الفرعية "تفاصيل"، انقر فوق " **معلومات إضافية**".</span><span class="sxs-lookup"><span data-stu-id="aeaab-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="aeaab-114">يتم عرض معلومات إضافية حول العنصر المحذوف (على سبيل المثال، سطر الموضوع وموقع العنصر عند حذفه) في الحقل **أفيكتيديتيمس** .</span><span class="sxs-lookup"><span data-stu-id="aeaab-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="aeaab-115">سوف تظهر الخاصية **كلينتينفوسترينج** إذا حدث الحذف في Outlook، Outlook على الويب (تعرف سابقا باسم تطبيق ويب Outlook) أو أي جهاز آخر.</span><span class="sxs-lookup"><span data-stu-id="aeaab-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="aeaab-116">لمزيد من المعلومات، راجع [تحديد الذي قام بإعداد علبة بريد إرسال البريد الإلكتروني](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="aeaab-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="aeaab-117">**ملاحظة**: لا يمكن استرداد العناصر المحذوفة باستخدام ميزة سجل التدقيق.</span><span class="sxs-lookup"><span data-stu-id="aeaab-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="aeaab-118">لاستعادة الرسائل المحذوفة في Outlook على الويب، راجع [استرداد العناصر المحذوفة في Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="aeaab-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
