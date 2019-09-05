---
title: لم يتم تسليم إعلامات تنبيه SharePoint
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36744628"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="d1f63-102">لم يتم تسليم إعلامات تنبيه SharePoint</span><span class="sxs-lookup"><span data-stu-id="d1f63-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="d1f63-103">الرجاء التحقق من مجلد JUNK في بريدك الإلكتروني، حيث قد تذهب التنبيهات إلى هناك في بعض الأحيان.</span><span class="sxs-lookup"><span data-stu-id="d1f63-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="d1f63-104">تحديد ما إذا **لم يتم تسليم كافة التنبيهات** أو إذا لم يتم تسليم تنبيه **فردي** من ملف معين أو مكتبة معينة.</span><span class="sxs-lookup"><span data-stu-id="d1f63-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="d1f63-105">**لا يتم تسليم التنبيهات الفردية:** إذا لم يتم تسليم تنبيه فردي من ملف أو مكتبة معينة، يمكنك محاولة حذفه وإعادة إنشائه.</span><span class="sxs-lookup"><span data-stu-id="d1f63-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="d1f63-106">راجع [إدارة تنبيهات SharePoint أو عرضها أو حذفها](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) لإعادة إنشاء التنبيه.</span><span class="sxs-lookup"><span data-stu-id="d1f63-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="d1f63-107">**لا يتم تسليم كافة التنبيهات:** إذا لم يتم تسليم كافة التنبيهات من ملفات أو مكتبات متعددة، قم بزيارة [لوحة معلومات "صحة الخدمة"](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) للتحقق من وجود أية نصائح/حوادث قد تحدث مع SharePoint أو Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1f63-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="d1f63-108">قد تكون المشكلة مع إمكانية التنبيه SharePoint أو التأخير في رسائل البريد الإلكتروني من خلال Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1f63-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="d1f63-109">سيكون من المهم أيضًا ملاحظة ما إذا كان يتم تسليم بريد إلكتروني آخر، وإذا لم يكن الأمر كذلك، فمن المحتمل أن تكون المشكلة مع تأخيرات Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1f63-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="d1f63-110">الأسئلة الشائعة حول التنبيهات:</span><span class="sxs-lookup"><span data-stu-id="d1f63-110">FAQ on alerts:</span></span>

- <span data-ttu-id="d1f63-111">من غير الممكن إرسال تنبيهات إلى مجموعة التوزيع، يتم دعم مجموعات الأمان وO365 فقط.</span><span class="sxs-lookup"><span data-stu-id="d1f63-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="d1f63-112">لا يمكنك تخصيص قوالب البريد الإلكتروني التنبيه; تحتاج إلى استخدام Microsoft FLOW أو سير عمل مصمم SharePoint لتحقيق تلك.</span><span class="sxs-lookup"><span data-stu-id="d1f63-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="d1f63-113">مزيد من المعلومات:</span><span class="sxs-lookup"><span data-stu-id="d1f63-113">More Information:</span></span>

- <span data-ttu-id="d1f63-114">**إعداد التنبيه**: لمزيد من المعلومات حول إعداد التنبيهات، راجع [إنشاء تنبيه للحصول على إعلام عند تغيير ملف أو مجلد في SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="d1f63-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="d1f63-115">**استكشاف أخطاء التنبيهات وإصلاحها:** لمزيد من المعلومات حول استكشاف أخطاء التنبيهات وإصلاحها، راجع [عدم تلقي المستخدمين إشعارات تنبيه SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="d1f63-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="d1f63-116">**نُهج تنبيه التوافق المتقدمة لـ O365:** لمزيد من المعلومات حول إعداد هذه التنبيهات، راجع [نُهج تنبيه التوافق](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="d1f63-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="d1f63-117">**سجلات تدقيق SharePoint و OneDrive:** لمزيد من المعلومات حول كيفية استرداد هذه الأحداث، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d1f63-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="d1f63-118">**التنبيهات المرسلة من قبل الحماية المتقدمة من التهديدات:** راجع [ATP لSharePoint و OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="d1f63-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="d1f63-119">**التنبيهات المرسلة من قبل شرطة منع فقدان البيانات**: راجع إشعارات البريد الإلكتروني لسياسات [DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="d1f63-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d1f63-120">مواضيع ذات صلة</span><span class="sxs-lookup"><span data-stu-id="d1f63-120">Related Topics</span></span>

<span data-ttu-id="d1f63-121">هل تريد تجربة تدفق Microsoft في SharePoint عبر الإنترنت؟</span><span class="sxs-lookup"><span data-stu-id="d1f63-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="d1f63-122">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="d1f63-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="d1f63-123">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="d1f63-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
