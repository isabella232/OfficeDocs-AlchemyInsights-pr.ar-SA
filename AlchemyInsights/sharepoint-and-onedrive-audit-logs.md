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
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509587"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="79b18-102">سجلات تدقيق SharePoint وOneDrive</span><span class="sxs-lookup"><span data-stu-id="79b18-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="79b18-103">سجلات مراجعة الحسابات الكلاسيكية SharePoint</span><span class="sxs-lookup"><span data-stu-id="79b18-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="79b18-104">تم ترحيل التدقيق القديم SPO إلى سجل التدقيق الموحد (UAL).</span><span class="sxs-lookup"><span data-stu-id="79b18-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="79b18-105">وسيتم الآن تشغيل جميع تقارير مراجعة الحسابات القديمة للمنظمات غير القادرة على العمل من خلال UAL، وتم ترحيل إشارات مراجعة الحسابات القديمة إلى UAL.</span><span class="sxs-lookup"><span data-stu-id="79b18-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="79b18-106">التغييرات الرئيسية:</span><span class="sxs-lookup"><span data-stu-id="79b18-106">Key changes:</span></span>

* <span data-ttu-id="79b18-107">التشذيب غير متوفر كقدرة.</span><span class="sxs-lookup"><span data-stu-id="79b18-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="79b18-108">اختيار أحداث معينة للتدقيق غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="79b18-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="79b18-109">راجع [هذا المستند](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) للحصول على قائمة كاملة بالأحداث المدققة المتوفرة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="79b18-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="79b18-110">خيار **الموقع** ضمن **التقارير المخصصة** غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="79b18-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="79b18-111">لا يتوفر خيار **أحداث فتح المستندات أو تنزيلها.**</span><span class="sxs-lookup"><span data-stu-id="79b18-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="79b18-112">تكوين إعدادات التدقيق لمجموعة مواقع</span><span class="sxs-lookup"><span data-stu-id="79b18-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="79b18-113">سجلات تدقيق اتّحدت SharePoint وOneDrive الحديثة من الامتثال</span><span class="sxs-lookup"><span data-stu-id="79b18-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="79b18-114">تشغيل/إيقاف تسجيل التدقيق الموحد</span><span class="sxs-lookup"><span data-stu-id="79b18-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="79b18-115">لا يوجد تكوين إضافي مطلوب داخل SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="79b18-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="79b18-116">استخدم بحث تسجيل التدقيق للتحقق من نشاط الملف (الملفات) والمجلد (المجلدات) والمستخدم (الأذونات) والأذونات:</span><span class="sxs-lookup"><span data-stu-id="79b18-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="79b18-117">أنشطة الملفات والصفحات</span><span class="sxs-lookup"><span data-stu-id="79b18-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="79b18-118">أنشطة المجلد</span><span class="sxs-lookup"><span data-stu-id="79b18-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="79b18-119">أنشطة المشاركة وطلب الوصول</span><span class="sxs-lookup"><span data-stu-id="79b18-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="79b18-120">أنشطة المزامنة</span><span class="sxs-lookup"><span data-stu-id="79b18-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="79b18-121">أنشطة إدارة الموقع</span><span class="sxs-lookup"><span data-stu-id="79b18-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="79b18-122">لمزيد من المعلومات حول كيفية استرداد هذه الأحداث، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="79b18-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
