---
title: تقارير سجل تدقيق SharePoint الكلاسيكية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992605"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="7b870-102">سجلات التدقيق في SharePoint و OneDrive</span><span class="sxs-lookup"><span data-stu-id="7b870-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="7b870-103">سجلات التدقيق الكلاسيكية ل SharePoint</span><span class="sxs-lookup"><span data-stu-id="7b870-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="7b870-104">تم ترحيل التدقيق القديم لمقياس المجال الاستراتيجي إلى سجل التدقيق الموحد (UAL).</span><span class="sxs-lookup"><span data-stu-id="7b870-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="7b870-105">سيتم الآن تشغيل كافة تقارير مراجعه الحسابات القديمة من خلال التقرير الكتروني للحسابات ، وتم ترحيل إشارات مراجعه الحسابات القديمة إلى UAL.</span><span class="sxs-lookup"><span data-stu-id="7b870-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="7b870-106">التغييرات الرئيسية:</span><span class="sxs-lookup"><span data-stu-id="7b870-106">Key changes:</span></span>

* <span data-ttu-id="7b870-107">التشذيب غير متوفر كقدره.</span><span class="sxs-lookup"><span data-stu-id="7b870-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="7b870-108">اختيار احداث معينه للتدقيق غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="7b870-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="7b870-109">راجع [هذا المستند](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) للحصول علي قائمه كامله بالاحداث المدققة المتوفرة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="7b870-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="7b870-110">خيار **الموقع** ضمن **التقارير المخصصة** غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="7b870-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="7b870-111">الخيار **فتح أو تحميل الاحداث المستندات** غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="7b870-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="7b870-112">تكوين إعدادات التدقيق لمجموعه موقع</span><span class="sxs-lookup"><span data-stu-id="7b870-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="7b870-113">سجلات SharePoint و OneDrive الحديثة الموحدة للتدقيق من الامتثال</span><span class="sxs-lookup"><span data-stu-id="7b870-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="7b870-114">تشغيل/إيقاف التسجيل الموحد للتدقيق</span><span class="sxs-lookup"><span data-stu-id="7b870-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="7b870-115">لا يوجد تكوين إضافي مطلوب داخل SharePoint أو اندريف.</span><span class="sxs-lookup"><span data-stu-id="7b870-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="7b870-116">استخدام تدوين تسجيل البحث للتحقق من نشاط الملف (المجلدات) ، والمستخدم (ق) ، والأذونات:</span><span class="sxs-lookup"><span data-stu-id="7b870-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="7b870-117">أنشطه الملفات والصفحات</span><span class="sxs-lookup"><span data-stu-id="7b870-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="7b870-118">أنشطه المجلد</span><span class="sxs-lookup"><span data-stu-id="7b870-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="7b870-119">أنشطه طلب المشاركة والوصول</span><span class="sxs-lookup"><span data-stu-id="7b870-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="7b870-120">أنشطه التزامن</span><span class="sxs-lookup"><span data-stu-id="7b870-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="7b870-121">أنشطه أداره الموقع</span><span class="sxs-lookup"><span data-stu-id="7b870-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="7b870-122">لمزيد من المعلومات حول كيفيه استرداد هذه الاحداث ، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="7b870-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
