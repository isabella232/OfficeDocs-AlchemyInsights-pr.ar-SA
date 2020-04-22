---
title: تقارير سجل مراجعة SharePoint الكلاسيكية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741952"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="de848-102">سجلات تدقيق SharePoint وOneDrive</span><span class="sxs-lookup"><span data-stu-id="de848-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="de848-103">سجلات مراجعة الحسابات الكلاسيكية SharePoint</span><span class="sxs-lookup"><span data-stu-id="de848-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="de848-104">تم ترحيل التدقيق القديم SPO إلى سجل التدقيق الموحد (UAL).</span><span class="sxs-lookup"><span data-stu-id="de848-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="de848-105">وسيتم الآن تشغيل جميع تقارير مراجعة الحسابات القديمة للمنظمات غير القادرة على العمل من خلال UAL، وتم ترحيل إشارات مراجعة الحسابات القديمة إلى UAL.</span><span class="sxs-lookup"><span data-stu-id="de848-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="de848-106">التغييرات الرئيسية:</span><span class="sxs-lookup"><span data-stu-id="de848-106">Key changes:</span></span>

* <span data-ttu-id="de848-107">التشذيب غير متوفر كقدرة.</span><span class="sxs-lookup"><span data-stu-id="de848-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="de848-108">اختيار أحداث معينة للتدقيق غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="de848-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="de848-109">راجع [هذا المستند](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) للحصول على قائمة كاملة بالأحداث المدققة المتوفرة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="de848-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="de848-110">خيار **الموقع** ضمن **التقارير المخصصة** غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="de848-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="de848-111">لا يتوفر خيار **أحداث فتح المستندات أو تنزيلها.**</span><span class="sxs-lookup"><span data-stu-id="de848-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="de848-112">تكوين إعدادات التدقيق لمجموعة مواقع</span><span class="sxs-lookup"><span data-stu-id="de848-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="de848-113">سجلات تدقيق اتّحدت SharePoint وOneDrive الحديثة من الامتثال</span><span class="sxs-lookup"><span data-stu-id="de848-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="de848-114">تشغيل/إيقاف تسجيل التدقيق الموحد</span><span class="sxs-lookup"><span data-stu-id="de848-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="de848-115">لا يوجد تكوين إضافي مطلوب داخل SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="de848-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="de848-116">استخدم بحث تسجيل التدقيق للتحقق من نشاط الملف (الملفات) والمجلد (المجلدات) والمستخدم (الأذونات) والأذونات:</span><span class="sxs-lookup"><span data-stu-id="de848-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="de848-117">أنشطة الملفات والصفحات</span><span class="sxs-lookup"><span data-stu-id="de848-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="de848-118">أنشطة المجلد</span><span class="sxs-lookup"><span data-stu-id="de848-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="de848-119">أنشطة المشاركة وطلب الوصول</span><span class="sxs-lookup"><span data-stu-id="de848-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="de848-120">أنشطة المزامنة</span><span class="sxs-lookup"><span data-stu-id="de848-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="de848-121">أنشطة إدارة الموقع</span><span class="sxs-lookup"><span data-stu-id="de848-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="de848-122">لمزيد من المعلومات حول كيفية استرداد هذه الأحداث، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="de848-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
